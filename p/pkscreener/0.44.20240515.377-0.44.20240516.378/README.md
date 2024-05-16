# Comparing `tmp/pkscreener-0.44.20240515.377.tar.gz` & `tmp/pkscreener-0.44.20240516.378.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240515.377.tar", last modified: Wed May 15 20:53:06 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240516.378.tar", last modified: Thu May 16 09:19:19 2024, max compression
```

## Comparing `pkscreener-0.44.20240515.377.tar` & `pkscreener-0.44.20240516.378.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 20:53:06.662270 pkscreener-0.44.20240515.377/
--rw-rw-rw-   0        0        0     1086 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-05-15 20:53:06.662270 pkscreener-0.44.20240515.377/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 20:53:06.646645 pkscreener-0.44.20240515.377/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 20:53:06.662270 pkscreener-0.44.20240515.377/pkscreener/classes/
--rw-rw-rw-   0        0        0    13324 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/ArtTexts.py
--rw-rw-rw-   0        0        0    10156 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1537 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    34250 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0    10076 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0    11407 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    42465 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    12534 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    24534 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    22221 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8158 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    18947 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   154876 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    56135 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4993 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    84592 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3789 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-15 20:53:00.000000 pkscreener-0.44.20240515.377/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     5262 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   141172 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/globals.py
--rw-rw-rw-   0        0        0     1090 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    53036 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    33205 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-05-15 20:53:06.646645 pkscreener-0.44.20240515.377/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-05-15 20:53:06.000000 pkscreener-0.44.20240515.377/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2024-05-15 20:53:06.000000 pkscreener-0.44.20240515.377/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 20:53:06.000000 pkscreener-0.44.20240515.377/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-05-15 20:53:06.000000 pkscreener-0.44.20240515.377/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-15 20:53:06.000000 pkscreener-0.44.20240515.377/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-15 20:53:06.000000 pkscreener-0.44.20240515.377/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-15 20:53:06.662270 pkscreener-0.44.20240515.377/setup.cfg
--rw-rw-rw-   0        0        0     4765 2024-05-15 20:49:48.000000 pkscreener-0.44.20240515.377/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:19:19.849475 pkscreener-0.44.20240516.378/
+-rw-rw-rw-   0        0        0     1086 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-05-16 09:19:19.849475 pkscreener-0.44.20240516.378/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 09:19:19.833866 pkscreener-0.44.20240516.378/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:19:19.849475 pkscreener-0.44.20240516.378/pkscreener/classes/
+-rw-rw-rw-   0        0        0    13324 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/ArtTexts.py
+-rw-rw-rw-   0        0        0    10156 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1537 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    34250 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10076 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    11407 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    42703 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    12534 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    24534 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    22221 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8158 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    18947 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   155530 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    56135 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4993 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    84725 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3789 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-16 09:19:05.000000 pkscreener-0.44.20240516.378/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     5262 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   141394 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/globals.py
+-rw-rw-rw-   0        0        0     1090 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    53036 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    33750 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:19:19.833866 pkscreener-0.44.20240516.378/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-05-16 09:19:19.000000 pkscreener-0.44.20240516.378/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2024-05-16 09:19:19.000000 pkscreener-0.44.20240516.378/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 09:19:19.000000 pkscreener-0.44.20240516.378/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-05-16 09:19:19.000000 pkscreener-0.44.20240516.378/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-16 09:19:19.000000 pkscreener-0.44.20240516.378/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-16 09:19:19.000000 pkscreener-0.44.20240516.378/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-16 09:19:19.849475 pkscreener-0.44.20240516.378/setup.cfg
+-rw-rw-rw-   0        0        0     4765 2024-05-16 09:14:30.000000 pkscreener-0.44.20240516.378/setup.py
```

### Comparing `pkscreener-0.44.20240515.377/LICENSE` & `pkscreener-0.44.20240516.378/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.377/LICENSE-Others` & `pkscreener-0.44.20240516.378/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.377/PKG-INFO` & `pkscreener-0.44.20240516.378/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240515.377
+Version: 0.44.20240516.378
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240515.377.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240516.378.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240515.376/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240515.377/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240515.376/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240515.377/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240515.376/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240515.377/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240515.377/README.md` & `pkscreener-0.44.20240516.378/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240515.376/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240515.377/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240515.376/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240515.377/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240515.376/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240515.377/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240515.377/pkscreener/__init__.py` & `pkscreener-0.44.20240516.378/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.377/pkscreener/classes/ArtTexts.py` & `pkscreener-0.44.20240516.378/pkscreener/classes/ArtTexts.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.377/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240516.378/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.377/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240516.378/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.377/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240516.378/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.377/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240516.378/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.377/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240516.378/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.377/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240516.378/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.377/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.44.20240516.378/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.377/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240516.378/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.377/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240516.378/pkscreener/classes/MenuOptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,38 +56,42 @@
     "Z": "Exit (Ctrl + C)",
 }
 level1_P_MenuDict = {
     "1": "Predefined Piped Scanners",
     "2": "Define my custom Piped Scanner",
     "M": "Back to the Top/Main menu",
 }
-PREDEFINED_SCAN_MENU_KEYS = ["1","2","3","4","5","6","7","8"]
+PREDEFINED_SCAN_MENU_KEYS = ["1","2","3","4","5","6","7","8","9","10"]
 PREDEFINED_SCAN_MENU_TEXTS = [
     "Volume Scanners | High Momentum | Breaking Out Now | ATR Cross",
     "Volume Scanners | High Momentum | ATR Cross",
     "Volume Scanners | High Momentum",
     "Volume Scanners | ATR Cross",
     "Volume Scanners | High Bid/Ask Build Up",
     "High Momentum | ATR Cross",
     "High Momentum | ATR Trailing Stop",
     "ATR Cross | ATR Trailing Stop",
+    "TTM Sqeeze Buy | Intraday RSI b/w 0 to 54",
+    "Volume Scanners | ATR Cross | Intraday RSI b/w 0 to 54",
 ]
 level2_P_MenuDict = {}
 for key in PREDEFINED_SCAN_MENU_KEYS:
     level2_P_MenuDict[key] = PREDEFINED_SCAN_MENU_TEXTS[int(key)-1]
 level2_P_MenuDict["M"] = "Back to the Top/Main menu"
 PREDEFINED_SCAN_MENU_VALUES =[
-    "-a y -e -o 'X:12:9:2.5:;|X:0:31:;|X:0:23:;|X:0:27:'",
-    "-a y -e -o 'X:12:9:2.5:;|X:0:31:;|X:0:27:'",
-    "-a y -e -o 'X:12:9:2.5:;|X:0:31:'",
-    "-a y -e -o 'X:12:9:2.5:;|X:0:27:'",
-    "-a y -e -o 'X:12:9:2.5:;|X:0:29:'",
-    "-a y -e -o 'X:12:31:;|X:0:27:'",
-    "-a y -e -o 'X:12:31:;|X:0:30:1:'",
-    "-a y -e -o 'X:12:27:;|X:0:30:1:'",
+    "-a y -e -o 'X:12:9:2.5:>|X:0:31:>|X:0:23:>|X:0:27:'",
+    "-a y -e -o 'X:12:9:2.5:>|X:0:31:>|X:0:27:'",
+    "-a y -e -o 'X:12:9:2.5:>|X:0:31:'",
+    "-a y -e -o 'X:12:9:2.5:>|X:0:27:'",
+    "-a y -e -o 'X:12:9:2.5:>|X:0:29:'",
+    "-a y -e -o 'X:12:31:>|X:0:27:'",
+    "-a y -e -o 'X:12:31:>|X:0:30:1:'",
+    "-a y -e -o 'X:12:27:>|X:0:30:1:'",
+    "-a y -e -o 'X:12:7:6:1:>|X:0:5:0:54:i 1m'",
+    "-a y -e -o 'X:12:9:2.5:>|X:0:27:>|X:0:5:0:54:i 1m'"
 ]
 PIPED_SCANNERS = {}
 for key in PREDEFINED_SCAN_MENU_KEYS:
     PIPED_SCANNERS[key] = PREDEFINED_SCAN_MENU_VALUES[int(key)-1]
 
 level1_T_MenuDict = {
     "L": "Long Term",
@@ -181,15 +185,15 @@
     "M": "Back to the Top/Main menu",
     "Z": "Exit (Ctrl + C)",
 }
 level3_X_Reversal_MenuDict = {
     "1": "Buy Signals (Bullish Reversal)",
     "2": "Sell Signals (Bearish Reversal)",
     "3": "Momentum Gainers (Rising Bullish Momentum)",
-    "4": "Reversal at Moving Average (Bullish Reversal)",
+    "4": "Reversal at Moving Average (Bullish/Bearish Reversal)",
     "5": "Volume Spread Analysis (Bullish VSA Reversal)",
     "6": "Narrow Range (NRx) Reversal",
     "7": "Lorentzian Classifier (Machine Learning based indicator)",
     "8": "PSAR and RSI reversal",
     "9": "Rising RSI",
     "10": "RSI MA Reversal",
     "0": "Cancel",
```

### Comparing `pkscreener-0.44.20240515.377/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240516.378/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.377/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240516.378/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.377/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240516.378/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.377/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240516.378/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.377/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240516.378/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.377/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240516.378/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.377/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240516.378/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.377/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240516.378/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.377/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240516.378/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.377/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240516.378/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.377/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240516.378/pkscreener/classes/ScreeningStatistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -3867,5814 +3867,5855 @@
 0000f1a0: 3032 293a 0d0a 2020 2020 2020 2020 6966  02):..        if
 0000f1b0: 2064 6620 6973 204e 6f6e 6520 6f72 206c   df is None or l
 0000f1c0: 656e 2864 6629 203d 3d20 303a 0d0a 2020  en(df) == 0:..  
 0000f1d0: 2020 2020 2020 2020 2020 7265 7475 726e            return
 0000f1e0: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
 0000f1f0: 6461 7461 203d 2064 662e 636f 7079 2829  data = df.copy()
 0000f200: 0d0a 2020 2020 2020 2020 6d61 5261 6e67  ..        maRang
-0000f210: 6520 3d20 5b31 302c 2032 302c 2035 302c  e = [10, 20, 50,
-0000f220: 2032 3030 5d0d 0a20 2020 2020 2020 2072   200]..        r
-0000f230: 6573 756c 7473 203d 205b 5d0d 0a20 2020  esults = []..   
-0000f240: 2020 2020 2068 6173 5265 7665 7273 616c       hasReversal
-0000f250: 7320 3d20 4661 6c73 650d 0a20 2020 2020  s = False..     
-0000f260: 2020 2064 6174 6120 3d20 6461 7461 5b3a     data = data[:
-0000f270: 3a2d 315d 0d0a 2020 2020 2020 2020 7361  :-1]..        sa
-0000f280: 7665 6420 3d20 7365 6c66 2e66 696e 6443  ved = self.findC
-0000f290: 7572 7265 6e74 5361 7665 6456 616c 7565  urrentSavedValue
-0000f2a0: 2873 6372 6565 6e44 6963 742c 7361 7665  (screenDict,save
-0000f2b0: 4469 6374 2c20 224d 412d 5369 676e 616c  Dict, "MA-Signal
-0000f2c0: 2229 0d0a 2020 2020 2020 2020 666f 7220  ")..        for 
-0000f2d0: 6d61 4c65 6e67 7468 2069 6e20 6d61 5261  maLength in maRa
-0000f2e0: 6e67 653a 0d0a 2020 2020 2020 2020 2020  nge:..          
-0000f2f0: 2020 6461 7461 436f 7079 203d 2064 6174    dataCopy = dat
-0000f300: 610d 0a20 2020 2020 2020 2020 2020 2069  a..            i
-0000f310: 6620 7365 6c66 2e63 6f6e 6669 674d 616e  f self.configMan
-0000f320: 6167 6572 2e75 7365 454d 413a 0d0a 2020  ager.useEMA:..  
-0000f330: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
-0000f340: 5265 7620 3d20 706b 7461 6c69 622e 454d  Rev = pktalib.EM
-0000f350: 4128 6461 7461 436f 7079 5b22 436c 6f73  A(dataCopy["Clos
-0000f360: 6522 5d2c 2074 696d 6570 6572 696f 643d  e"], timeperiod=
-0000f370: 6d61 4c65 6e67 7468 290d 0a20 2020 2020  maLength)..     
-0000f380: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-0000f390: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
-0000f3a0: 5265 7620 3d20 706b 7461 6c69 622e 4d41  Rev = pktalib.MA
-0000f3b0: 2864 6174 6143 6f70 795b 2243 6c6f 7365  (dataCopy["Close
-0000f3c0: 225d 2c20 7469 6d65 7065 7269 6f64 3d6d  "], timeperiod=m
-0000f3d0: 614c 656e 6774 6829 0d0a 2020 2020 2020  aLength)..      
-0000f3e0: 2020 2020 2020 7472 793a 0d0a 2020 2020        try:..    
-0000f3f0: 2020 2020 2020 2020 2020 2020 6461 7461              data
-0000f400: 436f 7079 2e64 726f 7028 226d 6152 6576  Copy.drop("maRev
-0000f410: 222c 2061 7869 733d 312c 2069 6e70 6c61  ", axis=1, inpla
-0000f420: 6365 3d54 7275 652c 2065 7272 6f72 733d  ce=True, errors=
-0000f430: 2269 676e 6f72 6522 290d 0a20 2020 2020  "ignore")..     
-0000f440: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
-0000f450: 6365 7074 696f 6e3a 2320 7072 6167 6d61  ception:# pragma
-0000f460: 3a20 6e6f 2063 6f76 6572 0d0a 2020 2020  : no cover..    
-0000f470: 2020 2020 2020 2020 2020 2020 7061 7373              pass
-0000f480: 0d0a 2020 2020 2020 2020 2020 2020 6461  ..            da
-0000f490: 7461 436f 7079 2e69 6e73 6572 7428 6c65  taCopy.insert(le
-0000f4a0: 6e28 6461 7461 436f 7079 2e63 6f6c 756d  n(dataCopy.colum
-0000f4b0: 6e73 292c 2022 6d61 5265 7622 2c20 6d61  ns), "maRev", ma
-0000f4c0: 5265 7629 0d0a 2020 2020 2020 2020 2020  Rev)..          
-0000f4d0: 2020 6461 7461 436f 7079 203d 2064 6174    dataCopy = dat
-0000f4e0: 6143 6f70 795b 3a3a 2d31 5d2e 6865 6164  aCopy[::-1].head
-0000f4f0: 2833 290d 0a20 2020 2020 2020 2020 2020  (3)..           
-0000f500: 2069 6620 280d 0a20 2020 2020 2020 2020   if (..         
-0000f510: 2020 2020 2020 2064 6174 6143 6f70 792e         dataCopy.
-0000f520: 6571 7561 6c73 280d 0a20 2020 2020 2020  equals(..       
-0000f530: 2020 2020 2020 2020 2020 2020 2064 6174               dat
-0000f540: 6143 6f70 795b 0d0a 2020 2020 2020 2020  aCopy[..        
-0000f550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f560: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
-0000f570: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-0000f580: 6174 6143 6f70 792e 436c 6f73 650d 0a20  ataCopy.Close.. 
-0000f590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f5a0: 2020 2020 2020 2020 2020 203e 3d20 2864             >= (d
-0000f5b0: 6174 6143 6f70 792e 6d61 5265 7620 2d20  ataCopy.maRev - 
-0000f5c0: 2864 6174 6143 6f70 792e 6d61 5265 7620  (dataCopy.maRev 
-0000f5d0: 2a20 7065 7263 656e 7461 6765 2929 0d0a  * percentage))..
-0000f5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f5f0: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
-0000f600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f610: 2020 2026 2028 0d0a 2020 2020 2020 2020     & (..        
-0000f620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f630: 2020 2020 6461 7461 436f 7079 2e43 6c6f      dataCopy.Clo
-0000f640: 7365 0d0a 2020 2020 2020 2020 2020 2020  se..            
-0000f650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f660: 3c3d 2028 6461 7461 436f 7079 2e6d 6152  <= (dataCopy.maR
-0000f670: 6576 202b 2028 6461 7461 436f 7079 2e6d  ev + (dataCopy.m
-0000f680: 6152 6576 202a 2070 6572 6365 6e74 6167  aRev * percentag
-0000f690: 6529 290d 0a20 2020 2020 2020 2020 2020  e))..           
-0000f6a0: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
-0000f6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f6c0: 2020 2020 5d0d 0a20 2020 2020 2020 2020      ]..         
-0000f6d0: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-0000f6e0: 2020 2020 2020 2020 2020 616e 6420 6461            and da
-0000f6f0: 7461 436f 7079 2e68 6561 6428 3129 5b22  taCopy.head(1)["
-0000f700: 436c 6f73 6522 5d2e 696c 6f63 5b30 5d0d  Close"].iloc[0].
-0000f710: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f720: 203e 3d20 6461 7461 436f 7079 2e68 6561   >= dataCopy.hea
-0000f730: 6428 3129 5b22 6d61 5265 7622 5d2e 696c  d(1)["maRev"].il
-0000f740: 6f63 5b30 5d0d 0a20 2020 2020 2020 2020  oc[0]..         
-0000f750: 2020 2029 3a0d 0a20 2020 2020 2020 2020     ):..         
-0000f760: 2020 2020 2020 2068 6173 5265 7665 7273         hasRevers
-0000f770: 616c 7320 3d20 5472 7565 0d0a 2020 2020  als = True..    
-0000f780: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-0000f790: 6c74 732e 6170 7065 6e64 2873 7472 286d  lts.append(str(m
-0000f7a0: 614c 656e 6774 6829 290d 0a20 2020 2020  aLength))..     
-0000f7b0: 2020 2069 6620 6861 7352 6576 6572 7361     if hasReversa
-0000f7c0: 6c73 3a0d 0a20 2020 2020 2020 2020 2020  ls:..           
-0000f7d0: 2073 6372 6565 6e44 6963 745b 224d 412d   screenDict["MA-
-0000f7e0: 5369 676e 616c 225d 203d 2028 0d0a 2020  Signal"] = (..  
-0000f7f0: 2020 2020 2020 2020 2020 2020 2020 7361                sa
-0000f800: 7665 645b 305d 200d 0a20 2020 2020 2020  ved[0] ..       
-0000f810: 2020 2020 2020 2020 202b 2063 6f6c 6f72           + color
-0000f820: 5465 7874 2e42 4f4c 440d 0a20 2020 2020  Text.BOLD..     
-0000f830: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
-0000f840: 6f72 5465 7874 2e47 5245 454e 0d0a 2020  orText.GREEN..  
-0000f850: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-0000f860: 6622 5265 7665 7273 616c 2d5b 7b27 2c27  f"Reversal-[{','
-0000f870: 2e6a 6f69 6e28 7265 7375 6c74 7329 7d5d  .join(results)}]
-0000f880: 4d41 220d 0a20 2020 2020 2020 2020 2020  MA"..           
-0000f890: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
-0000f8a0: 2e45 4e44 0d0a 2020 2020 2020 2020 2020  .END..          
-0000f8b0: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
-0000f8c0: 2073 6176 6544 6963 745b 224d 412d 5369   saveDict["MA-Si
-0000f8d0: 676e 616c 225d 203d 2073 6176 6564 5b31  gnal"] = saved[1
-0000f8e0: 5d20 2b20 6622 5265 7665 7273 616c 2d5b  ] + f"Reversal-[
-0000f8f0: 7b27 2c27 2e6a 6f69 6e28 7265 7375 6c74  {','.join(result
-0000f900: 7329 7d5d 4d41 220d 0a20 2020 2020 2020  s)}]MA"..       
-0000f910: 2072 6574 7572 6e20 6861 7352 6576 6572   return hasRever
-0000f920: 7361 6c73 0d0a 0d0a 2020 2020 6465 6620  sals....    def 
-0000f930: 6669 6e64 4375 7272 656e 7453 6176 6564  findCurrentSaved
-0000f940: 5661 6c75 6528 7365 6c66 2c20 7363 7265  Value(self, scre
-0000f950: 656e 4469 6374 2c20 7361 7665 4469 6374  enDict, saveDict
-0000f960: 2c20 6b65 7929 3a0d 0a20 2020 2020 2020  , key):..       
-0000f970: 2065 7869 7374 696e 6753 6372 6565 6e20   existingScreen 
-0000f980: 3d20 7363 7265 656e 4469 6374 2e67 6574  = screenDict.get
-0000f990: 286b 6579 290d 0a20 2020 2020 2020 2065  (key)..        e
-0000f9a0: 7869 7374 696e 6753 6176 6520 3d20 7361  xistingSave = sa
-0000f9b0: 7665 4469 6374 2e67 6574 286b 6579 290d  veDict.get(key).
-0000f9c0: 0a20 2020 2020 2020 2065 7869 7374 696e  .        existin
-0000f9d0: 6753 6372 6565 6e20 3d20 6622 7b65 7869  gScreen = f"{exi
-0000f9e0: 7374 696e 6753 6372 6565 6e7d 2c20 2220  stingScreen}, " 
-0000f9f0: 6966 2028 6578 6973 7469 6e67 5363 7265  if (existingScre
-0000fa00: 656e 2069 7320 6e6f 7420 4e6f 6e65 2061  en is not None a
-0000fa10: 6e64 206c 656e 2865 7869 7374 696e 6753  nd len(existingS
-0000fa20: 6372 6565 6e29 203e 2030 2920 656c 7365  creen) > 0) else
-0000fa30: 2022 220d 0a20 2020 2020 2020 2065 7869   ""..        exi
-0000fa40: 7374 696e 6753 6176 6520 3d20 6622 7b65  stingSave = f"{e
-0000fa50: 7869 7374 696e 6753 6176 657d 2c20 2220  xistingSave}, " 
-0000fa60: 6966 2028 6578 6973 7469 6e67 5361 7665  if (existingSave
-0000fa70: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
-0000fa80: 206c 656e 2865 7869 7374 696e 6753 6176   len(existingSav
-0000fa90: 6529 203e 2030 2920 656c 7365 2022 220d  e) > 0) else "".
-0000faa0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000fab0: 6578 6973 7469 6e67 5363 7265 656e 2c20  existingScreen, 
-0000fac0: 6578 6973 7469 6e67 5361 7665 0d0a 0d0a  existingSave....
-0000fad0: 2020 2020 2320 406d 6561 7375 7265 5f74      # @measure_t
-0000fae0: 696d 650d 0a20 2020 2064 6566 2066 696e  ime..    def fin
-0000faf0: 6442 6261 6e64 7353 7175 6565 7a65 2873  dBbandsSqueeze(s
-0000fb00: 656c 662c 6675 6c6c 4461 7461 2c20 7363  elf,fullData, sc
-0000fb10: 7265 656e 4469 6374 2c20 7361 7665 4469  reenDict, saveDi
-0000fb20: 6374 2c20 6669 6c74 6572 3d34 293a 0d0a  ct, filter=4):..
-0000fb30: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-0000fb40: 2020 2020 2054 6865 2054 544d 2053 7175       The TTM Squ
-0000fb50: 6565 7a65 2069 6e64 6963 6174 6f72 206d  eeze indicator m
-0000fb60: 6561 7375 7265 7320 7468 6520 7265 6c61  easures the rela
-0000fb70: 7469 6f6e 7368 6970 2062 6574 7765 656e  tionship between
-0000fb80: 2074 6865 200d 0a20 2020 2020 2020 2042   the ..        B
-0000fb90: 6f6c 6c69 6e67 6572 2042 616e 6473 2061  ollinger Bands a
-0000fba0: 6e64 204b 656c 746e 6572 2773 2043 6861  nd Keltner's Cha
-0000fbb0: 6e6e 656c 2e20 5768 656e 2074 6865 2076  nnel. When the v
-0000fbc0: 6f6c 6174 696c 6974 7920 696e 6372 6561  olatility increa
-0000fbd0: 7365 732c 200d 0a20 2020 2020 2020 2073  ses, ..        s
-0000fbe0: 6f20 646f 6573 2074 6865 2064 6973 7461  o does the dista
-0000fbf0: 6e63 6520 6265 7477 6565 6e20 7468 6520  nce between the 
-0000fc00: 6261 6e64 732c 2061 6e64 2063 6f6e 7665  bands, and conve
-0000fc10: 7273 656c 792c 2077 6865 6e20 7468 6520  rsely, when the 
-0000fc20: 0d0a 2020 2020 2020 2020 766f 6c61 7469  ..        volati
-0000fc30: 6c69 7479 2064 6563 6c69 6e65 732c 2074  lity declines, t
-0000fc40: 6865 2064 6973 7461 6e63 6520 616c 736f  he distance also
-0000fc50: 2064 6563 7265 6173 6573 2e20 5468 6520   decreases. The 
-0000fc60: 5371 7565 657a 6520 696e 6469 6361 746f  Squeeze indicato
-0000fc70: 7220 0d0a 2020 2020 2020 2020 6669 6e64  r ..        find
-0000fc80: 7320 7365 6374 696f 6e73 206f 6620 7468  s sections of th
-0000fc90: 6520 426f 6c6c 696e 6765 7220 4261 6e64  e Bollinger Band
-0000fca0: 7320 7374 7564 7920 7768 6963 6820 6661  s study which fa
-0000fcb0: 6c6c 2069 6e73 6964 6520 7468 6520 0d0a  ll inside the ..
-0000fcc0: 2020 2020 2020 2020 4b65 6c74 6e65 7227          Keltner'
-0000fcd0: 7320 4368 616e 6e65 6c73 2e0d 0a20 2020  s Channels...   
-0000fce0: 2020 2020 200d 0a20 2020 2020 2020 2041       ..        A
-0000fcf0: 7420 7468 6520 6d6f 6d65 6e74 2074 6869  t the moment thi
-0000fd00: 7320 7371 7565 657a 6520 6861 7070 656e  s squeeze happen
-0000fd10: 732c 2061 2070 7269 6365 2062 7265 616b  s, a price break
-0000fd20: 6f75 7420 6672 6f6d 2074 6865 2075 7070  out from the upp
-0000fd30: 6572 200d 0a20 2020 2020 2020 2042 6f6c  er ..        Bol
-0000fd40: 6c69 6e67 6572 2042 616e 6420 776f 756c  linger Band woul
-0000fd50: 6420 696e 6469 6361 7465 2074 6865 2070  d indicate the p
-0000fd60: 6f73 7369 6269 6c69 7479 206f 6620 616e  ossibility of an
-0000fd70: 2075 7074 7265 6e64 2069 6e20 7468 6520   uptrend in the 
-0000fd80: 0d0a 2020 2020 2020 2020 6675 7475 7265  ..        future
-0000fd90: 2e20 5468 6973 2069 7320 6261 636b 6564  . This is backed
-0000fda0: 2062 7920 7468 6520 6661 6374 2074 6861   by the fact tha
-0000fdb0: 7420 6f6e 6365 2074 6865 2070 7269 6365  t once the price
-0000fdc0: 2073 7461 7274 7320 6272 6561 6b69 6e67   starts breaking
-0000fdd0: 200d 0a20 2020 2020 2020 206f 7574 206f   ..        out o
-0000fde0: 6620 7468 6520 6261 6e64 732c 2069 7420  f the bands, it 
-0000fdf0: 776f 756c 6420 6d65 616e 2061 2072 656c  would mean a rel
-0000fe00: 6178 6174 696f 6e20 6f66 2074 6865 2073  axation of the s
-0000fe10: 7175 6565 7a65 2061 6e64 2074 6865 200d  queeze and the .
-0000fe20: 0a20 2020 2020 2020 2070 6f73 7369 6269  .        possibi
-0000fe30: 6c69 7479 206f 6620 6869 6768 206d 6172  lity of high mar
-0000fe40: 6b65 7420 766f 6c61 7469 6c69 7479 2061  ket volatility a
-0000fe50: 6e64 2070 7269 6365 206d 6f76 656d 656e  nd price movemen
-0000fe60: 7420 696e 2074 6865 2066 7574 7572 652e  t in the future.
-0000fe70: 200d 0a20 2020 2020 2020 2053 696d 696c   ..        Simil
-0000fe80: 6172 6c79 2c20 6120 7072 6963 6520 6272  arly, a price br
-0000fe90: 6561 6b6f 7574 2066 726f 6d20 7468 6520  eakout from the 
-0000fea0: 6c6f 7765 7220 426f 6c6c 696e 6765 7220  lower Bollinger 
-0000feb0: 4261 6e64 2061 6674 6572 2061 2073 7175  Band after a squ
-0000fec0: 6565 7a65 200d 0a20 2020 2020 2020 2077  eeze ..        w
-0000fed0: 6f75 6c64 2069 6e64 6963 6174 6520 7468  ould indicate th
-0000fee0: 6520 706f 7373 6962 696c 6974 7920 6f66  e possibility of
-0000fef0: 2061 2064 6f77 6e74 7265 6e64 2069 6e20   a downtrend in 
-0000ff00: 7468 6520 6675 7475 7265 2061 6e64 2061  the future and a
-0000ff10: 6e20 0d0a 2020 2020 2020 2020 696e 6372  n ..        incr
-0000ff20: 6561 7365 6420 6d61 726b 6574 2076 6f6c  eased market vol
-0000ff30: 6174 696c 6974 7920 696e 2074 6865 2073  atility in the s
-0000ff40: 616d 6520 6469 7265 6374 696f 6e2e 2057  ame direction. W
-0000ff50: 6865 6e20 7468 6520 6d61 726b 6574 200d  hen the market .
-0000ff60: 0a20 2020 2020 2020 2066 696e 6973 6865  .        finishe
-0000ff70: 7320 6120 6d6f 7665 2c20 7468 6520 696e  s a move, the in
-0000ff80: 6469 6361 746f 7220 7475 726e 7320 6f66  dicator turns of
-0000ff90: 662c 2077 6869 6368 2063 6f72 7265 7370  f, which corresp
-0000ffa0: 6f6e 6473 2074 6f20 6261 6e64 7320 0d0a  onds to bands ..
-0000ffb0: 2020 2020 2020 2020 6861 7669 6e67 2070          having p
-0000ffc0: 7573 6865 6420 7765 6c6c 206f 7574 7369  ushed well outsi
-0000ffd0: 6465 2074 6865 2072 616e 6765 206f 6620  de the range of 
-0000ffe0: 4b65 6c74 6e65 7227 7320 4368 616e 6e65  Keltner's Channe
-0000fff0: 6c73 2e0d 0a20 2020 2020 2020 2022 2222  ls...        """
-00010000: 0d0a 2020 2020 2020 2020 6966 2066 756c  ..        if ful
-00010010: 6c44 6174 6120 6973 204e 6f6e 6520 6f72  lData is None or
-00010020: 206c 656e 2866 756c 6c44 6174 6129 203c   len(fullData) <
-00010030: 2032 303a 0d0a 2020 2020 2020 2020 2020   20:..          
-00010040: 2020 7265 7475 726e 2046 616c 7365 0d0a    return False..
-00010050: 2020 2020 2020 2020 6f6c 6465 7374 5265          oldestRe
-00010060: 636f 7264 7346 6972 7374 5f64 6620 3d20  cordsFirst_df = 
-00010070: 6675 6c6c 4461 7461 2e68 6561 6428 3330  fullData.head(30
-00010080: 292e 636f 7079 2829 0d0a 2020 2020 2020  ).copy()..      
-00010090: 2020 6c61 7465 7374 5265 636f 7264 7346    latestRecordsF
-000100a0: 6972 7374 5f64 6620 3d20 6f6c 6465 7374  irst_df = oldest
-000100b0: 5265 636f 7264 7346 6972 7374 5f64 665b  RecordsFirst_df[
-000100c0: 3a3a 2d31 5d2e 7461 696c 2833 3029 0d0a  ::-1].tail(30)..
-000100d0: 2020 2020 2020 2020 6c61 7465 7374 5265          latestRe
-000100e0: 636f 7264 7346 6972 7374 5f64 6620 3d20  cordsFirst_df = 
-000100f0: 6c61 7465 7374 5265 636f 7264 7346 6972  latestRecordsFir
-00010100: 7374 5f64 662e 6669 6c6c 6e61 2830 290d  st_df.fillna(0).
-00010110: 0a20 2020 2020 2020 206c 6174 6573 7452  .        latestR
-00010120: 6563 6f72 6473 4669 7273 745f 6466 203d  ecordsFirst_df =
-00010130: 206c 6174 6573 7452 6563 6f72 6473 4669   latestRecordsFi
-00010140: 7273 745f 6466 2e72 6570 6c61 6365 285b  rst_df.replace([
-00010150: 6e70 2e69 6e66 2c20 2d6e 702e 696e 665d  np.inf, -np.inf]
-00010160: 2c20 3029 0d0a 2020 2020 2020 2020 2320  , 0)..        # 
-00010170: 426f 6c6c 696e 6765 7220 6261 6e64 730d  Bollinger bands.
-00010180: 0a20 2020 2020 2020 206c 6174 6573 7452  .        latestR
-00010190: 6563 6f72 6473 4669 7273 745f 6466 2e6c  ecordsFirst_df.l
-000101a0: 6f63 5b3a 2c27 4242 616e 6473 2d55 275d  oc[:,'BBands-U']
-000101b0: 2c20 6c61 7465 7374 5265 636f 7264 7346  , latestRecordsF
-000101c0: 6972 7374 5f64 662e 6c6f 635b 3a2c 2742  irst_df.loc[:,'B
-000101d0: 4261 6e64 732d 4d27 5d2c 206c 6174 6573  Bands-M'], lates
-000101e0: 7452 6563 6f72 6473 4669 7273 745f 6466  tRecordsFirst_df
-000101f0: 2e6c 6f63 5b3a 2c27 4242 616e 6473 2d4c  .loc[:,'BBands-L
-00010200: 275d 203d 2070 6b74 616c 6962 2e42 4241  '] = pktalib.BBA
-00010210: 4e44 5328 6c61 7465 7374 5265 636f 7264  NDS(latestRecord
-00010220: 7346 6972 7374 5f64 665b 2243 6c6f 7365  sFirst_df["Close
-00010230: 225d 2c20 3230 290d 0a20 2020 2020 2020  "], 20)..       
-00010240: 2023 2063 6f6d 7075 7465 204b 656c 746e   # compute Keltn
-00010250: 6572 2773 2063 6861 6e6e 656c 0d0a 2020  er's channel..  
-00010260: 2020 2020 2020 6c61 7465 7374 5265 636f        latestReco
-00010270: 7264 7346 6972 7374 5f64 665b 276c 6f77  rdsFirst_df['low
-00010280: 5f6b 656c 275d 2c20 6c61 7465 7374 5265  _kel'], latestRe
-00010290: 636f 7264 7346 6972 7374 5f64 665b 2775  cordsFirst_df['u
-000102a0: 7070 5f6b 656c 275d 203d 2070 6b74 616c  pp_kel'] = pktal
-000102b0: 6962 2e4b 656c 746e 6572 7343 6861 6e6e  ib.KeltnersChann
-000102c0: 656c 286c 6174 6573 7452 6563 6f72 6473  el(latestRecords
-000102d0: 4669 7273 745f 6466 5b22 4869 6768 225d  First_df["High"]
-000102e0: 2c20 6c61 7465 7374 5265 636f 7264 7346  , latestRecordsF
-000102f0: 6972 7374 5f64 665b 224c 6f77 225d 2c6c  irst_df["Low"],l
-00010300: 6174 6573 7452 6563 6f72 6473 4669 7273  atestRecordsFirs
-00010310: 745f 6466 5b22 436c 6f73 6522 5d2c 3230  t_df["Close"],20
-00010320: 290d 0a20 2020 2020 2020 2023 2073 7175  )..        # squ
-00010330: 6565 7a65 2069 6e64 6963 6174 6f72 0d0a  eeze indicator..
-00010340: 2020 2020 2020 2020 6465 6620 696e 5f73          def in_s
-00010350: 7175 6565 7a65 2864 6629 3a0d 0a20 2020  queeze(df):..   
-00010360: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00010370: 6466 5b27 6c6f 775f 6b65 6c27 5d20 3c20  df['low_kel'] < 
-00010380: 6466 5b27 4242 616e 6473 2d4c 275d 203c  df['BBands-L'] <
-00010390: 2064 665b 2742 4261 6e64 732d 5527 5d20   df['BBands-U'] 
-000103a0: 3c20 6466 5b27 7570 705f 6b65 6c27 5d0d  < df['upp_kel'].
-000103b0: 0a0d 0a20 2020 2020 2020 206c 6174 6573  ...        lates
-000103c0: 7452 6563 6f72 6473 4669 7273 745f 6466  tRecordsFirst_df
-000103d0: 5b27 7371 7565 657a 6527 5d20 3d20 6c61  ['squeeze'] = la
-000103e0: 7465 7374 5265 636f 7264 7346 6972 7374  testRecordsFirst
-000103f0: 5f64 662e 6170 706c 7928 696e 5f73 7175  _df.apply(in_squ
-00010400: 6565 7a65 2c20 6178 6973 3d31 290d 0a0d  eeze, axis=1)...
-00010410: 0a20 2020 2020 2020 2023 204c 6574 2773  .        # Let's
-00010420: 2072 6576 6965 7720 6a75 7374 2074 6865   review just the
-00010430: 2070 7265 7669 6f75 7320 3320 6361 6e64   previous 3 cand
-00010440: 6c65 7320 696e 636c 7564 696e 6720 746f  les including to
-00010450: 6461 7920 2861 7420 7468 6520 656e 6429  day (at the end)
-00010460: 0d0a 2020 2020 2020 2020 6c61 7465 7374  ..        latest
-00010470: 5265 636f 7264 7346 6972 7374 5f64 6620  RecordsFirst_df 
-00010480: 3d20 6c61 7465 7374 5265 636f 7264 7346  = latestRecordsF
-00010490: 6972 7374 5f64 662e 7461 696c 2833 290d  irst_df.tail(3).
-000104a0: 0a20 2020 2020 2020 2023 2073 746f 636b  .        # stock
-000104b0: 2069 7320 636f 6d69 6e67 206f 7574 206f   is coming out o
-000104c0: 6620 7468 6520 7371 7565 657a 650d 0a20  f the squeeze.. 
-000104d0: 2020 2020 2020 2073 6176 6564 203d 2073         saved = s
-000104e0: 656c 662e 6669 6e64 4375 7272 656e 7453  elf.findCurrentS
-000104f0: 6176 6564 5661 6c75 6528 7363 7265 656e  avedValue(screen
-00010500: 4469 6374 2c20 7361 7665 4469 6374 2c20  Dict, saveDict, 
-00010510: 2250 6174 7465 726e 2229 0d0a 2020 2020  "Pattern")..    
-00010520: 2020 2020 6361 6e64 6c65 3353 717a 203d      candle3Sqz =
-00010530: 206c 6174 6573 7452 6563 6f72 6473 4669   latestRecordsFi
-00010540: 7273 745f 6466 2e69 6c6f 635b 2d33 5d5b  rst_df.iloc[-3][
-00010550: 2273 7175 6565 7a65 225d 0d0a 2020 2020  "squeeze"]..    
-00010560: 2020 2020 6361 6e64 6c65 3153 717a 203d      candle1Sqz =
-00010570: 206c 6174 6573 7452 6563 6f72 6473 4669   latestRecordsFi
-00010580: 7273 745f 6466 2e69 6c6f 635b 2d31 5d5b  rst_df.iloc[-1][
-00010590: 2273 7175 6565 7a65 225d 0d0a 2020 2020  "squeeze"]..    
-000105a0: 2020 2020 6361 6e64 6c65 3253 717a 203d      candle2Sqz =
-000105b0: 206c 6174 6573 7452 6563 6f72 6473 4669   latestRecordsFi
-000105c0: 7273 745f 6466 2e69 6c6f 635b 2d32 5d5b  rst_df.iloc[-2][
-000105d0: 2273 7175 6565 7a65 225d 0d0a 2020 2020  "squeeze"]..    
-000105e0: 2020 2020 6966 2063 616e 646c 6533 5371      if candle3Sq
-000105f0: 7a20 616e 6420 6e6f 7420 6361 6e64 6c65  z and not candle
-00010600: 3153 717a 3a0d 0a20 2020 2020 2020 2020  1Sqz:..         
-00010610: 2020 2023 2033 7264 2063 616e 646c 6520     # 3rd candle 
-00010620: 6672 6f6d 2074 6865 206d 6f73 7420 7265  from the most re
-00010630: 6365 6e74 206f 6e65 2077 6173 2069 6e20  cent one was in 
-00010640: 7371 7565 657a 6520 6275 7420 7468 6520  squeeze but the 
-00010650: 6d6f 7374 2072 6563 656e 7420 6f6e 6520  most recent one 
-00010660: 6973 206e 6f74 2e0d 0a20 2020 2020 2020  is not...       
-00010670: 2020 2020 2069 6620 6669 6c74 6572 206e       if filter n
-00010680: 6f74 2069 6e20 5b31 2c33 2c34 5d3a 2023  ot in [1,3,4]: #
-00010690: 2042 7579 2f53 656c 6c2f 416c 6c0d 0a20   Buy/Sell/All.. 
-000106a0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000106b0: 6574 7572 6e20 4661 6c73 650d 0a20 2020  eturn False..   
-000106c0: 2020 2020 2020 2020 2023 2064 6563 6964           # decid
-000106d0: 6520 7768 6963 6820 6163 7469 6f6e 2074  e which action t
-000106e0: 6f20 7461 6b65 2062 7920 636f 6d70 6172  o take by compar
-000106f0: 696e 6720 6469 7374 616e 6365 7320 2020  ing distances   
-00010700: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-00010710: 2020 2020 2020 2020 2020 2064 6973 7461             dista
-00010720: 6e63 655f 746f 5f75 7070 6572 203d 2061  nce_to_upper = a
-00010730: 6273 286c 6174 6573 7452 6563 6f72 6473  bs(latestRecords
-00010740: 4669 7273 745f 6466 5b27 4242 616e 6473  First_df['BBands
-00010750: 2d55 275d 2e76 616c 7565 735b 2d31 5d20  -U'].values[-1] 
-00010760: 2d20 6c61 7465 7374 5265 636f 7264 7346  - latestRecordsF
-00010770: 6972 7374 5f64 665b 2743 6c6f 7365 275d  irst_df['Close']
-00010780: 2e76 616c 7565 735b 2d31 5d29 0d0a 2020  .values[-1])..  
-00010790: 2020 2020 2020 2020 2020 6469 7374 616e            distan
-000107a0: 6365 5f74 6f5f 6c6f 7765 7220 3d20 6162  ce_to_lower = ab
-000107b0: 7328 6c61 7465 7374 5265 636f 7264 7346  s(latestRecordsF
-000107c0: 6972 7374 5f64 665b 2742 4261 6e64 732d  irst_df['BBands-
-000107d0: 4c27 5d2e 7661 6c75 6573 5b2d 315d 202d  L'].values[-1] -
-000107e0: 206c 6174 6573 7452 6563 6f72 6473 4669   latestRecordsFi
-000107f0: 7273 745f 6466 5b27 436c 6f73 6527 5d2e  rst_df['Close'].
-00010800: 7661 6c75 6573 5b2d 315d 290d 0a20 2020  values[-1])..   
-00010810: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00010820: 2020 2020 2020 2061 6374 696f 6e20 3d20         action = 
-00010830: 4661 6c73 650d 0a20 2020 2020 2020 2020  False..         
-00010840: 2020 2069 6620 6469 7374 616e 6365 5f74     if distance_t
-00010850: 6f5f 7570 7065 7220 3c20 6469 7374 616e  o_upper < distan
-00010860: 6365 5f74 6f5f 6c6f 7765 723a 0d0a 2020  ce_to_lower:..  
-00010870: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00010880: 2066 696c 7465 7220 6e6f 7420 696e 205b   filter not in [
-00010890: 312c 345d 3a20 2320 4275 792f 416c 6c0d  1,4]: # Buy/All.
-000108a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000108b0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
-000108c0: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
-000108d0: 2020 2061 6374 696f 6e20 3d20 5472 7565     action = True
-000108e0: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
-000108f0: 6966 2066 696c 7465 7220 6e6f 7420 696e  if filter not in
-00010900: 205b 332c 345d 3a20 2320 5365 6c6c 2f41   [3,4]: # Sell/A
-00010910: 6c6c 0d0a 2020 2020 2020 2020 2020 2020  ll..            
-00010920: 2020 2020 7265 7475 726e 2046 616c 7365      return False
-00010930: 0d0a 2020 2020 2020 2020 2020 2020 7363  ..            sc
-00010940: 7265 656e 4469 6374 5b22 5061 7474 6572  reenDict["Patter
-00010950: 6e22 5d20 3d20 7361 7665 645b 305d 202b  n"] = saved[0] +
-00010960: 2063 6f6c 6f72 5465 7874 2e42 4f4c 4420   colorText.BOLD 
-00010970: 2b20 2863 6f6c 6f72 5465 7874 2e47 5245  + (colorText.GRE
-00010980: 454e 2069 6620 6163 7469 6f6e 2065 6c73  EN if action els
-00010990: 6520 636f 6c6f 7254 6578 742e 4641 494c  e colorText.FAIL
-000109a0: 2920 2b20 6622 4242 616e 6473 2d53 515a  ) + f"BBands-SQZ
-000109b0: 2d7b 2742 7579 2720 6966 2061 6374 696f  -{'Buy' if actio
-000109c0: 6e20 656c 7365 2027 5365 6c6c 277d 2220  n else 'Sell'}" 
-000109d0: 2b20 636f 6c6f 7254 6578 742e 454e 440d  + colorText.END.
-000109e0: 0a20 2020 2020 2020 2020 2020 2073 6176  .            sav
-000109f0: 6544 6963 745b 2250 6174 7465 726e 225d  eDict["Pattern"]
-00010a00: 203d 2073 6176 6564 5b31 5d20 2b20 6622   = saved[1] + f"
-00010a10: 5454 4d2d 5351 5a2d 7b27 4275 7927 2069  TTM-SQZ-{'Buy' i
-00010a20: 6620 6163 7469 6f6e 2065 6c73 6520 2753  f action else 'S
-00010a30: 656c 6c27 7d22 0d0a 2020 2020 2020 2020  ell'}"..        
-00010a40: 2020 2020 7265 7475 726e 2054 7275 650d      return True.
-00010a50: 0a20 2020 2020 2020 2065 6c69 6620 6361  .        elif ca
-00010a60: 6e64 6c65 3353 717a 2061 6e64 2063 616e  ndle3Sqz and can
-00010a70: 646c 6532 5371 7a20 616e 6420 6361 6e64  dle2Sqz and cand
-00010a80: 6c65 3153 717a 3a0d 0a20 2020 2020 2020  le1Sqz:..       
-00010a90: 2020 2020 2023 204c 6173 7420 3320 6361       # Last 3 ca
-00010aa0: 6e64 6c65 7320 696e 2073 7175 6565 7a65  ndles in squeeze
-00010ab0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00010ac0: 2066 696c 7465 7220 6e6f 7420 696e 205b   filter not in [
-00010ad0: 322c 345d 3a20 2320 5371 5a2f 416c 6c0d  2,4]: # SqZ/All.
-00010ae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010af0: 2072 6574 7572 6e20 4661 6c73 650d 0a20   return False.. 
-00010b00: 2020 2020 2020 2020 2020 2073 6372 6565             scree
-00010b10: 6e44 6963 745b 2250 6174 7465 726e 225d  nDict["Pattern"]
-00010b20: 203d 2066 277b 7361 7665 645b 305d 7d7b   = f'{saved[0]}{
-00010b30: 636f 6c6f 7254 6578 742e 424f 4c44 7d7b  colorText.BOLD}{
-00010b40: 636f 6c6f 7254 6578 742e 5741 524e 7d54  colorText.WARN}T
-00010b50: 544d 2d53 515a 7b63 6f6c 6f72 5465 7874  TM-SQZ{colorText
-00010b60: 2e45 4e44 7d27 0d0a 2020 2020 2020 2020  .END}'..        
-00010b70: 2020 2020 7361 7665 4469 6374 5b22 5061      saveDict["Pa
-00010b80: 7474 6572 6e22 5d20 3d20 6627 7b73 6176  ttern"] = f'{sav
-00010b90: 6564 5b31 5d7d 5454 4d2d 5351 5a27 0d0a  ed[1]}TTM-SQZ'..
-00010ba0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00010bb0: 726e 2054 7275 650d 0a20 2020 2020 2020  rn True..       
-00010bc0: 2072 6574 7572 6e20 4661 6c73 650d 0a0d   return False...
-00010bd0: 0a20 2020 2064 6566 2066 696e 6449 6e74  .    def findInt
-00010be0: 7261 6461 7948 6967 6843 726f 7373 6f76  radayHighCrossov
-00010bf0: 6572 2873 656c 662c 2064 662c 2061 6674  er(self, df, aft
-00010c00: 6572 5469 6d65 7374 616d 703d 4e6f 6e65  erTimestamp=None
-00010c10: 293a 0d0a 2020 2020 2020 2020 6966 2064  ):..        if d
-00010c20: 6620 6973 204e 6f6e 6520 6f72 206c 656e  f is None or len
-00010c30: 2864 6629 203d 3d20 303a 0d0a 2020 2020  (df) == 0:..    
-00010c40: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-00010c50: 616c 7365 0d0a 2020 2020 2020 2020 6461  alse..        da
-00010c60: 7461 203d 2064 662e 636f 7079 2829 0d0a  ta = df.copy()..
-00010c70: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
-00010c80: 6174 612e 6669 6c6c 6e61 2830 290d 0a20  ata.fillna(0).. 
-00010c90: 2020 2020 2020 2064 6174 6120 3d20 6461         data = da
-00010ca0: 7461 2e72 6570 6c61 6365 285b 6e70 2e69  ta.replace([np.i
-00010cb0: 6e66 2c20 2d6e 702e 696e 665d 2c20 3029  nf, -np.inf], 0)
-00010cc0: 0d0a 2020 2020 2020 2020 6461 7461 203d  ..        data =
-00010cd0: 2064 6174 615b 3a3a 2d31 5d20 2023 2052   data[::-1]  # R
-00010ce0: 6576 6572 7365 2074 6865 2064 6174 6166  everse the dataf
-00010cf0: 7261 6d65 2073 6f20 7468 6174 2069 7473  rame so that its
-00010d00: 2074 6865 206f 6c64 6573 7420 6461 7465   the oldest date
-00010d10: 2066 6972 7374 0d0a 2020 2020 2020 2020   first..        
-00010d20: 6469 6666 5f64 6620 3d20 4e6f 6e65 0d0a  diff_df = None..
-00010d30: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
-00010d40: 2020 2020 2020 2020 2020 2320 4c65 7427            # Let'
-00010d50: 7320 6f6e 6c79 2063 6f6e 7369 6465 7220  s only consider 
-00010d60: 7468 6f73 6520 6361 6e64 6c65 7320 7468  those candles th
-00010d70: 6174 2061 7265 2061 6674 6572 2074 6865  at are after the
-00010d80: 2061 6c65 7274 2069 7373 7565 2d74 696d   alert issue-tim
-00010d90: 6520 696e 2074 6865 206d 6f72 6e69 6e67  e in the morning
-00010da0: 7320 2b20 3220 6361 6e64 6c65 7320 2866  s + 2 candles (f
-00010db0: 6f72 2062 7579 2f73 656c 6c29 0d0a 2020  or buy/sell)..  
-00010dc0: 2020 2020 2020 2020 2020 6469 6666 5f64            diff_d
-00010dd0: 6620 3d20 6461 7461 5b64 6174 612e 696e  f = data[data.in
-00010de0: 6465 7820 3e3d 2020 7064 2e74 6f5f 6461  dex >=  pd.to_da
-00010df0: 7465 7469 6d65 2866 277b 504b 4461 7465  tetime(f'{PKDate
-00010e00: 5574 696c 6974 6965 732e 7472 6164 696e  Utilities.tradin
-00010e10: 6744 6174 6528 292e 7374 7266 7469 6d65  gDate().strftime
-00010e20: 2866 2225 592d 256d 2d25 6422 297d 2030  (f"%Y-%m-%d")} 0
-00010e30: 393a 7b31 352b 7365 6c66 2e63 6f6e 6669  9:{15+self.confi
-00010e40: 674d 616e 6167 6572 2e6d 6f72 6e69 6e67  gManager.morning
-00010e50: 616e 616c 7973 6973 6361 6e64 6c65 6e75  analysiscandlenu
-00010e60: 6d62 6572 202b 2032 7d3a 3030 2b30 353a  mber + 2}:00+05:
-00010e70: 3330 2729 2e74 6f5f 6461 7465 7469 6d65  30').to_datetime
-00010e80: 3634 2829 5d0d 0a20 2020 2020 2020 2020  64()]..         
-00010e90: 2020 2023 2062 726f 6b65 7253 7172 4f66     # brokerSqrOf
-00010ea0: 6674 696d 6520 3d20 7064 2e74 6f5f 6461  ftime = pd.to_da
-00010eb0: 7465 7469 6d65 2866 277b 504b 4461 7465  tetime(f'{PKDate
-00010ec0: 5574 696c 6974 6965 732e 7472 6164 696e  Utilities.tradin
-00010ed0: 6744 6174 6528 292e 7374 7266 7469 6d65  gDate().strftime
-00010ee0: 2866 2225 592d 256d 2d25 6422 297d 2031  (f"%Y-%m-%d")} 1
-00010ef0: 353a 3134 3a30 302b 3035 3a33 3027 292e  5:14:00+05:30').
-00010f00: 746f 5f64 6174 6574 696d 6536 3428 290d  to_datetime64().
-00010f10: 0a20 2020 2020 2020 2065 7863 6570 743a  .        except:
-00010f20: 0d0a 2020 2020 2020 2020 2020 2020 6469  ..            di
-00010f30: 6666 5f64 6620 3d20 6461 7461 5b64 6174  ff_df = data[dat
-00010f40: 612e 696e 6465 7820 3e3d 2020 7064 2e74  a.index >=  pd.t
-00010f50: 6f5f 6461 7465 7469 6d65 2866 277b 504b  o_datetime(f'{PK
-00010f60: 4461 7465 5574 696c 6974 6965 732e 7472  DateUtilities.tr
-00010f70: 6164 696e 6744 6174 6528 292e 7374 7266  adingDate().strf
-00010f80: 7469 6d65 2866 2225 592d 256d 2d25 6422  time(f"%Y-%m-%d"
-00010f90: 297d 2030 393a 7b31 352b 7365 6c66 2e63  )} 09:{15+self.c
-00010fa0: 6f6e 6669 674d 616e 6167 6572 2e6d 6f72  onfigManager.mor
-00010fb0: 6e69 6e67 616e 616c 7973 6973 6361 6e64  ninganalysiscand
-00010fc0: 6c65 6e75 6d62 6572 202b 2032 7d3a 3030  lenumber + 2}:00
-00010fd0: 2b30 353a 3330 272c 2075 7463 3d54 7275  +05:30', utc=Tru
-00010fe0: 6529 5d0d 0a20 2020 2020 2020 2020 2020  e)]..           
-00010ff0: 2023 2062 726f 6b65 7253 7172 4f66 6674   # brokerSqrOfft
-00011000: 696d 6520 3d20 7064 2e74 6f5f 6461 7465  ime = pd.to_date
-00011010: 7469 6d65 2866 277b 504b 4461 7465 5574  time(f'{PKDateUt
-00011020: 696c 6974 6965 732e 7472 6164 696e 6744  ilities.tradingD
-00011030: 6174 6528 292e 7374 7266 7469 6d65 2866  ate().strftime(f
-00011040: 2225 592d 256d 2d25 6422 297d 2031 353a  "%Y-%m-%d")} 15:
-00011050: 3134 3a30 302b 3035 3a33 3027 2c20 7574  14:00+05:30', ut
-00011060: 633d 5472 7565 290d 0a20 2020 2020 2020  c=True)..       
-00011070: 2020 2020 2070 6173 730d 0a20 2020 2020       pass..     
-00011080: 2020 2064 6179 4869 6768 4166 7465 7241     dayHighAfterA
-00011090: 6c65 7274 203d 2064 6966 665f 6466 5b22  lert = diff_df["
-000110a0: 4869 6768 225d 2e6d 6178 2829 0d0a 2020  High"].max()..  
-000110b0: 2020 2020 2020 6869 6768 526f 7720 3d20        highRow = 
-000110c0: 6469 6666 5f64 665b 6469 6666 5f64 665b  diff_df[diff_df[
-000110d0: 2248 6967 6822 5d20 3e3d 2064 6179 4869  "High"] >= dayHi
-000110e0: 6768 4166 7465 7241 6c65 7274 5d0d 0a20  ghAfterAlert].. 
-000110f0: 2020 2020 2020 2069 6620 6869 6768 526f         if highRo
-00011100: 7720 6973 206e 6f74 204e 6f6e 6520 616e  w is not None an
-00011110: 6420 6c65 6e28 6869 6768 526f 7729 203e  d len(highRow) >
-00011120: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
-00011130: 2068 6967 6852 6f77 203d 2068 6967 6852   highRow = highR
-00011140: 6f77 2e74 6169 6c28 3129 0d0a 2020 2020  ow.tail(1)..    
-00011150: 2020 2020 7265 7475 726e 2068 6967 6852      return highR
-00011160: 6f77 2e69 6e64 6578 5b2d 315d 2c20 6869  ow.index[-1], hi
-00011170: 6768 526f 770d 0a0d 0a0d 0a20 2020 2064  ghRow......    d
-00011180: 6566 2066 696e 644d 4143 4443 726f 7373  ef findMACDCross
-00011190: 6f76 6572 2873 656c 662c 2064 662c 2061  over(self, df, a
-000111a0: 6674 6572 5469 6d65 7374 616d 703d 4e6f  fterTimestamp=No
-000111b0: 6e65 2c20 6e74 6843 726f 7373 6f76 6572  ne, nthCrossover
-000111c0: 3d31 2c20 7570 4469 7265 6374 696f 6e3d  =1, upDirection=
-000111d0: 5472 7565 2c20 6d69 6e52 5349 3d36 3029  True, minRSI=60)
-000111e0: 3a0d 0a20 2020 2020 2020 2069 6620 6466  :..        if df
-000111f0: 2069 7320 4e6f 6e65 206f 7220 6c65 6e28   is None or len(
-00011200: 6466 2920 3d3d 2030 3a0d 0a20 2020 2020  df) == 0:..     
-00011210: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-00011220: 6c73 650d 0a20 2020 2020 2020 2064 6174  lse..        dat
-00011230: 6120 3d20 6466 2e63 6f70 7928 290d 0a20  a = df.copy().. 
-00011240: 2020 2020 2020 2064 6174 6120 3d20 6461         data = da
-00011250: 7461 2e66 696c 6c6e 6128 3029 0d0a 2020  ta.fillna(0)..  
-00011260: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
-00011270: 612e 7265 706c 6163 6528 5b6e 702e 696e  a.replace([np.in
-00011280: 662c 202d 6e70 2e69 6e66 5d2c 2030 290d  f, -np.inf], 0).
-00011290: 0a20 2020 2020 2020 2064 6174 612e 6472  .        data.dr
-000112a0: 6f70 6e61 2861 7869 733d 302c 2068 6f77  opna(axis=0, how
-000112b0: 3d22 616c 6c22 2c20 696e 706c 6163 653d  ="all", inplace=
-000112c0: 5472 7565 2920 2320 4d61 7962 6520 7468  True) # Maybe th
-000112d0: 6572 6520 7761 7320 6e6f 2074 7261 6465  ere was no trade
-000112e0: 2064 6f6e 6520 6174 2074 6865 7365 2074   done at these t
-000112f0: 696d 6573 3f0d 0a20 2020 2020 2020 2064  imes?..        d
-00011300: 6174 6120 3d20 6461 7461 5b3a 3a2d 315d  ata = data[::-1]
-00011310: 2020 2320 5265 7665 7273 6520 7468 6520    # Reverse the 
-00011320: 6461 7461 6672 616d 6520 736f 2074 6861  dataframe so tha
-00011330: 7420 6974 7320 7468 6520 6f6c 6465 7374  t its the oldest
-00011340: 2064 6174 6520 6669 7273 740d 0a20 2020   date first..   
-00011350: 2020 2020 206d 6163 644c 696e 652c 206d       macdLine, m
-00011360: 6163 6453 6967 6e61 6c2c 206d 6163 6448  acdSignal, macdH
-00011370: 6973 7420 3d20 706b 7461 6c69 622e 4d41  ist = pktalib.MA
-00011380: 4344 2864 6174 615b 2243 6c6f 7365 225d  CD(data["Close"]
-00011390: 2c20 3132 2c20 3236 2c20 3929 0d0a 2020  , 12, 26, 9)..  
-000113a0: 2020 2020 2020 2320 7273 695f 6466 203d        # rsi_df =
-000113b0: 2070 6b74 616c 6962 2e52 5349 2864 6174   pktalib.RSI(dat
-000113c0: 615b 2243 6c6f 7365 225d 2c20 3134 290d  a["Close"], 14).
-000113d0: 0a20 2020 2020 2020 206c 696e 655f 6466  .        line_df
-000113e0: 203d 2070 642e 4461 7461 4672 616d 6528   = pd.DataFrame(
-000113f0: 6d61 6364 4c69 6e65 290d 0a20 2020 2020  macdLine)..     
-00011400: 2020 2073 6967 6e61 6c5f 6466 203d 2070     signal_df = p
-00011410: 642e 4461 7461 4672 616d 6528 6d61 6364  d.DataFrame(macd
-00011420: 5369 676e 616c 290d 0a20 2020 2020 2020  Signal)..       
-00011430: 2076 6f6c 5f64 6620 3d20 6461 7461 5b22   vol_df = data["
-00011440: 566f 6c75 6d65 225d 0d0a 2020 2020 2020  Volume"]..      
-00011450: 2020 6469 6666 5f64 6620 3d20 7064 2e63    diff_df = pd.c
-00011460: 6f6e 6361 7428 5b6c 696e 655f 6466 2c20  oncat([line_df, 
-00011470: 7369 676e 616c 5f64 662c 2073 6967 6e61  signal_df, signa
-00011480: 6c5f 6466 2d6c 696e 655f 6466 2c76 6f6c  l_df-line_df,vol
-00011490: 5f64 665d 2c20 6178 6973 3d31 290d 0a20  _df], axis=1).. 
-000114a0: 2020 2020 2020 2064 6966 665f 6466 2e63         diff_df.c
-000114b0: 6f6c 756d 6e73 203d 205b 226c 696e 6522  olumns = ["line"
-000114c0: 2c22 7369 676e 616c 222c 2264 6966 6622  ,"signal","diff"
-000114d0: 2c22 766f 6c22 5d0d 0a20 2020 2020 2020  ,"vol"]..       
-000114e0: 2064 6966 665f 6466 203d 2064 6966 665f   diff_df = diff_
-000114f0: 6466 5b64 6966 665f 6466 5b22 766f 6c22  df[diff_df["vol"
-00011500: 5d20 3e20 305d 2023 2057 6527 7265 206e  ] > 0] # We're n
-00011510: 6f74 2067 6f69 6e67 2074 6f20 646f 2061  ot going to do a
-00011520: 6e79 7468 696e 6720 7769 7468 2061 2063  nything with a c
-00011530: 616e 646c 6520 7768 6572 6520 7468 6572  andle where ther
-00011540: 6520 7761 7320 6e6f 2074 7261 6465 2e0d  e was no trade..
-00011550: 0a20 2020 2020 2020 2023 2062 726f 6b65  .        # broke
-00011560: 7253 7172 4f66 6674 696d 6520 3d20 4e6f  rSqrOfftime = No
-00011570: 6e65 0d0a 2020 2020 2020 2020 7472 793a  ne..        try:
-00011580: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-00011590: 4c65 7427 7320 6f6e 6c79 2063 6f6e 7369  Let's only consi
-000115a0: 6465 7220 7468 6f73 6520 6361 6e64 6c65  der those candle
-000115b0: 7320 7468 6174 2061 7265 2061 6674 6572  s that are after
-000115c0: 2074 6865 2061 6c65 7274 2069 7373 7565   the alert issue
-000115d0: 2d74 696d 6520 696e 2074 6865 206d 6f72  -time in the mor
-000115e0: 6e69 6e67 7320 2b20 3220 6361 6e64 6c65  nings + 2 candle
-000115f0: 7320 2866 6f72 2062 7579 2f73 656c 6c29  s (for buy/sell)
-00011600: 0d0a 2020 2020 2020 2020 2020 2020 6469  ..            di
-00011610: 6666 5f64 6620 3d20 6469 6666 5f64 665b  ff_df = diff_df[
-00011620: 6469 6666 5f64 662e 696e 6465 7820 3e3d  diff_df.index >=
-00011630: 2020 7064 2e74 6f5f 6461 7465 7469 6d65    pd.to_datetime
-00011640: 2866 277b 504b 4461 7465 5574 696c 6974  (f'{PKDateUtilit
-00011650: 6965 732e 7472 6164 696e 6744 6174 6528  ies.tradingDate(
-00011660: 292e 7374 7266 7469 6d65 2866 2225 592d  ).strftime(f"%Y-
-00011670: 256d 2d25 6422 297d 2030 393a 7b31 352b  %m-%d")} 09:{15+
-00011680: 7365 6c66 2e63 6f6e 6669 674d 616e 6167  self.configManag
-00011690: 6572 2e6d 6f72 6e69 6e67 616e 616c 7973  er.morninganalys
-000116a0: 6973 6361 6e64 6c65 6e75 6d62 6572 202b  iscandlenumber +
-000116b0: 2032 7d3a 3030 2b30 353a 3330 2729 2e74   2}:00+05:30').t
-000116c0: 6f5f 6461 7465 7469 6d65 3634 2829 5d0d  o_datetime64()].
-000116d0: 0a20 2020 2020 2020 2020 2020 2023 2062  .            # b
-000116e0: 726f 6b65 7253 7172 4f66 6674 696d 6520  rokerSqrOfftime 
-000116f0: 3d20 7064 2e74 6f5f 6461 7465 7469 6d65  = pd.to_datetime
-00011700: 2866 277b 504b 4461 7465 5574 696c 6974  (f'{PKDateUtilit
-00011710: 6965 732e 7472 6164 696e 6744 6174 6528  ies.tradingDate(
-00011720: 292e 7374 7266 7469 6d65 2866 2225 592d  ).strftime(f"%Y-
-00011730: 256d 2d25 6422 297d 2031 353a 3134 3a30  %m-%d")} 15:14:0
-00011740: 302b 3035 3a33 3027 292e 746f 5f64 6174  0+05:30').to_dat
-00011750: 6574 696d 6536 3428 290d 0a20 2020 2020  etime64()..     
-00011760: 2020 2065 7863 6570 743a 0d0a 2020 2020     except:..    
-00011770: 2020 2020 2020 2020 6469 6666 5f64 6620          diff_df 
-00011780: 3d20 6469 6666 5f64 665b 6469 6666 5f64  = diff_df[diff_d
-00011790: 662e 696e 6465 7820 3e3d 2020 7064 2e74  f.index >=  pd.t
-000117a0: 6f5f 6461 7465 7469 6d65 2866 277b 504b  o_datetime(f'{PK
-000117b0: 4461 7465 5574 696c 6974 6965 732e 7472  DateUtilities.tr
-000117c0: 6164 696e 6744 6174 6528 292e 7374 7266  adingDate().strf
-000117d0: 7469 6d65 2866 2225 592d 256d 2d25 6422  time(f"%Y-%m-%d"
-000117e0: 297d 2030 393a 7b31 352b 7365 6c66 2e63  )} 09:{15+self.c
-000117f0: 6f6e 6669 674d 616e 6167 6572 2e6d 6f72  onfigManager.mor
-00011800: 6e69 6e67 616e 616c 7973 6973 6361 6e64  ninganalysiscand
-00011810: 6c65 6e75 6d62 6572 202b 2032 7d3a 3030  lenumber + 2}:00
-00011820: 2b30 353a 3330 272c 2075 7463 3d54 7275  +05:30', utc=Tru
-00011830: 6529 5d0d 0a20 2020 2020 2020 2020 2020  e)]..           
-00011840: 2023 2062 726f 6b65 7253 7172 4f66 6674   # brokerSqrOfft
-00011850: 696d 6520 3d20 7064 2e74 6f5f 6461 7465  ime = pd.to_date
-00011860: 7469 6d65 2866 277b 504b 4461 7465 5574  time(f'{PKDateUt
-00011870: 696c 6974 6965 732e 7472 6164 696e 6744  ilities.tradingD
-00011880: 6174 6528 292e 7374 7266 7469 6d65 2866  ate().strftime(f
-00011890: 2225 592d 256d 2d25 6422 297d 2031 353a  "%Y-%m-%d")} 15:
-000118a0: 3134 3a30 302b 3035 3a33 3027 2c20 7574  14:00+05:30', ut
-000118b0: 633d 5472 7565 290d 0a20 2020 2020 2020  c=True)..       
-000118c0: 2020 2020 2070 6173 730d 0a20 2020 2020       pass..     
-000118d0: 2020 2069 6e64 6578 203d 206c 656e 2864     index = len(d
-000118e0: 6966 665f 6466 290d 0a20 2020 2020 2020  iff_df)..       
-000118f0: 2063 726f 7373 4f76 6572 203d 2030 0d0a   crossOver = 0..
-00011900: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00011910: 2020 2320 4c6f 6f70 2075 6e74 696c 2077    # Loop until w
-00011920: 6527 7665 2066 6f75 6e64 2074 6865 206e  e've found the n
-00011930: 7468 2063 726f 7373 6f76 6572 2066 6f72  th crossover for
-00011940: 204d 4143 4420 6f72 2077 6527 7665 2072   MACD or we've r
-00011950: 6561 6368 6564 2074 6865 206c 6173 7420  eached the last 
-00011960: 706f 696e 7420 696e 2074 696d 650d 0a20  point in time.. 
-00011970: 2020 2020 2020 2077 6869 6c65 2028 6372         while (cr
-00011980: 6f73 734f 7665 7220 3c20 6e74 6843 726f  ossOver < nthCro
-00011990: 7373 6f76 6572 2061 6e64 2069 6e64 6578  ssover and index
-000119a0: 203e 3d30 293a 0d0a 2020 2020 2020 2020   >=0):..        
-000119b0: 2020 2020 6966 2064 6966 665f 6466 5b22      if diff_df["
-000119c0: 6469 6666 225d 5b69 6e64 6578 2d31 5d20  diff"][index-1] 
-000119d0: 3c20 303a 2023 2053 6967 6e61 6c20 6c69  < 0: # Signal li
-000119e0: 6e65 2068 6173 206e 6f74 2063 726f 7373  ne has not cross
-000119f0: 6564 2079 6574 2061 6e64 2069 7320 6265  ed yet and is be
-00011a00: 6c6f 7720 7468 6520 7a65 726f 206c 696e  low the zero lin
-00011a10: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
-00011a20: 2020 2077 6869 6c65 2828 6469 6666 5f64     while((diff_d
-00011a30: 665b 2264 6966 6622 5d5b 696e 6465 782d  f["diff"][index-
-00011a40: 315d 203c 2030 2061 6e64 2069 6e64 6578  1] < 0 and index
-00011a50: 203e 3d30 2929 3a20 2320 616e 6420 6469   >=0)): # and di
-00011a60: 6666 5f64 662e 696e 6465 7820 3c3d 2062  ff_df.index <= b
-00011a70: 726f 6b65 7253 7172 4f66 6674 696d 6529  rokerSqrOfftime)
-00011a80: 3a20 2320 6f72 2064 6966 665f 6466 5b22  : # or diff_df["
-00011a90: 7273 6922 5d5b 696e 6465 782d 315d 203c  rsi"][index-1] <
-00011aa0: 3d20 6d69 6e52 5349 293a 0d0a 2020 2020  = minRSI):..    
-00011ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ac0: 2320 4c6f 6f70 2077 6869 6c65 2053 6967  # Loop while Sig
-00011ad0: 6e61 6c20 6c69 6e65 2068 6173 206e 6f74  nal line has not
-00011ae0: 2063 726f 7373 6564 2079 6574 2061 6e64   crossed yet and
-00011af0: 2069 7320 6265 6c6f 7720 7468 6520 7a65   is below the ze
-00011b00: 726f 206c 696e 6520 616e 6420 7765 2776  ro line and we'v
-00011b10: 6520 6e6f 7420 7265 6163 6865 6420 7468  e not reached th
-00011b20: 6520 6c61 7374 2070 6f69 6e74 0d0a 2020  e last point..  
-00011b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b40: 2020 696e 6465 7820 2d3d 2031 0d0a 2020    index -= 1..  
-00011b50: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
-00011b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011b70: 2077 6869 6c65 2828 6469 6666 5f64 665b   while((diff_df[
-00011b80: 2264 6966 6622 5d5b 696e 6465 782d 315d  "diff"][index-1]
-00011b90: 203e 3d20 3020 616e 6420 696e 6465 7820   >= 0 and index 
-00011ba0: 3e3d 3029 293a 2023 2061 6e64 2064 6966  >=0)): # and dif
-00011bb0: 665f 6466 2e69 6e64 6578 203c 3d20 6272  f_df.index <= br
-00011bc0: 6f6b 6572 5371 724f 6666 7469 6d65 293a  okerSqrOfftime):
-00011bd0: 2023 206f 7220 6469 6666 5f64 665b 2272   # or diff_df["r
-00011be0: 7369 225d 5b69 6e64 6578 2d31 5d20 3c3d  si"][index-1] <=
-00011bf0: 206d 696e 5253 4929 3a0d 0a20 2020 2020   minRSI):..     
-00011c00: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00011c10: 204c 6f6f 7020 756e 7469 6c20 7369 676e   Loop until sign
-00011c20: 616c 206c 696e 6520 6861 7320 6e6f 7420  al line has not 
-00011c30: 6372 6f73 7365 6420 7965 7420 616e 6420  crossed yet and 
-00011c40: 6973 2061 626f 7665 2074 6865 207a 6572  is above the zer
-00011c50: 6f20 6c69 6e65 0d0a 2020 2020 2020 2020  o line..        
-00011c60: 2020 2020 2020 2020 2020 2020 696e 6465              inde
-00011c70: 7820 2d3d 2031 0d0a 2020 2020 2020 2020  x -= 1..        
-00011c80: 2020 2020 6372 6f73 734f 7665 7220 2b3d      crossOver +=
-00011c90: 2031 0d0a 2020 2020 2020 2020 7473 203d   1..        ts =
-00011ca0: 2064 6966 665f 6466 2e74 6169 6c28 6c65   diff_df.tail(le
-00011cb0: 6e28 6469 6666 5f64 6629 2d69 6e64 6578  n(diff_df)-index
-00011cc0: 202b 3129 2e68 6561 6428 3129 2e69 6e64   +1).head(1).ind
-00011cd0: 6578 5b2d 315d 0d0a 2020 2020 2020 2020  ex[-1]..        
-00011ce0: 7265 7475 726e 2074 732c 2064 6174 615b  return ts, data[
-00011cf0: 6461 7461 2e69 6e64 6578 203d 3d20 7473  data.index == ts
-00011d00: 5d20 2364 662e 6865 6164 286c 656e 2864  ] #df.head(len(d
-00011d10: 6629 202d 696e 6465 7820 2b31 292e 7461  f) -index +1).ta
-00011d20: 696c 2831 290d 0a20 2020 200d 0a20 2020  il(1)..    ..   
-00011d30: 2023 2046 696e 6420 7374 6f63 6b20 7368   # Find stock sh
-00011d40: 6f77 696e 6720 5253 4920 6372 6f73 7369  owing RSI crossi
-00011d50: 6e67 2077 6974 6820 5253 4920 3920 534d  ng with RSI 9 SM
-00011d60: 410d 0a20 2020 2064 6566 2066 696e 6452  A..    def findR
-00011d70: 5349 4372 6f73 7369 6e67 4d41 2873 656c  SICrossingMA(sel
-00011d80: 662c 2064 662c 2073 6372 6565 6e44 6963  f, df, screenDic
-00011d90: 742c 2073 6176 6544 6963 742c 6c6f 6f6b  t, saveDict,look
-00011da0: 466f 723d 312c 206d 614c 656e 6774 683d  For=1, maLength=
-00011db0: 392c 2072 7369 4b65 793d 2252 5349 2229  9, rsiKey="RSI")
-00011dc0: 3a0d 0a20 2020 2020 2020 2069 6620 6466  :..        if df
-00011dd0: 2069 7320 4e6f 6e65 206f 7220 6c65 6e28   is None or len(
-00011de0: 6466 2920 3d3d 2030 3a0d 0a20 2020 2020  df) == 0:..     
-00011df0: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-00011e00: 6c73 650d 0a20 2020 2020 2020 2069 6620  lse..        if 
-00011e10: 7273 694b 6579 206e 6f74 2069 6e20 6466  rsiKey not in df
-00011e20: 2e63 6f6c 756d 6e73 3a0d 0a20 2020 2020  .columns:..     
-00011e30: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-00011e40: 6c73 650d 0a20 2020 2020 2020 2064 6174  lse..        dat
-00011e50: 6120 3d20 6466 2e63 6f70 7928 290d 0a20  a = df.copy().. 
-00011e60: 2020 2020 2020 2064 6174 6120 3d20 6461         data = da
-00011e70: 7461 5b3a 3a2d 315d 0d0a 2020 2020 2020  ta[::-1]..      
-00011e80: 2020 6d61 5273 6920 3d20 706b 7461 6c69    maRsi = pktali
-00011e90: 622e 4d41 2864 6174 615b 7273 694b 6579  b.MA(data[rsiKey
-00011ea0: 5d2c 2074 696d 6570 6572 696f 643d 6d61  ], timeperiod=ma
-00011eb0: 4c65 6e67 7468 290d 0a20 2020 2020 2020  Length)..       
-00011ec0: 2064 6174 6120 3d20 6461 7461 5b3a 3a2d   data = data[::-
-00011ed0: 315d 2e68 6561 6428 3329 0d0a 2020 2020  1].head(3)..    
-00011ee0: 2020 2020 6d61 5273 6920 3d20 6d61 5273      maRsi = maRs
-00011ef0: 695b 3a3a 2d31 5d2e 6865 6164 2833 290d  i[::-1].head(3).
-00011f00: 0a20 2020 2020 2020 2073 6176 6564 203d  .        saved =
-00011f10: 2073 656c 662e 6669 6e64 4375 7272 656e   self.findCurren
-00011f20: 7453 6176 6564 5661 6c75 6528 7363 7265  tSavedValue(scre
-00011f30: 656e 4469 6374 2c73 6176 6544 6963 742c  enDict,saveDict,
-00011f40: 2254 7265 6e64 2229 0d0a 2020 2020 2020  "Trend")..      
-00011f50: 2020 6966 206c 6f6f 6b46 6f72 2069 6e20    if lookFor in 
-00011f60: 5b31 2c33 5d20 616e 6420 6d61 5273 692e  [1,3] and maRsi.
-00011f70: 696c 6f63 5b30 5d20 3c3d 2064 6174 615b  iloc[0] <= data[
-00011f80: 7273 694b 6579 5d2e 696c 6f63 5b30 5d20  rsiKey].iloc[0] 
-00011f90: 616e 6420 6d61 5273 692e 696c 6f63 5b31  and maRsi.iloc[1
-00011fa0: 5d20 3e20 6461 7461 5b72 7369 4b65 795d  ] > data[rsiKey]
-00011fb0: 2e69 6c6f 635b 315d 3a0d 0a20 2020 2020  .iloc[1]:..     
-00011fc0: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
-00011fd0: 745b 274d 412d 5369 676e 616c 275d 203d  t['MA-Signal'] =
-00011fe0: 2073 6176 6564 5b30 5d20 2b20 636f 6c6f   saved[0] + colo
-00011ff0: 7254 6578 742e 424f 4c44 202b 2063 6f6c  rText.BOLD + col
-00012000: 6f72 5465 7874 2e47 5245 454e 202b 2066  orText.GREEN + f
-00012010: 2752 5349 2d4d 412d 4275 7927 202b 2063  'RSI-MA-Buy' + c
-00012020: 6f6c 6f72 5465 7874 2e45 4e44 0d0a 2020  olorText.END..  
-00012030: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
-00012040: 6374 5b27 4d41 2d53 6967 6e61 6c27 5d20  ct['MA-Signal'] 
-00012050: 3d20 7361 7665 645b 315d 202b 2066 2752  = saved[1] + f'R
-00012060: 5349 2d4d 412d 4275 7927 0d0a 2020 2020  SI-MA-Buy'..    
-00012070: 2020 2020 2020 2020 7265 7475 726e 2054          return T
-00012080: 7275 6520 6966 2028 7273 694b 6579 203d  rue if (rsiKey =
-00012090: 3d20 2252 5349 6922 2920 656c 7365 2028  = "RSIi") else (
-000120a0: 7365 6c66 2e66 696e 6452 5349 4372 6f73  self.findRSICros
-000120b0: 7369 6e67 4d41 2864 662c 2073 6372 6565  singMA(df, scree
-000120c0: 6e44 6963 742c 2073 6176 6544 6963 742c  nDict, saveDict,
-000120d0: 6c6f 6f6b 466f 723d 6c6f 6f6b 466f 722c  lookFor=lookFor,
-000120e0: 206d 614c 656e 6774 683d 6d61 4c65 6e67   maLength=maLeng
-000120f0: 7468 2c20 7273 694b 6579 3d22 5253 4969  th, rsiKey="RSIi
-00012100: 2229 206f 7220 5472 7565 290d 0a20 2020  ") or True)..   
-00012110: 2020 2020 2065 6c69 6620 6c6f 6f6b 466f       elif lookFo
-00012120: 7220 696e 205b 322c 335d 2061 6e64 206d  r in [2,3] and m
-00012130: 6152 7369 2e69 6c6f 635b 305d 203e 3d20  aRsi.iloc[0] >= 
-00012140: 6461 7461 5b72 7369 4b65 795d 2e69 6c6f  data[rsiKey].ilo
-00012150: 635b 305d 2061 6e64 206d 6152 7369 2e69  c[0] and maRsi.i
-00012160: 6c6f 635b 315d 203c 2064 6174 615b 7273  loc[1] < data[rs
-00012170: 694b 6579 5d2e 696c 6f63 5b31 5d3a 0d0a  iKey].iloc[1]:..
-00012180: 2020 2020 2020 2020 2020 2020 7363 7265              scre
-00012190: 656e 4469 6374 5b27 4d41 2d53 6967 6e61  enDict['MA-Signa
-000121a0: 6c27 5d20 3d20 7361 7665 645b 305d 202b  l'] = saved[0] +
-000121b0: 2063 6f6c 6f72 5465 7874 2e42 4f4c 4420   colorText.BOLD 
-000121c0: 2b20 636f 6c6f 7254 6578 742e 4641 494c  + colorText.FAIL
-000121d0: 202b 2066 2752 5349 2d4d 412d 5365 6c6c   + f'RSI-MA-Sell
-000121e0: 2720 2b20 636f 6c6f 7254 6578 742e 454e  ' + colorText.EN
-000121f0: 440d 0a20 2020 2020 2020 2020 2020 2073  D..            s
-00012200: 6176 6544 6963 745b 274d 412d 5369 676e  aveDict['MA-Sign
-00012210: 616c 275d 203d 2073 6176 6564 5b31 5d20  al'] = saved[1] 
-00012220: 2b20 6627 5253 492d 4d41 2d53 656c 6c27  + f'RSI-MA-Sell'
-00012230: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00012240: 7475 726e 2054 7275 6520 6966 2028 7273  turn True if (rs
-00012250: 694b 6579 203d 3d20 2252 5349 6922 2920  iKey == "RSIi") 
-00012260: 656c 7365 2028 7365 6c66 2e66 696e 6452  else (self.findR
-00012270: 5349 4372 6f73 7369 6e67 4d41 2864 662c  SICrossingMA(df,
-00012280: 2073 6372 6565 6e44 6963 742c 2073 6176   screenDict, sav
-00012290: 6544 6963 742c 6c6f 6f6b 466f 723d 6c6f  eDict,lookFor=lo
-000122a0: 6f6b 466f 722c 206d 614c 656e 6774 683d  okFor, maLength=
-000122b0: 6d61 4c65 6e67 7468 2c20 7273 694b 6579  maLength, rsiKey
-000122c0: 3d22 5253 4969 2229 206f 7220 5472 7565  ="RSIi") or True
-000122d0: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-000122e0: 6e20 4661 6c73 6520 6966 2028 7273 694b  n False if (rsiK
-000122f0: 6579 203d 3d20 2252 5349 6922 2920 656c  ey == "RSIi") el
-00012300: 7365 2028 7365 6c66 2e66 696e 6452 5349  se (self.findRSI
-00012310: 4372 6f73 7369 6e67 4d41 2864 662c 2073  CrossingMA(df, s
-00012320: 6372 6565 6e44 6963 742c 2073 6176 6544  creenDict, saveD
-00012330: 6963 742c 6c6f 6f6b 466f 723d 6c6f 6f6b  ict,lookFor=look
-00012340: 466f 722c 206d 614c 656e 6774 683d 6d61  For, maLength=ma
-00012350: 4c65 6e67 7468 2c20 7273 694b 6579 3d22  Length, rsiKey="
-00012360: 5253 4969 2229 290d 0a20 2020 200d 0a20  RSIi"))..    .. 
-00012370: 2020 2023 2046 696e 6420 7374 6f63 6b73     # Find stocks
-00012380: 2077 6974 6820 7269 7369 6e67 2052 5349   with rising RSI
-00012390: 2066 726f 6d20 6c6f 7765 7220 6c65 7665   from lower leve
-000123a0: 6c73 0d0a 2020 2020 6465 6620 6669 6e64  ls..    def find
-000123b0: 5269 7369 6e67 5253 4928 7365 6c66 2c20  RisingRSI(self, 
-000123c0: 6466 2c20 7273 694b 6579 3d22 5253 4922  df, rsiKey="RSI"
-000123d0: 293a 0d0a 2020 2020 2020 2020 6966 2064  ):..        if d
-000123e0: 6620 6973 204e 6f6e 6520 6f72 206c 656e  f is None or len
-000123f0: 2864 6629 203d 3d20 303a 0d0a 2020 2020  (df) == 0:..    
-00012400: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-00012410: 616c 7365 0d0a 2020 2020 2020 2020 6966  alse..        if
-00012420: 2072 7369 4b65 7920 6e6f 7420 696e 2064   rsiKey not in d
-00012430: 662e 636f 6c75 6d6e 733a 0d0a 2020 2020  f.columns:..    
-00012440: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-00012450: 616c 7365 0d0a 2020 2020 2020 2020 6461  alse..        da
-00012460: 7461 203d 2064 662e 636f 7079 2829 0d0a  ta = df.copy()..
-00012470: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
-00012480: 6174 615b 3a3a 2d31 5d0d 0a20 2020 2020  ata[::-1]..     
-00012490: 2020 2064 6174 6120 3d20 6461 7461 2e74     data = data.t
-000124a0: 6169 6c28 3329 0d0a 2020 2020 2020 2020  ail(3)..        
-000124b0: 6966 206c 656e 2864 6174 6129 203c 2033  if len(data) < 3
-000124c0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-000124d0: 6574 7572 6e20 4661 6c73 650d 0a20 2020  eturn False..   
-000124e0: 2020 2020 2064 6179 4d69 6e75 7332 5253       dayMinus2RS
-000124f0: 4920 3d20 6461 7461 5b22 5253 4922 5d2e  I = data["RSI"].
-00012500: 696c 6f63 5b30 5d0d 0a20 2020 2020 2020  iloc[0]..       
-00012510: 2064 6179 4d69 6e75 7331 5253 4920 3d20   dayMinus1RSI = 
-00012520: 6461 7461 5b22 5253 4922 5d2e 696c 6f63  data["RSI"].iloc
-00012530: 5b31 5d0d 0a20 2020 2020 2020 2064 6179  [1]..        day
-00012540: 5253 4920 3d20 6461 7461 5b22 5253 4922  RSI = data["RSI"
-00012550: 5d2e 696c 6f63 5b32 5d0d 0a20 2020 2020  ].iloc[2]..     
-00012560: 2020 2072 6574 7572 6e56 616c 7565 203d     returnValue =
-00012570: 2028 6461 794d 696e 7573 3252 5349 203c   (dayMinus2RSI <
-00012580: 3d20 3335 2061 6e64 2064 6179 4d69 6e75  = 35 and dayMinu
-00012590: 7331 5253 4920 3e20 6461 794d 696e 7573  s1RSI > dayMinus
-000125a0: 3252 5349 2061 6e64 2064 6179 5253 4920  2RSI and dayRSI 
-000125b0: 3e20 6461 794d 696e 7573 3152 5349 2920  > dayMinus1RSI) 
-000125c0: 6f72 205c 0d0a 2020 2020 2020 2020 2020  or \..          
-000125d0: 2020 2020 2020 2864 6179 4d69 6e75 7331        (dayMinus1
-000125e0: 5253 4920 3c3d 2033 3520 616e 6420 6461  RSI <= 35 and da
-000125f0: 7952 5349 203e 2064 6179 4d69 6e75 7331  yRSI > dayMinus1
-00012600: 5253 4929 0d0a 2020 2020 2020 2020 6966  RSI)..        if
-00012610: 2072 7369 4b65 7920 3d3d 2022 5253 4922   rsiKey == "RSI"
-00012620: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-00012630: 6574 7572 6e56 616c 7565 203d 2073 656c  eturnValue = sel
-00012640: 662e 6669 6e64 5269 7369 6e67 5253 4928  f.findRisingRSI(
-00012650: 6466 2c20 7273 694b 6579 3d22 5253 4969  df, rsiKey="RSIi
-00012660: 2229 206f 7220 7265 7475 726e 5661 6c75  ") or returnValu
-00012670: 650d 0a20 2020 2020 2020 2072 6574 7572  e..        retur
-00012680: 6e20 7265 7475 726e 5661 6c75 650d 0a0d  n returnValue...
-00012690: 0a20 2020 2023 406d 6561 7375 7265 5f74  .    #@measure_t
-000126a0: 696d 650d 0a20 2020 2023 2046 696e 6420  ime..    # Find 
-000126b0: 6f75 7420 7472 656e 6420 666f 7220 6461  out trend for da
-000126c0: 7973 2074 6f20 6c6f 6f6b 6261 636b 0d0a  ys to lookback..
-000126d0: 2020 2020 6465 6620 6669 6e64 5472 656e      def findTren
-000126e0: 6428 7365 6c66 2c20 6466 2c20 7363 7265  d(self, df, scre
-000126f0: 656e 4469 6374 2c20 7361 7665 4469 6374  enDict, saveDict
-00012700: 2c20 6461 7973 546f 4c6f 6f6b 6261 636b  , daysToLookback
-00012710: 3d4e 6f6e 652c 2073 746f 636b 4e61 6d65  =None, stockName
-00012720: 3d22 2229 3a0d 0a20 2020 2020 2020 2069  =""):..        i
-00012730: 6620 6466 2069 7320 4e6f 6e65 206f 7220  f df is None or 
-00012740: 6c65 6e28 6466 2920 3d3d 2030 3a0d 0a20  len(df) == 0:.. 
-00012750: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00012760: 6e20 2255 6e6b 6e6f 776e 220d 0a20 2020  n "Unknown"..   
-00012770: 2020 2020 2064 6174 6120 3d20 6466 2e63       data = df.c
-00012780: 6f70 7928 290d 0a20 2020 2020 2020 2069  opy()..        i
-00012790: 6620 6461 7973 546f 4c6f 6f6b 6261 636b  f daysToLookback
-000127a0: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
-000127b0: 2020 2020 2020 2064 6179 7354 6f4c 6f6f         daysToLoo
-000127c0: 6b62 6163 6b20 3d20 7365 6c66 2e63 6f6e  kback = self.con
-000127d0: 6669 674d 616e 6167 6572 2e64 6179 7354  figManager.daysT
-000127e0: 6f4c 6f6f 6b62 6163 6b0d 0a20 2020 2020  oLookback..     
-000127f0: 2020 2064 6174 6120 3d20 6461 7461 2e68     data = data.h
-00012800: 6561 6428 6461 7973 546f 4c6f 6f6b 6261  ead(daysToLookba
-00012810: 636b 290d 0a20 2020 2020 2020 2064 6174  ck)..        dat
-00012820: 6120 3d20 6461 7461 5b3a 3a2d 315d 0d0a  a = data[::-1]..
-00012830: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
-00012840: 6174 612e 7365 745f 696e 6465 7828 6e70  ata.set_index(np
-00012850: 2e61 7261 6e67 6528 6c65 6e28 6461 7461  .arange(len(data
-00012860: 2929 290d 0a20 2020 2020 2020 2064 6174  )))..        dat
-00012870: 6120 3d20 6461 7461 2e66 696c 6c6e 6128  a = data.fillna(
-00012880: 3029 0d0a 2020 2020 2020 2020 6461 7461  0)..        data
-00012890: 203d 2064 6174 612e 7265 706c 6163 6528   = data.replace(
-000128a0: 5b6e 702e 696e 662c 202d 6e70 2e69 6e66  [np.inf, -np.inf
-000128b0: 5d2c 2030 290d 0a20 2020 2020 2020 2073  ], 0)..        s
-000128c0: 6176 6564 203d 2073 656c 662e 6669 6e64  aved = self.find
-000128d0: 4375 7272 656e 7453 6176 6564 5661 6c75  CurrentSavedValu
-000128e0: 6528 7363 7265 656e 4469 6374 2c73 6176  e(screenDict,sav
-000128f0: 6544 6963 742c 2254 7265 6e64 2229 0d0a  eDict,"Trend")..
-00012900: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
-00012910: 2020 2020 2020 2020 2020 7769 7468 2053            with S
-00012920: 7570 7072 6573 734f 7574 7075 7428 7375  uppressOutput(su
-00012930: 7070 7265 7373 5f73 7464 6f75 743d 5472  ppress_stdout=Tr
-00012940: 7565 2c20 7375 7070 7265 7373 5f73 7464  ue, suppress_std
-00012950: 6572 723d 5472 7565 293a 0d0a 2020 2020  err=True):..    
-00012960: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00012970: 5b22 746f 7073 225d 203d 2064 6174 615b  ["tops"] = data[
-00012980: 2243 6c6f 7365 225d 2e69 6c6f 635b 0d0a  "Close"].iloc[..
-00012990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000129a0: 2020 2020 6c69 7374 280d 0a20 2020 2020      list(..     
-000129b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000129c0: 2020 2070 6b74 616c 6962 2e61 7267 7265     pktalib.argre
-000129d0: 6c65 7874 7265 6d61 280d 0a20 2020 2020  lextrema(..     
-000129e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000129f0: 2020 2020 2020 206e 702e 6172 7261 7928         np.array(
-00012a00: 6461 7461 5b22 436c 6f73 6522 5d29 2c20  data["Close"]), 
-00012a10: 6e70 2e67 7265 6174 6572 5f65 7175 616c  np.greater_equal
-00012a20: 2c20 6f72 6465 723d 310d 0a20 2020 2020  , order=1..     
-00012a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a40: 2020 2029 5b30 5d0d 0a20 2020 2020 2020     )[0]..       
-00012a50: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
-00012a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a70: 5d0d 0a20 2020 2020 2020 2020 2020 2064  ]..            d
-00012a80: 6174 6120 3d20 6461 7461 2e66 696c 6c6e  ata = data.filln
-00012a90: 6128 3029 0d0a 2020 2020 2020 2020 2020  a(0)..          
-00012aa0: 2020 6461 7461 203d 2064 6174 612e 7265    data = data.re
-00012ab0: 706c 6163 6528 5b6e 702e 696e 662c 202d  place([np.inf, -
-00012ac0: 6e70 2e69 6e66 5d2c 2030 290d 0a0d 0a20  np.inf], 0).... 
-00012ad0: 2020 2020 2020 2020 2020 2074 7279 3a0d             try:.
-00012ae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012af0: 2023 2069 6620 6c65 6e28 6461 7461 2920   # if len(data) 
-00012b00: 3c20 6461 7973 546f 4c6f 6f6b 6261 636b  < daysToLookback
-00012b10: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00012b20: 2020 2023 2020 2020 2073 656c 662e 6465     #     self.de
-00012b30: 6661 756c 745f 6c6f 6767 6572 2e64 6562  fault_logger.deb
-00012b40: 7567 2864 6174 6129 0d0a 2020 2020 2020  ug(data)..      
-00012b50: 2020 2020 2020 2020 2020 2320 2020 2020            #     
-00012b60: 7261 6973 6520 5374 6f63 6b44 6174 614e  raise StockDataN
-00012b70: 6f74 4164 6571 7561 7465 0d0a 2020 2020  otAdequate..    
-00012b80: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00012b90: 203d 2064 6174 612e 7265 706c 6163 6528   = data.replace(
-00012ba0: 6e70 2e69 6e66 2c20 6e70 2e6e 616e 292e  np.inf, np.nan).
-00012bb0: 7265 706c 6163 6528 2d6e 702e 696e 662c  replace(-np.inf,
-00012bc0: 206e 702e 6e61 6e29 2e64 726f 706e 6128   np.nan).dropna(
-00012bd0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00012be0: 2020 2069 6620 6c65 6e28 6461 7461 5b22     if len(data["
-00012bf0: 746f 7073 225d 5b64 6174 612e 746f 7073  tops"][data.tops
-00012c00: 203e 2030 5d29 203e 2031 3a0d 0a20 2020   > 0]) > 1:..   
-00012c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012c20: 2073 6c6f 7065 203d 206e 702e 706f 6c79   slope = np.poly
-00012c30: 6669 7428 0d0a 2020 2020 2020 2020 2020  fit(..          
-00012c40: 2020 2020 2020 2020 2020 2020 2020 6461                da
-00012c50: 7461 2e69 6e64 6578 5b64 6174 612e 746f  ta.index[data.to
-00012c60: 7073 203e 2030 5d2c 2064 6174 615b 2274  ps > 0], data["t
-00012c70: 6f70 7322 5d5b 6461 7461 2e74 6f70 7320  ops"][data.tops 
-00012c80: 3e20 305d 2c20 310d 0a20 2020 2020 2020  > 0], 1..       
-00012c90: 2020 2020 2020 2020 2020 2020 2029 5b30               )[0
-00012ca0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00012cb0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00012cc0: 2020 2020 2020 2020 2020 2020 2020 736c                sl
-00012cd0: 6f70 6520 3d20 300d 0a20 2020 2020 2020  ope = 0..       
-00012ce0: 2020 2020 2065 7863 6570 7420 6e70 2e6c       except np.l
-00012cf0: 696e 616c 672e 4c69 6e41 6c67 4572 726f  inalg.LinAlgErro
-00012d00: 7220 6173 2065 3a20 2320 7072 6167 6d61  r as e: # pragma
-00012d10: 3a20 6e6f 2063 6f76 6572 0d0a 2020 2020  : no cover..    
-00012d20: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00012d30: 2e64 6566 6175 6c74 5f6c 6f67 6765 722e  .default_logger.
-00012d40: 6465 6275 6728 652c 2065 7863 5f69 6e66  debug(e, exc_inf
-00012d50: 6f3d 5472 7565 290d 0a20 2020 2020 2020  o=True)..       
-00012d60: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
-00012d70: 6963 745b 2254 7265 6e64 225d 203d 2028  ict["Trend"] = (
-00012d80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012d90: 2020 2020 2020 7361 7665 645b 305d 202b        saved[0] +
-00012da0: 2063 6f6c 6f72 5465 7874 2e42 4f4c 4420   colorText.BOLD 
-00012db0: 2b20 636f 6c6f 7254 6578 742e 5741 524e  + colorText.WARN
-00012dc0: 202b 2022 556e 6b6e 6f77 6e22 202b 2063   + "Unknown" + c
-00012dd0: 6f6c 6f72 5465 7874 2e45 4e44 0d0a 2020  olorText.END..  
-00012de0: 2020 2020 2020 2020 2020 2020 2020 290d                ).
-00012df0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012e00: 2073 6176 6544 6963 745b 2254 7265 6e64   saveDict["Trend
-00012e10: 225d 203d 2073 6176 6564 5b31 5d20 2b20  "] = saved[1] + 
-00012e20: 2255 6e6b 6e6f 776e 220d 0a20 2020 2020  "Unknown"..     
-00012e30: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00012e40: 6e20 7361 7665 4469 6374 5b22 5472 656e  n saveDict["Tren
-00012e50: 6422 5d0d 0a20 2020 2020 2020 2020 2020  d"]..           
-00012e60: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
-00012e70: 6e20 6173 2065 3a20 2023 2070 7261 676d  n as e:  # pragm
-00012e80: 613a 206e 6f20 636f 7665 720d 0a20 2020  a: no cover..   
-00012e90: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00012ea0: 662e 6465 6661 756c 745f 6c6f 6767 6572  f.default_logger
-00012eb0: 2e64 6562 7567 2865 2c20 6578 635f 696e  .debug(e, exc_in
-00012ec0: 666f 3d54 7275 6529 0d0a 2020 2020 2020  fo=True)..      
-00012ed0: 2020 2020 2020 2020 2020 736c 6f70 652c            slope,
-00012ee0: 205f 203d 2030 2c20 300d 0a20 2020 2020   _ = 0, 0..     
-00012ef0: 2020 2020 2020 2061 6e67 6c65 203d 206e         angle = n
-00012f00: 702e 7261 6432 6465 6728 6e70 2e61 7263  p.rad2deg(np.arc
-00012f10: 7461 6e28 736c 6f70 6529 290d 0a20 2020  tan(slope))..   
-00012f20: 2020 2020 2020 2020 2069 6620 616e 676c           if angl
-00012f30: 6520 3d3d 2030 3a0d 0a20 2020 2020 2020  e == 0:..       
-00012f40: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
-00012f50: 6963 745b 2254 7265 6e64 225d 203d 2028  ict["Trend"] = (
-00012f60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012f70: 2020 2020 2020 7361 7665 645b 305d 202b        saved[0] +
-00012f80: 2063 6f6c 6f72 5465 7874 2e42 4f4c 4420   colorText.BOLD 
-00012f90: 2b20 636f 6c6f 7254 6578 742e 5741 524e  + colorText.WARN
-00012fa0: 202b 2022 556e 6b6e 6f77 6e22 202b 2063   + "Unknown" + c
-00012fb0: 6f6c 6f72 5465 7874 2e45 4e44 0d0a 2020  olorText.END..  
-00012fc0: 2020 2020 2020 2020 2020 2020 2020 290d                ).
-00012fd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012fe0: 2073 6176 6544 6963 745b 2254 7265 6e64   saveDict["Trend
-00012ff0: 225d 203d 2073 6176 6564 5b31 5d20 2b20  "] = saved[1] + 
-00013000: 2255 6e6b 6e6f 776e 220d 0a20 2020 2020  "Unknown"..     
-00013010: 2020 2020 2020 2065 6c69 6620 616e 676c         elif angl
-00013020: 6520 3c3d 2033 3020 616e 6420 616e 676c  e <= 30 and angl
-00013030: 6520 3e3d 202d 3330 3a0d 0a20 2020 2020  e >= -30:..     
-00013040: 2020 2020 2020 2020 2020 2073 6372 6565             scree
-00013050: 6e44 6963 745b 2254 7265 6e64 225d 203d  nDict["Trend"] =
-00013060: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
-00013070: 2020 2020 2020 2020 7361 7665 645b 305d          saved[0]
-00013080: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
-00013090: 4420 2b20 636f 6c6f 7254 6578 742e 5741  D + colorText.WA
-000130a0: 524e 202b 2022 5369 6465 7761 7973 2220  RN + "Sideways" 
-000130b0: 2b20 636f 6c6f 7254 6578 742e 454e 440d  + colorText.END.
-000130c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000130d0: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
-000130e0: 2020 2020 7361 7665 4469 6374 5b22 5472      saveDict["Tr
-000130f0: 656e 6422 5d20 3d20 7361 7665 645b 315d  end"] = saved[1]
-00013100: 202b 2022 5369 6465 7761 7973 220d 0a20   + "Sideways".. 
-00013110: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-00013120: 616e 676c 6520 3e3d 2033 3020 616e 6420  angle >= 30 and 
-00013130: 616e 676c 6520 3c20 3631 3a0d 0a20 2020  angle < 61:..   
-00013140: 2020 2020 2020 2020 2020 2020 2073 6372               scr
-00013150: 6565 6e44 6963 745b 2254 7265 6e64 225d  eenDict["Trend"]
-00013160: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
-00013170: 2020 2020 2020 2020 2020 7361 7665 645b            saved[
-00013180: 305d 202b 2063 6f6c 6f72 5465 7874 2e42  0] + colorText.B
-00013190: 4f4c 4420 2b20 636f 6c6f 7254 6578 742e  OLD + colorText.
-000131a0: 4752 4545 4e20 2b20 2257 6561 6b20 5570  GREEN + "Weak Up
-000131b0: 2220 2b20 636f 6c6f 7254 6578 742e 454e  " + colorText.EN
-000131c0: 440d 0a20 2020 2020 2020 2020 2020 2020  D..             
-000131d0: 2020 2029 0d0a 2020 2020 2020 2020 2020     )..          
-000131e0: 2020 2020 2020 7361 7665 4469 6374 5b22        saveDict["
-000131f0: 5472 656e 6422 5d20 3d20 7361 7665 645b  Trend"] = saved[
-00013200: 315d 202b 2022 5765 616b 2055 7022 0d0a  1] + "Weak Up"..
-00013210: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-00013220: 2061 6e67 6c65 203e 3d20 3630 3a0d 0a20   angle >= 60:.. 
-00013230: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00013240: 6372 6565 6e44 6963 745b 2254 7265 6e64  creenDict["Trend
-00013250: 225d 203d 2028 0d0a 2020 2020 2020 2020  "] = (..        
-00013260: 2020 2020 2020 2020 2020 2020 7361 7665              save
-00013270: 645b 305d 202b 2063 6f6c 6f72 5465 7874  d[0] + colorText
-00013280: 2e42 4f4c 4420 2b20 636f 6c6f 7254 6578  .BOLD + colorTex
-00013290: 742e 4752 4545 4e20 2b20 2253 7472 6f6e  t.GREEN + "Stron
-000132a0: 6720 5570 2220 2b20 636f 6c6f 7254 6578  g Up" + colorTex
-000132b0: 742e 454e 440d 0a20 2020 2020 2020 2020  t.END..         
-000132c0: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-000132d0: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
-000132e0: 6374 5b22 5472 656e 6422 5d20 3d20 7361  ct["Trend"] = sa
-000132f0: 7665 645b 315d 202b 2022 5374 726f 6e67  ved[1] + "Strong
-00013300: 2055 7022 0d0a 2020 2020 2020 2020 2020   Up"..          
-00013310: 2020 656c 6966 2061 6e67 6c65 203c 3d20    elif angle <= 
-00013320: 2d33 3020 616e 6420 616e 676c 6520 3e20  -30 and angle > 
-00013330: 2d36 313a 0d0a 2020 2020 2020 2020 2020  -61:..          
-00013340: 2020 2020 2020 7363 7265 656e 4469 6374        screenDict
-00013350: 5b22 5472 656e 6422 5d20 3d20 280d 0a20  ["Trend"] = (.. 
-00013360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013370: 2020 2073 6176 6564 5b30 5d20 2b20 636f     saved[0] + co
-00013380: 6c6f 7254 6578 742e 424f 4c44 202b 2063  lorText.BOLD + c
-00013390: 6f6c 6f72 5465 7874 2e46 4149 4c20 2b20  olorText.FAIL + 
-000133a0: 2257 6561 6b20 446f 776e 2220 2b20 636f  "Weak Down" + co
-000133b0: 6c6f 7254 6578 742e 454e 440d 0a20 2020  lorText.END..   
-000133c0: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
-000133d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000133e0: 7361 7665 4469 6374 5b22 5472 656e 6422  saveDict["Trend"
-000133f0: 5d20 3d20 7361 7665 645b 315d 202b 2022  ] = saved[1] + "
-00013400: 5765 616b 2044 6f77 6e22 0d0a 2020 2020  Weak Down"..    
-00013410: 2020 2020 2020 2020 656c 6966 2061 6e67          elif ang
-00013420: 6c65 203c 202d 3630 3a0d 0a20 2020 2020  le < -60:..     
-00013430: 2020 2020 2020 2020 2020 2073 6372 6565             scree
-00013440: 6e44 6963 745b 2254 7265 6e64 225d 203d  nDict["Trend"] =
-00013450: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
-00013460: 2020 2020 2020 2020 7361 7665 645b 305d          saved[0]
-00013470: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
-00013480: 4420 2b20 636f 6c6f 7254 6578 742e 4641  D + colorText.FA
-00013490: 494c 202b 2022 5374 726f 6e67 2044 6f77  IL + "Strong Dow
-000134a0: 6e22 202b 2063 6f6c 6f72 5465 7874 2e45  n" + colorText.E
-000134b0: 4e44 0d0a 2020 2020 2020 2020 2020 2020  ND..            
-000134c0: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
-000134d0: 2020 2020 2020 2073 6176 6544 6963 745b         saveDict[
-000134e0: 2254 7265 6e64 225d 203d 2073 6176 6564  "Trend"] = saved
-000134f0: 5b31 5d20 2b20 2253 7472 6f6e 6720 446f  [1] + "Strong Do
-00013500: 776e 220d 0a20 2020 2020 2020 2065 7863  wn"..        exc
-00013510: 6570 7420 6e70 2e6c 696e 616c 672e 4c69  ept np.linalg.Li
-00013520: 6e41 6c67 4572 726f 7220 6173 2065 3a20  nAlgError as e: 
-00013530: 2320 7072 6167 6d61 3a20 6e6f 2063 6f76  # pragma: no cov
-00013540: 6572 0d0a 2020 2020 2020 2020 2020 2020  er..            
-00013550: 7365 6c66 2e64 6566 6175 6c74 5f6c 6f67  self.default_log
-00013560: 6765 722e 6465 6275 6728 652c 2065 7863  ger.debug(e, exc
-00013570: 5f69 6e66 6f3d 5472 7565 290d 0a20 2020  _info=True)..   
-00013580: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
-00013590: 6963 745b 2254 7265 6e64 225d 203d 2028  ict["Trend"] = (
-000135a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000135b0: 2020 7361 7665 645b 305d 202b 2063 6f6c    saved[0] + col
-000135c0: 6f72 5465 7874 2e42 4f4c 4420 2b20 636f  orText.BOLD + co
-000135d0: 6c6f 7254 6578 742e 5741 524e 202b 2022  lorText.WARN + "
-000135e0: 556e 6b6e 6f77 6e22 202b 2063 6f6c 6f72  Unknown" + color
-000135f0: 5465 7874 2e45 4e44 0d0a 2020 2020 2020  Text.END..      
-00013600: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-00013610: 2020 2020 2073 6176 6544 6963 745b 2254       saveDict["T
-00013620: 7265 6e64 225d 203d 2073 6176 6564 5b31  rend"] = saved[1
-00013630: 5d20 2b20 2255 6e6b 6e6f 776e 220d 0a20  ] + "Unknown".. 
-00013640: 2020 2020 2020 2072 6574 7572 6e20 7361         return sa
-00013650: 7665 4469 6374 5b22 5472 656e 6422 5d0d  veDict["Trend"].
-00013660: 0a0d 0a20 2020 2023 2046 696e 6420 7374  ...    # Find st
-00013670: 6f63 6b73 2061 7070 726f 6368 696e 6720  ocks approching 
-00013680: 746f 206c 6f6e 6720 7465 726d 2074 7265  to long term tre
-00013690: 6e64 6c69 6e65 730d 0a20 2020 2064 6566  ndlines..    def
-000136a0: 2066 696e 6454 7265 6e64 6c69 6e65 7328   findTrendlines(
-000136b0: 7365 6c66 2c20 6466 2c20 7363 7265 656e  self, df, screen
-000136c0: 4469 6374 2c20 7361 7665 4469 6374 2c20  Dict, saveDict, 
-000136d0: 7065 7263 656e 7461 6765 3d30 2e30 3529  percentage=0.05)
-000136e0: 3a0d 0a20 2020 2020 2020 2023 2070 6572  :..        # per
-000136f0: 696f 6420 3d20 696e 7428 2222 2e6a 6f69  iod = int("".joi
-00013700: 6e28 6320 666f 7220 6320 696e 2073 656c  n(c for c in sel
-00013710: 662e 636f 6e66 6967 4d61 6e61 6765 722e  f.configManager.
-00013720: 7065 7269 6f64 2069 6620 632e 6973 6469  period if c.isdi
-00013730: 6769 7428 2929 290d 0a20 2020 2020 2020  git()))..       
-00013740: 2023 2069 6620 6c65 6e28 6461 7461 2920   # if len(data) 
-00013750: 3c20 7065 7269 6f64 3a0d 0a20 2020 2020  < period:..     
-00013760: 2020 2023 2020 2020 2072 6574 7572 6e20     #     return 
-00013770: 4661 6c73 650d 0a20 2020 2020 2020 2064  False..        d
-00013780: 6174 6120 3d20 6466 2e63 6f70 7928 290d  ata = df.copy().
-00013790: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
-000137a0: 6461 7461 5b3a 3a2d 315d 0d0a 2020 2020  data[::-1]..    
-000137b0: 2020 2020 6461 7461 5b22 4e75 6d62 6572      data["Number
-000137c0: 225d 203d 206e 702e 6172 616e 6765 286c  "] = np.arange(l
-000137d0: 656e 2864 6174 6129 2920 2b20 310d 0a20  en(data)) + 1.. 
-000137e0: 2020 2020 2020 2064 6174 615f 6c6f 7720         data_low 
-000137f0: 3d20 6461 7461 2e63 6f70 7928 290d 0a20  = data.copy().. 
-00013800: 2020 2020 2020 2070 6f69 6e74 7320 3d20         points = 
-00013810: 3330 0d0a 0d0a 2020 2020 2020 2020 2222  30....        ""
-00013820: 2220 4967 6e6f 7269 6e67 2074 6865 2052  " Ignoring the R
-00013830: 6573 6974 616e 6365 2066 6f72 206c 6f6e  esitance for lon
-00013840: 672d 7465 726d 2070 7572 706f 7365 0d0a  g-term purpose..
-00013850: 2020 2020 2020 2020 7768 696c 6520 6c65          while le
-00013860: 6e28 6461 7461 5f68 6967 6829 203e 2070  n(data_high) > p
-00013870: 6f69 6e74 733a 0d0a 2020 2020 2020 2020  oints:..        
-00013880: 2020 2020 736c 6f70 652c 2069 6e74 6572      slope, inter
-00013890: 6365 7074 2c20 725f 7661 6c75 652c 2070  cept, r_value, p
-000138a0: 5f76 616c 7565 2c20 7374 645f 6572 7220  _value, std_err 
-000138b0: 3d20 6c69 6e72 6567 7265 7373 2878 3d64  = linregress(x=d
-000138c0: 6174 615f 6869 6768 5b27 4e75 6d62 6572  ata_high['Number
-000138d0: 275d 2c20 793d 6461 7461 5f68 6967 685b  '], y=data_high[
-000138e0: 2748 6967 6827 5d29 0d0a 2020 2020 2020  'High'])..      
-000138f0: 2020 2020 2020 6461 7461 5f68 6967 6820        data_high 
-00013900: 3d20 6461 7461 5f68 6967 682e 6c6f 635b  = data_high.loc[
-00013910: 6461 7461 5f68 6967 685b 2748 6967 6827  data_high['High'
-00013920: 5d20 3e20 736c 6f70 6520 2a20 6461 7461  ] > slope * data
-00013930: 5f68 6967 685b 274e 756d 6265 7227 5d20  _high['Number'] 
-00013940: 2b20 696e 7465 7263 6570 745d 0d0a 2020  + intercept]..  
-00013950: 2020 2020 2020 736c 6f70 652c 2069 6e74        slope, int
-00013960: 6572 6365 7074 2c20 725f 7661 6c75 652c  ercept, r_value,
-00013970: 2070 5f76 616c 7565 2c20 7374 645f 6572   p_value, std_er
-00013980: 7220 3d20 6c69 6e72 6567 7265 7373 2878  r = linregress(x
-00013990: 3d64 6174 615f 6869 6768 5b27 4e75 6d62  =data_high['Numb
-000139a0: 6572 275d 2c20 793d 6461 7461 5f68 6967  er'], y=data_hig
-000139b0: 685b 2743 6c6f 7365 275d 290d 0a20 2020  h['Close'])..   
-000139c0: 2020 2020 2064 6174 615b 2752 6573 6973       data['Resis
-000139d0: 7461 6e63 6527 5d20 3d20 736c 6f70 6520  tance'] = slope 
-000139e0: 2a20 6461 7461 5b27 4e75 6d62 6572 275d  * data['Number']
-000139f0: 202b 2069 6e74 6572 6365 7074 0d0a 2020   + intercept..  
-00013a00: 2020 2020 2020 2222 220d 0a0d 0a20 2020        """....   
-00013a10: 2020 2020 2077 6869 6c65 206c 656e 2864       while len(d
-00013a20: 6174 615f 6c6f 7729 203e 2070 6f69 6e74  ata_low) > point
-00013a30: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00013a40: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
-00013a50: 2020 2020 2020 736c 6f70 652c 2069 6e74        slope, int
-00013a60: 6572 6365 7074 2c20 725f 7661 6c75 652c  ercept, r_value,
-00013a70: 2070 5f76 616c 7565 2c20 7374 645f 6572   p_value, std_er
-00013a80: 7220 3d20 6c69 6e72 6567 7265 7373 280d  r = linregress(.
-00013a90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013aa0: 2020 2020 2078 3d64 6174 615f 6c6f 775b       x=data_low[
-00013ab0: 224e 756d 6265 7222 5d2c 2079 3d64 6174  "Number"], y=dat
-00013ac0: 615f 6c6f 775b 224c 6f77 225d 0d0a 2020  a_low["Low"]..  
-00013ad0: 2020 2020 2020 2020 2020 2020 2020 290d                ).
-00013ae0: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
-00013af0: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
-00013b00: 2065 3a20 2023 2070 7261 676d 613a 206e   e:  # pragma: n
-00013b10: 6f20 636f 7665 720d 0a20 2020 2020 2020  o cover..       
-00013b20: 2020 2020 2020 2020 2073 656c 662e 6465           self.de
-00013b30: 6661 756c 745f 6c6f 6767 6572 2e64 6562  fault_logger.deb
-00013b40: 7567 2865 2c20 6578 635f 696e 666f 3d54  ug(e, exc_info=T
-00013b50: 7275 6529 0d0a 2020 2020 2020 2020 2020  rue)..          
-00013b60: 2020 2020 2020 636f 6e74 696e 7565 0d0a        continue..
-00013b70: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00013b80: 5f6c 6f77 203d 2064 6174 615f 6c6f 772e  _low = data_low.
-00013b90: 6c6f 635b 0d0a 2020 2020 2020 2020 2020  loc[..          
-00013ba0: 2020 2020 2020 6461 7461 5f6c 6f77 5b22        data_low["
-00013bb0: 4c6f 7722 5d20 3c20 736c 6f70 6520 2a20  Low"] < slope * 
-00013bc0: 6461 7461 5f6c 6f77 5b22 4e75 6d62 6572  data_low["Number
-00013bd0: 225d 202b 2069 6e74 6572 6365 7074 0d0a  "] + intercept..
-00013be0: 2020 2020 2020 2020 2020 2020 5d0d 0a0d              ]...
-00013bf0: 0a20 2020 2020 2020 2073 6c6f 7065 2c20  .        slope, 
-00013c00: 696e 7465 7263 6570 742c 2072 5f76 616c  intercept, r_val
-00013c10: 7565 2c20 705f 7661 6c75 652c 2073 7464  ue, p_value, std
-00013c20: 5f65 7272 203d 206c 696e 7265 6772 6573  _err = linregres
-00013c30: 7328 0d0a 2020 2020 2020 2020 2020 2020  s(..            
-00013c40: 783d 6461 7461 5f6c 6f77 5b22 4e75 6d62  x=data_low["Numb
-00013c50: 6572 225d 2c20 793d 6461 7461 5f6c 6f77  er"], y=data_low
-00013c60: 5b22 436c 6f73 6522 5d0d 0a20 2020 2020  ["Close"]..     
-00013c70: 2020 2029 0d0a 2020 2020 2020 2020 6461     )..        da
-00013c80: 7461 5b22 5375 7070 6f72 7422 5d20 3d20  ta["Support"] = 
-00013c90: 736c 6f70 6520 2a20 6461 7461 5b22 4e75  slope * data["Nu
-00013ca0: 6d62 6572 225d 202b 2069 6e74 6572 6365  mber"] + interce
-00013cb0: 7074 0d0a 2020 2020 2020 2020 6e6f 7720  pt..        now 
-00013cc0: 3d20 6461 7461 2e74 6169 6c28 3129 0d0a  = data.tail(1)..
-00013cd0: 0d0a 2020 2020 2020 2020 6c69 6d69 745f  ..        limit_
-00013ce0: 7570 7065 7220 3d20 6e6f 775b 2253 7570  upper = now["Sup
-00013cf0: 706f 7274 225d 2e69 6c6f 635b 305d 202b  port"].iloc[0] +
-00013d00: 2028 6e6f 775b 2253 7570 706f 7274 225d   (now["Support"]
-00013d10: 2e69 6c6f 635b 305d 202a 2070 6572 6365  .iloc[0] * perce
-00013d20: 6e74 6167 6529 0d0a 2020 2020 2020 2020  ntage)..        
-00013d30: 6c69 6d69 745f 6c6f 7765 7220 3d20 6e6f  limit_lower = no
-00013d40: 775b 2253 7570 706f 7274 225d 2e69 6c6f  w["Support"].ilo
-00013d50: 635b 305d 202d 2028 6e6f 775b 2253 7570  c[0] - (now["Sup
-00013d60: 706f 7274 225d 2e69 6c6f 635b 305d 202a  port"].iloc[0] *
-00013d70: 2070 6572 6365 6e74 6167 6529 0d0a 2020   percentage)..  
-00013d80: 2020 2020 2020 7361 7665 6420 3d20 7365        saved = se
-00013d90: 6c66 2e66 696e 6443 7572 7265 6e74 5361  lf.findCurrentSa
-00013da0: 7665 6456 616c 7565 2873 6372 6565 6e44  vedValue(screenD
-00013db0: 6963 742c 2073 6176 6544 6963 742c 2022  ict, saveDict, "
-00013dc0: 5061 7474 6572 6e22 290d 0a20 2020 2020  Pattern")..     
-00013dd0: 2020 2069 6620 6c69 6d69 745f 6c6f 7765     if limit_lowe
-00013de0: 7220 3c20 6e6f 775b 2243 6c6f 7365 225d  r < now["Close"]
-00013df0: 2e69 6c6f 635b 305d 203c 206c 696d 6974  .iloc[0] < limit
-00013e00: 5f75 7070 6572 2061 6e64 2073 6c6f 7065  _upper and slope
-00013e10: 203e 2030 2e31 353a 0d0a 2020 2020 2020   > 0.15:..      
-00013e20: 2020 2020 2020 7363 7265 656e 4469 6374        screenDict
-00013e30: 5b22 5061 7474 6572 6e22 5d20 3d20 280d  ["Pattern"] = (.
-00013e40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013e50: 2073 6176 6564 5b30 5d20 2b20 636f 6c6f   saved[0] + colo
-00013e60: 7254 6578 742e 424f 4c44 202b 2063 6f6c  rText.BOLD + col
-00013e70: 6f72 5465 7874 2e47 5245 454e 202b 2022  orText.GREEN + "
-00013e80: 5472 656e 646c 696e 652d 5375 7070 6f72  Trendline-Suppor
-00013e90: 7422 202b 2063 6f6c 6f72 5465 7874 2e45  t" + colorText.E
-00013ea0: 4e44 0d0a 2020 2020 2020 2020 2020 2020  ND..            
-00013eb0: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
-00013ec0: 6176 6544 6963 745b 2250 6174 7465 726e  aveDict["Pattern
-00013ed0: 225d 203d 2073 6176 6564 5b31 5d20 2b20  "] = saved[1] + 
-00013ee0: 2254 7265 6e64 6c69 6e65 2d53 7570 706f  "Trendline-Suppo
-00013ef0: 7274 220d 0a20 2020 2020 2020 2020 2020  rt"..           
-00013f00: 2072 6574 7572 6e20 5472 7565 0d0a 0d0a   return True....
-00013f10: 2020 2020 2020 2020 2222 2220 506c 6f74          """ Plot
-00013f20: 7320 666f 7220 6465 6275 6767 696e 670d  s for debugging.
-00013f30: 0a20 2020 2020 2020 2069 6d70 6f72 7420  .        import 
-00013f40: 6d61 7470 6c6f 746c 6962 2e70 7970 6c6f  matplotlib.pyplo
-00013f50: 7420 6173 2070 6c74 0d0a 2020 2020 2020  t as plt..      
-00013f60: 2020 6669 672c 2061 7831 203d 2070 6c74    fig, ax1 = plt
-00013f70: 2e73 7562 706c 6f74 7328 6669 6773 697a  .subplots(figsiz
-00013f80: 653d 2831 352c 3130 2929 0d0a 2020 2020  e=(15,10))..    
-00013f90: 2020 2020 636f 6c6f 7220 3d20 2774 6162      color = 'tab
-00013fa0: 3a67 7265 656e 270d 0a20 2020 2020 2020  :green'..       
-00013fb0: 2078 6461 7465 203d 205b 782e 6461 7465   xdate = [x.date
-00013fc0: 2829 2066 6f72 2078 2069 6e20 6461 7461  () for x in data
-00013fd0: 2e69 6e64 6578 5d0d 0a20 2020 2020 2020  .index]..       
-00013fe0: 2061 7831 2e73 6574 5f78 6c61 6265 6c28   ax1.set_xlabel(
-00013ff0: 2744 6174 6527 2c20 636f 6c6f 723d 636f  'Date', color=co
-00014000: 6c6f 7229 0d0a 2020 2020 2020 2020 6178  lor)..        ax
-00014010: 312e 706c 6f74 2878 6461 7465 2c20 6461  1.plot(xdate, da
-00014020: 7461 2e43 6c6f 7365 2c20 6c61 6265 6c3d  ta.Close, label=
-00014030: 2263 6c6f 7365 222c 2063 6f6c 6f72 3d63  "close", color=c
-00014040: 6f6c 6f72 290d 0a20 2020 2020 2020 2061  olor)..        a
-00014050: 7831 2e74 6963 6b5f 7061 7261 6d73 2861  x1.tick_params(a
-00014060: 7869 733d 2778 272c 206c 6162 656c 636f  xis='x', labelco
-00014070: 6c6f 723d 636f 6c6f 7229 0d0a 0d0a 2020  lor=color)....  
-00014080: 2020 2020 2020 6178 3220 3d20 6178 312e        ax2 = ax1.
-00014090: 7477 696e 7928 2920 2320 6178 3220 616e  twiny() # ax2 an
-000140a0: 6420 6178 3120 7769 6c6c 2068 6176 6520  d ax1 will have 
-000140b0: 636f 6d6d 6f6e 2079 2061 7869 7320 616e  common y axis an
-000140c0: 6420 6469 6666 6572 656e 7420 7820 6178  d different x ax
-000140d0: 6973 2c20 7477 696e 790d 0a20 2020 2020  is, twiny..     
-000140e0: 2020 2061 7832 2e70 6c6f 7428 6461 7461     ax2.plot(data
-000140f0: 2e4e 756d 6265 722c 2064 6174 612e 5265  .Number, data.Re
-00014100: 7369 7374 616e 6365 2c20 6c61 6265 6c3d  sistance, label=
-00014110: 2252 6573 2229 0d0a 2020 2020 2020 2020  "Res")..        
-00014120: 6178 322e 706c 6f74 2864 6174 612e 4e75  ax2.plot(data.Nu
-00014130: 6d62 6572 2c20 6461 7461 2e53 7570 706f  mber, data.Suppo
-00014140: 7274 2c20 6c61 6265 6c3d 2253 7570 2229  rt, label="Sup")
-00014150: 0d0a 0d0a 2020 2020 2020 2020 706c 742e  ....        plt.
-00014160: 6c65 6765 6e64 2829 0d0a 2020 2020 2020  legend()..      
-00014170: 2020 706c 742e 6772 6964 2829 0d0a 2020    plt.grid()..  
-00014180: 2020 2020 2020 706c 742e 7368 6f77 2829        plt.show()
-00014190: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-000141a0: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-000141b0: 6c73 650d 0a0d 0a20 2020 2023 2040 6d65  lse....    # @me
-000141c0: 6173 7572 655f 7469 6d65 0d0a 2020 2020  asure_time..    
-000141d0: 6465 6620 6669 6e64 5570 7472 656e 6428  def findUptrend(
-000141e0: 7365 6c66 2c20 6466 2c20 7363 7265 656e  self, df, screen
-000141f0: 4469 6374 2c20 7361 7665 4469 6374 2c20  Dict, saveDict, 
-00014200: 7465 7374 696e 672c 2073 746f 636b 2c6f  testing, stock,o
-00014210: 6e6c 794d 463d 4661 6c73 652c 686f 7374  nlyMF=False,host
-00014220: 4461 7461 3d4e 6f6e 652c 6578 6368 616e  Data=None,exchan
-00014230: 6765 4e61 6d65 3d22 494e 4449 4122 293a  geName="INDIA"):
-00014240: 0d0a 2020 2020 2020 2020 2320 7368 6f75  ..        # shou
-00014250: 6c64 5072 6f63 6565 6420 3d20 5472 7565  ldProceed = True
-00014260: 0d0a 2020 2020 2020 2020 6973 5570 7472  ..        isUptr
-00014270: 656e 6420 3d20 4661 6c73 650d 0a20 2020  end = False..   
-00014280: 2020 2020 2069 7344 6f77 6e74 7265 6e64       isDowntrend
-00014290: 203d 2046 616c 7365 0d0a 2020 2020 2020   = False..      
-000142a0: 2020 6973 3530 444d 4155 7074 7265 6e64    is50DMAUptrend
-000142b0: 203d 2046 616c 7365 0d0a 2020 2020 2020   = False..      
-000142c0: 2020 6973 3530 444d 4144 6f77 6e74 7265    is50DMADowntre
-000142d0: 6e64 203d 2046 616c 7365 0d0a 2020 2020  nd = False..    
-000142e0: 2020 2020 6465 6369 7369 6f6e 203d 2022      decision = "
-000142f0: 220d 0a20 2020 2020 2020 2064 6d61 3530  "..        dma50
-00014300: 6465 6369 7369 6f6e 203d 2022 220d 0a20  decision = "".. 
-00014310: 2020 2020 2020 2066 6169 7256 616c 7565         fairValue
-00014320: 203d 2030 0d0a 2020 2020 2020 2020 6661   = 0..        fa
-00014330: 6972 5661 6c75 6544 6966 6620 3d20 300d  irValueDiff = 0.
-00014340: 0a20 2020 2020 2020 2023 2069 6620 6466  .        # if df
-00014350: 2069 7320 4e6f 6e65 206f 7220 6c65 6e28   is None or len(
-00014360: 6466 2920 3c20 3232 3020 6f72 2074 6573  df) < 220 or tes
-00014370: 7469 6e67 3a0d 0a20 2020 2020 2020 2023  ting:..        #
-00014380: 2020 2020 2073 686f 756c 6450 726f 6365       shouldProce
-00014390: 6564 203d 2046 616c 7365 0d0a 2020 2020  ed = False..    
-000143a0: 2020 2020 6966 2064 6620 6973 206e 6f74      if df is not
-000143b0: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-000143c0: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
-000143d0: 2020 2020 2020 2020 2020 6461 7461 203d            data =
-000143e0: 2064 662e 636f 7079 2829 0d0a 2020 2020   df.copy()..    
-000143f0: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00014400: 203d 2064 6174 615b 3a3a 2d31 5d0d 0a20   = data[::-1].. 
-00014410: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00014420: 6f64 6179 5f73 6d61 203d 2070 6b74 616c  oday_sma = pktal
-00014430: 6962 2e53 4d41 2864 6174 615b 2243 6c6f  ib.SMA(data["Clo
-00014440: 7365 225d 2c20 7469 6d65 7065 7269 6f64  se"], timeperiod
-00014450: 3d35 3029 0d0a 2020 2020 2020 2020 2020  =50)..          
-00014460: 2020 2020 2020 736d 615f 6d69 6e75 7339        sma_minus9
-00014470: 203d 2070 6b74 616c 6962 2e53 4d41 2864   = pktalib.SMA(d
-00014480: 6174 612e 6865 6164 286c 656e 2864 6174  ata.head(len(dat
-00014490: 6129 2d39 295b 2243 6c6f 7365 225d 2c20  a)-9)["Close"], 
-000144a0: 7469 6d65 7065 7269 6f64 3d35 3029 0d0a  timeperiod=50)..
-000144b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000144c0: 736d 615f 6d69 6e75 7331 3420 3d20 706b  sma_minus14 = pk
-000144d0: 7461 6c69 622e 534d 4128 6461 7461 2e68  talib.SMA(data.h
-000144e0: 6561 6428 6c65 6e28 6461 7461 292d 3134  ead(len(data)-14
-000144f0: 295b 2243 6c6f 7365 225d 2c20 7469 6d65  )["Close"], time
-00014500: 7065 7269 6f64 3d35 3029 0d0a 2020 2020  period=50)..    
-00014510: 2020 2020 2020 2020 2020 2020 736d 615f              sma_
-00014520: 6d69 6e75 7332 3020 3d20 706b 7461 6c69  minus20 = pktali
-00014530: 622e 534d 4128 6461 7461 2e68 6561 6428  b.SMA(data.head(
-00014540: 6c65 6e28 6461 7461 292d 3230 295b 2243  len(data)-20)["C
-00014550: 6c6f 7365 225d 2c20 7469 6d65 7065 7269  lose"], timeperi
-00014560: 6f64 3d35 3029 0d0a 2020 2020 2020 2020  od=50)..        
-00014570: 2020 2020 2020 2020 746f 6461 795f 6c6d          today_lm
-00014580: 6120 3d20 706b 7461 6c69 622e 534d 4128  a = pktalib.SMA(
-00014590: 6461 7461 5b22 436c 6f73 6522 5d2c 2074  data["Close"], t
-000145a0: 696d 6570 6572 696f 643d 3230 3029 0d0a  imeperiod=200)..
-000145b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000145c0: 6c6d 615f 6d69 6e75 7332 3020 3d20 706b  lma_minus20 = pk
-000145d0: 7461 6c69 622e 534d 4128 6461 7461 2e68  talib.SMA(data.h
-000145e0: 6561 6428 6c65 6e28 6461 7461 292d 3230  ead(len(data)-20
-000145f0: 295b 2243 6c6f 7365 225d 2c20 7469 6d65  )["Close"], time
-00014600: 7065 7269 6f64 3d32 3030 290d 0a20 2020  period=200)..   
-00014610: 2020 2020 2020 2020 2020 2020 206c 6d61               lma
-00014620: 5f6d 696e 7573 3830 203d 2070 6b74 616c  _minus80 = pktal
-00014630: 6962 2e53 4d41 2864 6174 612e 6865 6164  ib.SMA(data.head
-00014640: 286c 656e 2864 6174 6129 2d38 3029 5b22  (len(data)-80)["
-00014650: 436c 6f73 6522 5d2c 2074 696d 6570 6572  Close"], timeper
-00014660: 696f 643d 3230 3029 0d0a 2020 2020 2020  iod=200)..      
-00014670: 2020 2020 2020 2020 2020 6c6d 615f 6d69            lma_mi
-00014680: 6e75 7331 3030 203d 2070 6b74 616c 6962  nus100 = pktalib
-00014690: 2e53 4d41 2864 6174 612e 6865 6164 286c  .SMA(data.head(l
-000146a0: 656e 2864 6174 6129 2d31 3030 295b 2243  en(data)-100)["C
-000146b0: 6c6f 7365 225d 2c20 7469 6d65 7065 7269  lose"], timeperi
-000146c0: 6f64 3d32 3030 290d 0a20 2020 2020 2020  od=200)..       
-000146d0: 2020 2020 2020 2020 2074 6f64 6179 5f6c           today_l
-000146e0: 6d61 203d 2074 6f64 6179 5f6c 6d61 2e69  ma = today_lma.i
-000146f0: 6c6f 635b 6c65 6e28 746f 6461 795f 6c6d  loc[len(today_lm
-00014700: 6129 2d31 5d20 6966 2074 6f64 6179 5f6c  a)-1] if today_l
-00014710: 6d61 2069 7320 6e6f 7420 4e6f 6e65 2065  ma is not None e
-00014720: 6c73 6520 300d 0a20 2020 2020 2020 2020  lse 0..         
-00014730: 2020 2020 2020 206c 6d61 5f6d 696e 7573         lma_minus
-00014740: 3230 203d 206c 6d61 5f6d 696e 7573 3230  20 = lma_minus20
-00014750: 2e69 6c6f 635b 6c65 6e28 6c6d 615f 6d69  .iloc[len(lma_mi
-00014760: 6e75 7332 3029 2d31 5d20 6966 206c 6d61  nus20)-1] if lma
-00014770: 5f6d 696e 7573 3230 2069 7320 6e6f 7420  _minus20 is not 
-00014780: 4e6f 6e65 2065 6c73 6520 300d 0a20 2020  None else 0..   
-00014790: 2020 2020 2020 2020 2020 2020 206c 6d61               lma
-000147a0: 5f6d 696e 7573 3830 203d 206c 6d61 5f6d  _minus80 = lma_m
-000147b0: 696e 7573 3830 2e69 6c6f 635b 6c65 6e28  inus80.iloc[len(
-000147c0: 6c6d 615f 6d69 6e75 7338 3029 2d31 5d20  lma_minus80)-1] 
-000147d0: 6966 206c 6d61 5f6d 696e 7573 3830 2069  if lma_minus80 i
-000147e0: 7320 6e6f 7420 4e6f 6e65 2065 6c73 6520  s not None else 
-000147f0: 300d 0a20 2020 2020 2020 2020 2020 2020  0..             
-00014800: 2020 206c 6d61 5f6d 696e 7573 3130 3020     lma_minus100 
-00014810: 3d20 6c6d 615f 6d69 6e75 7331 3030 2e69  = lma_minus100.i
-00014820: 6c6f 635b 6c65 6e28 6c6d 615f 6d69 6e75  loc[len(lma_minu
-00014830: 7331 3030 292d 315d 2069 6620 6c6d 615f  s100)-1] if lma_
-00014840: 6d69 6e75 7331 3030 2069 7320 6e6f 7420  minus100 is not 
-00014850: 4e6f 6e65 2065 6c73 6520 300d 0a20 2020  None else 0..   
-00014860: 2020 2020 2020 2020 2020 2020 2074 6f64               tod
-00014870: 6179 5f73 6d61 203d 2074 6f64 6179 5f73  ay_sma = today_s
-00014880: 6d61 2e69 6c6f 635b 6c65 6e28 746f 6461  ma.iloc[len(toda
-00014890: 795f 736d 6129 2d31 5d20 6966 2074 6f64  y_sma)-1] if tod
-000148a0: 6179 5f73 6d61 2069 7320 6e6f 7420 4e6f  ay_sma is not No
-000148b0: 6e65 2065 6c73 6520 300d 0a20 2020 2020  ne else 0..     
-000148c0: 2020 2020 2020 2020 2020 2073 6d61 5f6d             sma_m
-000148d0: 696e 7573 3920 3d20 736d 615f 6d69 6e75  inus9 = sma_minu
-000148e0: 7339 2e69 6c6f 635b 6c65 6e28 736d 615f  s9.iloc[len(sma_
-000148f0: 6d69 6e75 7339 292d 315d 2069 6620 736d  minus9)-1] if sm
-00014900: 615f 6d69 6e75 7339 2069 7320 6e6f 7420  a_minus9 is not 
-00014910: 4e6f 6e65 2065 6c73 6520 300d 0a20 2020  None else 0..   
-00014920: 2020 2020 2020 2020 2020 2020 2073 6d61               sma
-00014930: 5f6d 696e 7573 3134 203d 2073 6d61 5f6d  _minus14 = sma_m
-00014940: 696e 7573 3134 2e69 6c6f 635b 6c65 6e28  inus14.iloc[len(
-00014950: 736d 615f 6d69 6e75 7331 3429 2d31 5d20  sma_minus14)-1] 
-00014960: 6966 2073 6d61 5f6d 696e 7573 3134 2069  if sma_minus14 i
-00014970: 7320 6e6f 7420 4e6f 6e65 2065 6c73 6520  s not None else 
-00014980: 300d 0a20 2020 2020 2020 2020 2020 2020  0..             
-00014990: 2020 2073 6d61 5f6d 696e 7573 3230 203d     sma_minus20 =
-000149a0: 2073 6d61 5f6d 696e 7573 3230 2e69 6c6f   sma_minus20.ilo
-000149b0: 635b 6c65 6e28 736d 615f 6d69 6e75 7332  c[len(sma_minus2
-000149c0: 3029 2d31 5d20 6966 2073 6d61 5f6d 696e  0)-1] if sma_min
-000149d0: 7573 3230 2069 7320 6e6f 7420 4e6f 6e65  us20 is not None
-000149e0: 2065 6c73 6520 300d 0a20 2020 2020 2020   else 0..       
-000149f0: 2020 2020 2020 2020 2069 7355 7074 7265           isUptre
-00014a00: 6e64 203d 2028 746f 6461 795f 6c6d 6120  nd = (today_lma 
-00014a10: 3e20 6c6d 615f 6d69 6e75 7332 3029 206f  > lma_minus20) o
-00014a20: 7220 2874 6f64 6179 5f6c 6d61 203e 206c  r (today_lma > l
-00014a30: 6d61 5f6d 696e 7573 3830 2920 6f72 2028  ma_minus80) or (
-00014a40: 746f 6461 795f 6c6d 6120 3e20 6c6d 615f  today_lma > lma_
-00014a50: 6d69 6e75 7331 3030 290d 0a20 2020 2020  minus100)..     
-00014a60: 2020 2020 2020 2020 2020 2069 7344 6f77             isDow
-00014a70: 6e74 7265 6e64 203d 2028 746f 6461 795f  ntrend = (today_
-00014a80: 6c6d 6120 3c20 6c6d 615f 6d69 6e75 7332  lma < lma_minus2
-00014a90: 3029 2061 6e64 2028 746f 6461 795f 6c6d  0) and (today_lm
-00014aa0: 6120 3c20 6c6d 615f 6d69 6e75 7338 3029  a < lma_minus80)
-00014ab0: 2061 6e64 2028 746f 6461 795f 6c6d 6120   and (today_lma 
-00014ac0: 3c20 6c6d 615f 6d69 6e75 7331 3030 290d  < lma_minus100).
-00014ad0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014ae0: 2069 7335 3044 4d41 5570 7472 656e 6420   is50DMAUptrend 
-00014af0: 3d20 2874 6f64 6179 5f73 6d61 203e 2073  = (today_sma > s
-00014b00: 6d61 5f6d 696e 7573 3929 206f 7220 2874  ma_minus9) or (t
-00014b10: 6f64 6179 5f73 6d61 203e 2073 6d61 5f6d  oday_sma > sma_m
-00014b20: 696e 7573 3134 2920 6f72 2028 746f 6461  inus14) or (toda
-00014b30: 795f 736d 6120 3e20 736d 615f 6d69 6e75  y_sma > sma_minu
-00014b40: 7332 3029 0d0a 2020 2020 2020 2020 2020  s20)..          
-00014b50: 2020 2020 2020 6973 3530 444d 4144 6f77        is50DMADow
-00014b60: 6e74 7265 6e64 203d 2028 746f 6461 795f  ntrend = (today_
-00014b70: 736d 6120 3c20 736d 615f 6d69 6e75 7339  sma < sma_minus9
-00014b80: 2920 616e 6420 2874 6f64 6179 5f73 6d61  ) and (today_sma
-00014b90: 203c 2073 6d61 5f6d 696e 7573 3134 2920   < sma_minus14) 
-00014ba0: 616e 6420 2874 6f64 6179 5f73 6d61 203c  and (today_sma <
-00014bb0: 2073 6d61 5f6d 696e 7573 3230 290d 0a20   sma_minus20).. 
-00014bc0: 2020 2020 2020 2020 2020 2065 7863 6570             excep
-00014bd0: 7420 4578 6365 7074 696f 6e3a 2020 2320  t Exception:  # 
-00014be0: 7072 6167 6d61 3a20 6e6f 2063 6f76 6572  pragma: no cover
-00014bf0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00014c00: 2020 2320 7365 6c66 2e64 6566 6175 6c74    # self.default
-00014c10: 5f6c 6f67 6765 722e 6465 6275 6728 652c  _logger.debug(e,
-00014c20: 2065 7863 5f69 6e66 6f3d 5472 7565 290d   exc_info=True).
-00014c30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014c40: 2070 6173 730d 0a20 2020 2020 2020 2064   pass..        d
-00014c50: 6563 6973 696f 6e20 3d20 2754 3ae2 96b2  ecision = 'T:...
-00014c60: 2720 6966 2069 7355 7074 7265 6e64 2065  ' if isUptrend e
-00014c70: 6c73 6520 2827 543a e296 bc27 2069 6620  lse ('T:...' if 
-00014c80: 6973 446f 776e 7472 656e 6420 656c 7365  isDowntrend else
-00014c90: 2027 2729 0d0a 2020 2020 2020 2020 646d   '')..        dm
-00014ca0: 6135 3064 6563 6973 696f 6e20 3d20 2774  a50decision = 't
-00014cb0: 3ae2 96b2 2720 6966 2069 7335 3044 4d41  :...' if is50DMA
-00014cc0: 5570 7472 656e 6420 656c 7365 2028 2774  Uptrend else ('t
-00014cd0: 3ae2 96bc 2720 6966 2069 7335 3044 4d41  :...' if is50DMA
-00014ce0: 446f 776e 7472 656e 6420 656c 7365 2027  Downtrend else '
-00014cf0: 2729 0d0a 2020 2020 2020 2020 6d66 5f69  ')..        mf_i
-00014d00: 6e73 745f 6f77 6e65 7273 6869 7043 6861  nst_ownershipCha
-00014d10: 6e67 6520 3d20 300d 0a20 2020 2020 2020  nge = 0..       
-00014d20: 2063 6861 6e67 655f 6d69 6c6c 696f 6e73   change_millions
-00014d30: 203d 2222 0d0a 2020 2020 2020 2020 7472   =""..        tr
-00014d40: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
-00014d50: 6d66 5f69 6e73 745f 6f77 6e65 7273 6869  mf_inst_ownershi
-00014d60: 7043 6861 6e67 6520 3d20 7365 6c66 2e67  pChange = self.g
-00014d70: 6574 4d75 7475 616c 4675 6e64 5374 6174  etMutualFundStat
-00014d80: 7573 2873 746f 636b 2c6f 6e6c 794d 463d  us(stock,onlyMF=
-00014d90: 6f6e 6c79 4d46 2c68 6f73 7444 6174 613d  onlyMF,hostData=
-00014da0: 686f 7374 4461 7461 2c66 6f72 6365 3d28  hostData,force=(
-00014db0: 686f 7374 4461 7461 2069 7320 4e6f 6e65  hostData is None
-00014dc0: 206f 7220 686f 7374 4461 7461 2e65 6d70   or hostData.emp
-00014dd0: 7479 206f 7220 6e6f 7420 2822 4d46 2220  ty or not ("MF" 
-00014de0: 696e 2068 6f73 7444 6174 612e 636f 6c75  in hostData.colu
-00014df0: 6d6e 7320 6f72 2022 4649 4922 2069 6e20  mns or "FII" in 
-00014e00: 686f 7374 4461 7461 2e63 6f6c 756d 6e73  hostData.columns
-00014e10: 2929 2c65 7863 6861 6e67 654e 616d 653d  )),exchangeName=
-00014e20: 6578 6368 616e 6765 4e61 6d65 290d 0a20  exchangeName).. 
-00014e30: 2020 2020 2020 2020 2020 2069 6620 6973             if is
-00014e40: 696e 7374 616e 6365 286d 665f 696e 7374  instance(mf_inst
-00014e50: 5f6f 776e 6572 7368 6970 4368 616e 6765  _ownershipChange
-00014e60: 2c20 7064 2e53 6572 6965 7329 3a0d 0a20  , pd.Series):.. 
-00014e70: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00014e80: 665f 696e 7374 5f6f 776e 6572 7368 6970  f_inst_ownership
-00014e90: 4368 616e 6765 203d 2030 0d0a 2020 2020  Change = 0..    
-00014ea0: 2020 2020 2020 2020 726f 756e 644f 6666          roundOff
-00014eb0: 203d 2032 0d0a 2020 2020 2020 2020 2020   = 2..          
-00014ec0: 2020 6d69 6c6c 696f 6e73 203d 2072 6f75    millions = rou
-00014ed0: 6e64 286d 665f 696e 7374 5f6f 776e 6572  nd(mf_inst_owner
-00014ee0: 7368 6970 4368 616e 6765 2f31 3030 3030  shipChange/10000
-00014ef0: 3030 2c72 6f75 6e64 4f66 6629 0d0a 2020  00,roundOff)..  
-00014f00: 2020 2020 2020 2020 2020 7768 696c 6520            while 
-00014f10: 666c 6f61 7428 6d69 6c6c 696f 6e73 2920  float(millions) 
-00014f20: 3d3d 2030 2061 6e64 2072 6f75 6e64 4f66  == 0 and roundOf
-00014f30: 6620 3c3d 353a 0d0a 2020 2020 2020 2020  f <=5:..        
-00014f40: 2020 2020 2020 2020 726f 756e 644f 6666          roundOff
-00014f50: 202b 3d31 0d0a 2020 2020 2020 2020 2020   +=1..          
-00014f60: 2020 2020 2020 6d69 6c6c 696f 6e73 203d        millions =
-00014f70: 2072 6f75 6e64 286d 665f 696e 7374 5f6f   round(mf_inst_o
-00014f80: 776e 6572 7368 6970 4368 616e 6765 2f31  wnershipChange/1
-00014f90: 3030 3030 3030 2c72 6f75 6e64 4f66 6629  000000,roundOff)
-00014fa0: 0d0a 2020 2020 2020 2020 2020 2020 6368  ..            ch
-00014fb0: 616e 6765 5f6d 696c 6c69 6f6e 7320 3d20  ange_millions = 
-00014fc0: 6622 287b 6d69 6c6c 696f 6e73 7d4d 2922  f"({millions}M)"
-00014fd0: 0d0a 2020 2020 2020 2020 6578 6365 7074  ..        except
-00014fe0: 2045 7863 6570 7469 6f6e 2061 7320 653a   Exception as e:
-00014ff0: 2020 2320 7072 6167 6d61 3a20 6e6f 2063    # pragma: no c
-00015000: 6f76 6572 0d0a 2020 2020 2020 2020 2020  over..          
-00015010: 2020 7365 6c66 2e64 6566 6175 6c74 5f6c    self.default_l
-00015020: 6f67 6765 722e 6465 6275 6728 652c 2065  ogger.debug(e, e
-00015030: 7863 5f69 6e66 6f3d 5472 7565 290d 0a20  xc_info=True).. 
-00015040: 2020 2020 2020 2020 2020 2070 6173 730d             pass.
-00015050: 0a20 2020 2020 2020 2074 7279 3a0d 0a20  .        try:.. 
-00015060: 2020 2020 2020 2020 2020 2023 4c65 7427             #Let'
-00015070: 7320 6765 7420 7468 6520 6661 6972 2076  s get the fair v
-00015080: 616c 7565 2c20 6569 7468 6572 2073 6176  alue, either sav
-00015090: 6564 206f 7220 6672 6573 6820 6672 6f6d  ed or fresh from
-000150a0: 2073 6572 7669 6365 0d0a 2020 2020 2020   service..      
-000150b0: 2020 2020 2020 6661 6972 5661 6c75 6520        fairValue 
-000150c0: 3d20 7365 6c66 2e67 6574 4661 6972 5661  = self.getFairVa
-000150d0: 6c75 6528 7374 6f63 6b2c 686f 7374 4461  lue(stock,hostDa
-000150e0: 7461 2c66 6f72 6365 3d28 686f 7374 4461  ta,force=(hostDa
-000150f0: 7461 2069 7320 4e6f 6e65 206f 7220 686f  ta is None or ho
-00015100: 7374 4461 7461 2e65 6d70 7479 206f 7220  stData.empty or 
-00015110: 2246 6169 7256 616c 7565 2220 6e6f 7420  "FairValue" not 
-00015120: 696e 2068 6f73 7444 6174 612e 636f 6c75  in hostData.colu
-00015130: 6d6e 7329 2c65 7863 6861 6e67 654e 616d  mns),exchangeNam
-00015140: 653d 6578 6368 616e 6765 4e61 6d65 290d  e=exchangeName).
-00015150: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00015160: 6661 6972 5661 6c75 6520 6973 206e 6f74  fairValue is not
-00015170: 204e 6f6e 6520 616e 6420 6661 6972 5661   None and fairVa
-00015180: 6c75 6520 213d 2030 3a0d 0a20 2020 2020  lue != 0:..     
-00015190: 2020 2020 2020 2020 2020 206c 7470 203d             ltp =
-000151a0: 2073 6176 6544 6963 745b 224c 5450 225d   saveDict["LTP"]
-000151b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000151c0: 2020 6661 6972 5661 6c75 6544 6966 6620    fairValueDiff 
-000151d0: 3d20 726f 756e 6428 6661 6972 5661 6c75  = round(fairValu
-000151e0: 6520 2d20 6c74 702c 3029 0d0a 2020 2020  e - ltp,0)..    
-000151f0: 2020 2020 2020 2020 2020 2020 7361 7665              save
-00015200: 4469 6374 5b22 4661 6972 5661 6c75 6522  Dict["FairValue"
-00015210: 5d20 3d20 7374 7228 6661 6972 5661 6c75  ] = str(fairValu
-00015220: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
-00015230: 2020 2020 7361 7665 4469 6374 5b22 4656      saveDict["FV
-00015240: 4469 6666 225d 203d 2066 6169 7256 616c  Diff"] = fairVal
-00015250: 7565 4469 6666 0d0a 2020 2020 2020 2020  ueDiff..        
-00015260: 2020 2020 2020 2020 7363 7265 656e 4469          screenDi
-00015270: 6374 5b22 4656 4469 6666 225d 203d 2066  ct["FVDiff"] = f
-00015280: 6169 7256 616c 7565 4469 6666 0d0a 2020  airValueDiff..  
-00015290: 2020 2020 2020 2020 2020 2020 2020 7363                sc
-000152a0: 7265 656e 4469 6374 5b22 4661 6972 5661  reenDict["FairVa
-000152b0: 6c75 6522 5d20 3d20 2863 6f6c 6f72 5465  lue"] = (colorTe
-000152c0: 7874 2e47 5245 454e 2069 6620 6661 6972  xt.GREEN if fair
-000152d0: 5661 6c75 6520 3e3d 206c 7470 2065 6c73  Value >= ltp els
-000152e0: 6520 636f 6c6f 7254 6578 742e 4641 494c  e colorText.FAIL
-000152f0: 2920 2b20 7361 7665 4469 6374 5b22 4661  ) + saveDict["Fa
-00015300: 6972 5661 6c75 6522 5d20 2b20 636f 6c6f  irValue"] + colo
-00015310: 7254 6578 742e 454e 440d 0a20 2020 2020  rText.END..     
-00015320: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
-00015330: 696f 6e20 6173 2065 3a20 2023 2070 7261  ion as e:  # pra
-00015340: 676d 613a 206e 6f20 636f 7665 720d 0a20  gma: no cover.. 
-00015350: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00015360: 6465 6661 756c 745f 6c6f 6767 6572 2e64  default_logger.d
-00015370: 6562 7567 2865 2c20 6578 635f 696e 666f  ebug(e, exc_info
-00015380: 3d54 7275 6529 0d0a 2020 2020 2020 2020  =True)..        
-00015390: 2020 2020 7061 7373 0d0a 2020 2020 2020      pass..      
-000153a0: 2020 6d66 203d 2022 220d 0a20 2020 2020    mf = ""..     
-000153b0: 2020 206d 6673 203d 2022 220d 0a20 2020     mfs = ""..   
-000153c0: 2020 2020 2069 6620 6d66 5f69 6e73 745f       if mf_inst_
-000153d0: 6f77 6e65 7273 6869 7043 6861 6e67 6520  ownershipChange 
-000153e0: 3e20 303a 0d0a 2020 2020 2020 2020 2020  > 0:..          
-000153f0: 2020 6d66 203d 2066 224d 4649 3ae2 96b2    mf = f"MFI:...
-00015400: 207b 6368 616e 6765 5f6d 696c 6c69 6f6e   {change_million
-00015410: 737d 220d 0a20 2020 2020 2020 2020 2020  s}"..           
-00015420: 206d 6673 203d 2063 6f6c 6f72 5465 7874   mfs = colorText
-00015430: 2e47 5245 454e 202b 206d 6620 2b20 636f  .GREEN + mf + co
-00015440: 6c6f 7254 6578 742e 454e 440d 0a20 2020  lorText.END..   
-00015450: 2020 2020 2065 6c69 6620 6d66 5f69 6e73       elif mf_ins
-00015460: 745f 6f77 6e65 7273 6869 7043 6861 6e67  t_ownershipChang
-00015470: 6520 3c20 303a 0d0a 2020 2020 2020 2020  e < 0:..        
-00015480: 2020 2020 6d66 203d 2066 224d 4649 3ae2      mf = f"MFI:.
-00015490: 96bc 207b 6368 616e 6765 5f6d 696c 6c69  .. {change_milli
-000154a0: 6f6e 737d 220d 0a20 2020 2020 2020 2020  ons}"..         
-000154b0: 2020 206d 6673 203d 2063 6f6c 6f72 5465     mfs = colorTe
-000154c0: 7874 2e46 4149 4c20 2b20 6d66 202b 2063  xt.FAIL + mf + c
-000154d0: 6f6c 6f72 5465 7874 2e45 4e44 0d0a 0d0a  olorText.END....
-000154e0: 2020 2020 2020 2020 7361 7665 6420 3d20          saved = 
-000154f0: 7365 6c66 2e66 696e 6443 7572 7265 6e74  self.findCurrent
-00015500: 5361 7665 6456 616c 7565 2873 6372 6565  SavedValue(scree
-00015510: 6e44 6963 742c 7361 7665 4469 6374 2c22  nDict,saveDict,"
-00015520: 5472 656e 6422 290d 0a20 2020 2020 2020  Trend")..       
-00015530: 2064 6563 6973 696f 6e5f 7363 7220 3d20   decision_scr = 
-00015540: 2863 6f6c 6f72 5465 7874 2e47 5245 454e  (colorText.GREEN
-00015550: 2069 6620 6973 5570 7472 656e 6420 656c   if isUptrend el
-00015560: 7365 2028 636f 6c6f 7254 6578 742e 4641  se (colorText.FA
-00015570: 494c 2069 6620 6973 446f 776e 7472 656e  IL if isDowntren
-00015580: 6420 656c 7365 2063 6f6c 6f72 5465 7874  d else colorText
-00015590: 2e57 4152 4e29 2920 2b20 6622 7b64 6563  .WARN)) + f"{dec
-000155a0: 6973 696f 6e7d 2220 2b20 636f 6c6f 7254  ision}" + colorT
-000155b0: 6578 742e 454e 440d 0a20 2020 2020 2020  ext.END..       
-000155c0: 2064 6d61 3530 6465 6369 7369 6f6e 5f73   dma50decision_s
-000155d0: 6372 203d 2028 636f 6c6f 7254 6578 742e  cr = (colorText.
-000155e0: 4752 4545 4e20 6966 2069 7335 3044 4d41  GREEN if is50DMA
-000155f0: 5570 7472 656e 6420 656c 7365 2028 636f  Uptrend else (co
-00015600: 6c6f 7254 6578 742e 4641 494c 2069 6620  lorText.FAIL if 
-00015610: 6973 3530 444d 4144 6f77 6e74 7265 6e64  is50DMADowntrend
-00015620: 2065 6c73 6520 636f 6c6f 7254 6578 742e   else colorText.
-00015630: 5741 524e 2929 202b 2066 227b 646d 6135  WARN)) + f"{dma5
-00015640: 3064 6563 6973 696f 6e7d 2220 2b20 636f  0decision}" + co
-00015650: 6c6f 7254 6578 742e 454e 440d 0a20 2020  lorText.END..   
-00015660: 2020 2020 2073 6176 6544 6963 745b 2254       saveDict["T
-00015670: 7265 6e64 225d 203d 2066 227b 7361 7665  rend"] = f"{save
-00015680: 645b 315d 7d20 7b64 6563 6973 696f 6e7d  d[1]} {decision}
-00015690: 207b 646d 6135 3064 6563 6973 696f 6e7d   {dma50decision}
-000156a0: 207b 6d66 7d22 0d0a 2020 2020 2020 2020   {mf}"..        
-000156b0: 7363 7265 656e 4469 6374 5b22 5472 656e  screenDict["Tren
-000156c0: 6422 5d20 3d20 6622 7b73 6176 6564 5b30  d"] = f"{saved[0
-000156d0: 5d7d 207b 6465 6369 7369 6f6e 5f73 6372  ]} {decision_scr
-000156e0: 7d20 7b64 6d61 3530 6465 6369 7369 6f6e  } {dma50decision
-000156f0: 5f73 6372 7d20 7b6d 6673 7d22 0d0a 2020  _scr} {mfs}"..  
-00015700: 2020 2020 2020 7361 7665 4469 6374 5b22        saveDict["
-00015710: 4d46 4922 5d20 3d20 6d66 5f69 6e73 745f  MFI"] = mf_inst_
-00015720: 6f77 6e65 7273 6869 7043 6861 6e67 650d  ownershipChange.
-00015730: 0a20 2020 2020 2020 2073 6372 6565 6e44  .        screenD
-00015740: 6963 745b 224d 4649 225d 203d 206d 665f  ict["MFI"] = mf_
-00015750: 696e 7374 5f6f 776e 6572 7368 6970 4368  inst_ownershipCh
-00015760: 616e 6765 0d0a 2020 2020 2020 2020 7265  ange..        re
-00015770: 7475 726e 2069 7355 7074 7265 6e64 2c20  turn isUptrend, 
-00015780: 6d66 5f69 6e73 745f 6f77 6e65 7273 6869  mf_inst_ownershi
-00015790: 7043 6861 6e67 652c 2066 6169 7256 616c  pChange, fairVal
-000157a0: 7565 4469 6666 0d0a 2020 2020 0d0a 2020  ueDiff..    ..  
-000157b0: 2020 2320 5072 6976 6174 6520 6d65 7468    # Private meth
-000157c0: 6f64 2074 6f20 6669 6e64 2063 616e 646c  od to find candl
-000157d0: 6520 7479 7065 0d0a 2020 2020 2320 5472  e type..    # Tr
-000157e0: 7565 203d 2042 756c 6c69 7368 2c20 4661  ue = Bullish, Fa
-000157f0: 6c73 6520 3d20 4265 6172 6973 680d 0a20  lse = Bearish.. 
-00015800: 2020 2064 6566 2067 6574 4361 6e64 6c65     def getCandle
-00015810: 5479 7065 2873 656c 662c 2064 6169 6c79  Type(self, daily
-00015820: 4461 7461 293a 0d0a 2020 2020 2020 2020  Data):..        
-00015830: 7265 7475 726e 2062 6f6f 6c28 6461 696c  return bool(dail
-00015840: 7944 6174 615b 2243 6c6f 7365 225d 2e69  yData["Close"].i
-00015850: 6c6f 635b 305d 203e 3d20 6461 696c 7944  loc[0] >= dailyD
-00015860: 6174 615b 224f 7065 6e22 5d2e 696c 6f63  ata["Open"].iloc
-00015870: 5b30 5d29 0d0a 0d0a 2020 2020 6465 6620  [0])....    def 
-00015880: 6765 7443 616e 646c 6542 6f64 7948 6569  getCandleBodyHei
-00015890: 6768 7428 7365 6c66 2c20 6461 696c 7944  ght(self, dailyD
-000158a0: 6174 6129 3a0d 0a20 2020 2020 2020 2062  ata):..        b
-000158b0: 6f64 7948 6569 6768 7420 3d20 6461 696c  odyHeight = dail
-000158c0: 7944 6174 615b 2243 6c6f 7365 225d 2e69  yData["Close"].i
-000158d0: 6c6f 635b 305d 202d 2064 6169 6c79 4461  loc[0] - dailyDa
-000158e0: 7461 5b22 4f70 656e 225d 2e69 6c6f 635b  ta["Open"].iloc[
-000158f0: 305d 0d0a 2020 2020 2020 2020 7265 7475  0]..        retu
-00015900: 726e 2062 6f64 7948 6569 6768 740d 0a0d  rn bodyHeight...
-00015910: 0a20 2020 2064 6566 2067 6574 4661 6972  .    def getFair
-00015920: 5661 6c75 6528 7365 6c66 2c20 7374 6f63  Value(self, stoc
-00015930: 6b2c 2068 6f73 7444 6174 613d 4e6f 6e65  k, hostData=None
-00015940: 2c20 666f 7263 653d 4661 6c73 652c 6578  , force=False,ex
-00015950: 6368 616e 6765 4e61 6d65 3d22 494e 4449  changeName="INDI
-00015960: 4122 293a 0d0a 2020 2020 2020 2020 6966  A"):..        if
-00015970: 2068 6f73 7444 6174 6120 6973 204e 6f6e   hostData is Non
-00015980: 6520 6f72 206c 656e 2868 6f73 7444 6174  e or len(hostDat
-00015990: 6129 203c 2031 3a0d 0a20 2020 2020 2020  a) < 1:..       
-000159a0: 2020 2020 2068 6f73 7444 6174 6120 3d20       hostData = 
-000159b0: 7064 2e44 6174 6146 7261 6d65 2829 0d0a  pd.DataFrame()..
-000159c0: 2020 2020 2020 2020 2320 4c65 7427 7320          # Let's 
-000159d0: 6c6f 6f6b 2066 6f72 2066 6169 7220 7661  look for fair va
-000159e0: 6c75 6573 0d0a 2020 2020 2020 2020 6661  lues..        fa
-000159f0: 6972 5661 6c75 6520 3d20 300d 0a20 2020  irValue = 0..   
-00015a00: 2020 2020 2069 6620 2246 6169 7256 616c       if "FairVal
-00015a10: 7565 2220 696e 2068 6f73 7444 6174 612e  ue" in hostData.
-00015a20: 636f 6c75 6d6e 7320 616e 6420 504b 4461  columns and PKDa
-00015a30: 7465 5574 696c 6974 6965 732e 6375 7272  teUtilities.curr
-00015a40: 656e 7444 6174 6554 696d 6528 292e 7765  entDateTime().we
-00015a50: 656b 6461 7928 2920 3c3d 2034 3a0d 0a20  ekday() <= 4:.. 
-00015a60: 2020 2020 2020 2020 2020 2074 7279 3a0d             try:.
-00015a70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015a80: 2066 6169 7256 616c 7565 203d 2068 6f73   fairValue = hos
-00015a90: 7444 6174 612e 6c6f 635b 686f 7374 4461  tData.loc[hostDa
-00015aa0: 7461 2e69 6e64 6578 5b2d 315d 2c22 4661  ta.index[-1],"Fa
-00015ab0: 6972 5661 6c75 6522 5d0d 0a20 2020 2020  irValue"]..     
-00015ac0: 2020 2020 2020 2065 7863 6570 7420 284b         except (K
-00015ad0: 6579 4572 726f 722c 496e 6465 7845 7272  eyError,IndexErr
-00015ae0: 6f72 293a 0d0a 2020 2020 2020 2020 2020  or):..          
-00015af0: 2020 2020 2020 2020 2020 7061 7373 0d0a            pass..
-00015b00: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-00015b10: 2020 2020 2020 2020 2020 2069 6620 504b             if PK
-00015b20: 4461 7465 5574 696c 6974 6965 732e 6375  DateUtilities.cu
-00015b30: 7272 656e 7444 6174 6554 696d 6528 292e  rrentDateTime().
-00015b40: 7765 656b 6461 7928 2920 3e3d 2035 206f  weekday() >= 5 o
-00015b50: 7220 666f 7263 653a 0d0a 2020 2020 2020  r force:..      
-00015b60: 2020 2020 2020 2020 2020 7365 6375 7269            securi
-00015b70: 7479 203d 204e 6f6e 650d 0a20 2020 2020  ty = None..     
-00015b80: 2020 2020 2020 2020 2020 2023 2052 6566             # Ref
-00015b90: 7265 7368 2065 6163 6820 7361 7475 7264  resh each saturd
-00015ba0: 6179 206f 7220 7375 6e64 6179 206f 7220  ay or sunday or 
-00015bb0: 7768 656e 206e 6f74 2066 6f75 6e64 2069  when not found i
-00015bc0: 6e20 7361 7665 6420 6461 7461 0d0a 2020  n saved data..  
-00015bd0: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-00015be0: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
-00015bf0: 2020 2020 2020 2020 7769 7468 2053 7570          with Sup
-00015c00: 7072 6573 734f 7574 7075 7428 7375 7070  pressOutput(supp
-00015c10: 7265 7373 5f73 7464 6572 723d 5472 7565  ress_stderr=True
-00015c20: 2c20 7375 7070 7265 7373 5f73 7464 6f75  , suppress_stdou
-00015c30: 743d 5472 7565 293a 0d0a 2020 2020 2020  t=True):..      
-00015c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015c50: 2020 7365 6375 7269 7479 203d 2053 746f    security = Sto
-00015c60: 636b 2873 746f 636b 2c65 7863 6861 6e67  ck(stock,exchang
-00015c70: 653d 6578 6368 616e 6765 4e61 6d65 290d  e=exchangeName).
-00015c80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015c90: 2065 7863 6570 7420 5661 6c75 6545 7272   except ValueErr
-00015ca0: 6f72 3a20 2320 7072 6167 6d61 3a20 6e6f  or: # pragma: no
-00015cb0: 2063 6f76 6572 0d0a 2020 2020 2020 2020   cover..        
-00015cc0: 2020 2020 2020 2020 2020 2020 2320 5765              # We
-00015cd0: 2064 6964 206e 6f74 2066 696e 6420 7468   did not find th
-00015ce0: 6520 7374 6f63 6b3f 2049 7427 7320 6f6b  e stock? It's ok
-00015cf0: 6179 2e20 4d6f 7665 206f 6e20 746f 2074  ay. Move on to t
-00015d00: 6865 206e 6578 7420 6f6e 652e 0d0a 2020  he next one...  
-00015d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015d20: 2020 7061 7373 0d0a 2020 2020 2020 2020    pass..        
-00015d30: 2020 2020 2020 2020 6966 2073 6563 7572          if secur
-00015d40: 6974 7920 6973 206e 6f74 204e 6f6e 653a  ity is not None:
-00015d50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00015d60: 2020 2020 2020 7769 7468 2053 7570 7072        with Suppr
-00015d70: 6573 734f 7574 7075 7428 7375 7070 7265  essOutput(suppre
-00015d80: 7373 5f73 7464 6572 723d 5472 7565 2c20  ss_stderr=True, 
-00015d90: 7375 7070 7265 7373 5f73 7464 6f75 743d  suppress_stdout=
-00015da0: 5472 7565 293a 0d0a 2020 2020 2020 2020  True):..        
-00015db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015dc0: 6676 203d 2073 6563 7572 6974 792e 6661  fv = security.fa
-00015dd0: 6972 5661 6c75 6528 290d 0a20 2020 2020  irValue()..     
-00015de0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00015df0: 6620 6676 2069 7320 6e6f 7420 4e6f 6e65  f fv is not None
-00015e00: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00015e10: 2020 2020 2020 2020 2020 2074 7279 3a0d             try:.
-00015e20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015e30: 2020 2020 2020 2020 2020 2020 2066 7652               fvR
-00015e40: 6573 706f 6e73 6556 616c 7565 203d 2066  esponseValue = f
-00015e50: 765b 226c 6174 6573 7446 6169 7256 616c  v["latestFairVal
-00015e60: 7565 225d 0d0a 2020 2020 2020 2020 2020  ue"]..          
-00015e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015e80: 2020 6966 2066 7652 6573 706f 6e73 6556    if fvResponseV
-00015e90: 616c 7565 2069 7320 6e6f 7420 4e6f 6e65  alue is not None
-00015ea0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00015eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015ec0: 2020 2066 6169 7256 616c 7565 203d 2066     fairValue = f
-00015ed0: 6c6f 6174 2866 7652 6573 706f 6e73 6556  loat(fvResponseV
-00015ee0: 616c 7565 290d 0a20 2020 2020 2020 2020  alue)..         
-00015ef0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00015f00: 7863 6570 743a 2023 2070 7261 676d 613a  xcept: # pragma:
-00015f10: 206e 6f20 636f 7665 720d 0a20 2020 2020   no cover..     
-00015f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015f30: 2020 2020 2020 2070 6173 730d 0a20 2020         pass..   
-00015f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015f50: 2020 2020 2020 2020 2023 2073 656c 662e           # self.
-00015f60: 6465 6661 756c 745f 6c6f 6767 6572 2e64  default_logger.d
-00015f70: 6562 7567 2866 227b 657d 5c6e 5265 7370  ebug(f"{e}\nResp
-00015f80: 6f6e 7365 3a66 763a 5c6e 7b66 767d 222c  onse:fv:\n{fv}",
-00015f90: 2065 7863 5f69 6e66 6f3d 5472 7565 290d   exc_info=True).
-00015fa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015fb0: 2020 2020 2066 6169 7256 616c 7565 203d       fairValue =
-00015fc0: 2072 6f75 6e64 2866 6c6f 6174 2866 6169   round(float(fai
-00015fd0: 7256 616c 7565 292c 3129 0d0a 2020 2020  rValue),1)..    
+0000f210: 6520 3d20 5b39 2c20 3130 2c20 3230 2c20  e = [9, 10, 20, 
+0000f220: 3530 2c20 3230 305d 2069 6620 6d61 4c65  50, 200] if maLe
+0000f230: 6e67 7468 2069 7320 4e6f 6e65 2065 6c73  ngth is None els
+0000f240: 6520 5b6d 614c 656e 6774 685d 0d0a 2020  e [maLength]..  
+0000f250: 2020 2020 2020 7265 7375 6c74 7320 3d20        results = 
+0000f260: 5b5d 0d0a 2020 2020 2020 2020 6861 7352  []..        hasR
+0000f270: 6576 6572 7361 6c73 203d 2046 616c 7365  eversals = False
+0000f280: 0d0a 2020 2020 2020 2020 6461 7461 203d  ..        data =
+0000f290: 2064 6174 615b 3a3a 2d31 5d0d 0a20 2020   data[::-1]..   
+0000f2a0: 2020 2020 2073 6176 6564 203d 2073 656c       saved = sel
+0000f2b0: 662e 6669 6e64 4375 7272 656e 7453 6176  f.findCurrentSav
+0000f2c0: 6564 5661 6c75 6528 7363 7265 656e 4469  edValue(screenDi
+0000f2d0: 6374 2c73 6176 6544 6963 742c 2022 4d41  ct,saveDict, "MA
+0000f2e0: 2d53 6967 6e61 6c22 290d 0a20 2020 2020  -Signal")..     
+0000f2f0: 2020 2066 6f72 206d 614c 656e 6774 6820     for maLength 
+0000f300: 696e 206d 6152 616e 6765 3a0d 0a20 2020  in maRange:..   
+0000f310: 2020 2020 2020 2020 2064 6174 6143 6f70           dataCop
+0000f320: 7920 3d20 6461 7461 0d0a 2020 2020 2020  y = data..      
+0000f330: 2020 2020 2020 6966 2073 656c 662e 636f        if self.co
+0000f340: 6e66 6967 4d61 6e61 6765 722e 7573 6545  nfigManager.useE
+0000f350: 4d41 206f 7220 6d61 4c65 6e67 7468 203d  MA or maLength =
+0000f360: 3d20 393a 0d0a 2020 2020 2020 2020 2020  = 9:..          
+0000f370: 2020 2020 2020 6d61 5265 7620 3d20 706b        maRev = pk
+0000f380: 7461 6c69 622e 454d 4128 6461 7461 436f  talib.EMA(dataCo
+0000f390: 7079 5b22 436c 6f73 6522 5d2c 2074 696d  py["Close"], tim
+0000f3a0: 6570 6572 696f 643d 6d61 4c65 6e67 7468  eperiod=maLength
+0000f3b0: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
+0000f3c0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+0000f3d0: 2020 2020 2020 6d61 5265 7620 3d20 706b        maRev = pk
+0000f3e0: 7461 6c69 622e 4d41 2864 6174 6143 6f70  talib.MA(dataCop
+0000f3f0: 795b 2243 6c6f 7365 225d 2c20 7469 6d65  y["Close"], time
+0000f400: 7065 7269 6f64 3d6d 614c 656e 6774 6829  period=maLength)
+0000f410: 0d0a 2020 2020 2020 2020 2020 2020 7472  ..            tr
+0000f420: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
+0000f430: 2020 2020 6461 7461 436f 7079 2e64 726f      dataCopy.dro
+0000f440: 7028 226d 6152 6576 222c 2061 7869 733d  p("maRev", axis=
+0000f450: 312c 2069 6e70 6c61 6365 3d54 7275 652c  1, inplace=True,
+0000f460: 2065 7272 6f72 733d 2269 676e 6f72 6522   errors="ignore"
+0000f470: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
+0000f480: 7863 6570 7420 4578 6365 7074 696f 6e3a  xcept Exception:
+0000f490: 2320 7072 6167 6d61 3a20 6e6f 2063 6f76  # pragma: no cov
+0000f4a0: 6572 0d0a 2020 2020 2020 2020 2020 2020  er..            
+0000f4b0: 2020 2020 7061 7373 0d0a 2020 2020 2020      pass..      
+0000f4c0: 2020 2020 2020 6461 7461 436f 7079 2e69        dataCopy.i
+0000f4d0: 6e73 6572 7428 6c65 6e28 6461 7461 436f  nsert(len(dataCo
+0000f4e0: 7079 2e63 6f6c 756d 6e73 292c 2022 6d61  py.columns), "ma
+0000f4f0: 5265 7622 2c20 6d61 5265 7629 0d0a 2020  Rev", maRev)..  
+0000f500: 2020 2020 2020 2020 2020 6461 7461 436f            dataCo
+0000f510: 7079 203d 2064 6174 6143 6f70 795b 3a3a  py = dataCopy[::
+0000f520: 2d31 5d2e 6865 6164 2834 290d 0a20 2020  -1].head(4)..   
+0000f530: 2020 2020 2020 2020 2062 756c 6c69 7368           bullish
+0000f540: 4d41 5265 7665 7273 616c 203d 2064 6174  MAReversal = dat
+0000f550: 6143 6f70 795b 226d 6152 6576 225d 2e69  aCopy["maRev"].i
+0000f560: 6c6f 635b 305d 203e 3d20 6461 7461 436f  loc[0] >= dataCo
+0000f570: 7079 5b22 6d61 5265 7622 5d2e 696c 6f63  py["maRev"].iloc
+0000f580: 5b31 5d20 616e 6420 5c0d 0a20 2020 2020  [1] and \..     
+0000f590: 2020 2020 2020 2020 2020 2064 6174 6143             dataC
+0000f5a0: 6f70 795b 226d 6152 6576 225d 2e69 6c6f  opy["maRev"].ilo
+0000f5b0: 635b 315d 203e 3d20 6461 7461 436f 7079  c[1] >= dataCopy
+0000f5c0: 5b22 6d61 5265 7622 5d2e 696c 6f63 5b32  ["maRev"].iloc[2
+0000f5d0: 5d20 616e 6420 5c0d 0a20 2020 2020 2020  ] and \..       
+0000f5e0: 2020 2020 2020 2020 2020 2020 2064 6174               dat
+0000f5f0: 6143 6f70 795b 226d 6152 6576 225d 2e69  aCopy["maRev"].i
+0000f600: 6c6f 635b 325d 203c 2064 6174 6143 6f70  loc[2] < dataCop
+0000f610: 795b 226d 6152 6576 225d 2e69 6c6f 635b  y["maRev"].iloc[
+0000f620: 335d 0d0a 2020 2020 2020 2020 2020 2020  3]..            
+0000f630: 6275 6c6c 6973 6843 6c6f 7365 203d 2064  bullishClose = d
+0000f640: 6174 6143 6f70 792e 6865 6164 2831 295b  ataCopy.head(1)[
+0000f650: 2243 6c6f 7365 225d 2e69 6c6f 635b 305d  "Close"].iloc[0]
+0000f660: 203e 3d20 6461 7461 436f 7079 2e68 6561   >= dataCopy.hea
+0000f670: 6428 3129 5b22 6d61 5265 7622 5d2e 696c  d(1)["maRev"].il
+0000f680: 6f63 5b30 5d0d 0a20 2020 2020 2020 2020  oc[0]..         
+0000f690: 2020 2062 6561 7269 7368 4d41 5265 7665     bearishMAReve
+0000f6a0: 7273 616c 203d 2064 6174 6143 6f70 795b  rsal = dataCopy[
+0000f6b0: 226d 6152 6576 225d 2e69 6c6f 635b 305d  "maRev"].iloc[0]
+0000f6c0: 203c 3d20 6461 7461 436f 7079 5b22 6d61   <= dataCopy["ma
+0000f6d0: 5265 7622 5d2e 696c 6f63 5b31 5d20 616e  Rev"].iloc[1] an
+0000f6e0: 6420 5c0d 0a20 2020 2020 2020 2020 2020  d \..           
+0000f6f0: 2020 2020 2064 6174 6143 6f70 795b 226d       dataCopy["m
+0000f700: 6152 6576 225d 2e69 6c6f 635b 315d 203c  aRev"].iloc[1] <
+0000f710: 3d20 6461 7461 436f 7079 5b22 6d61 5265  = dataCopy["maRe
+0000f720: 7622 5d2e 696c 6f63 5b32 5d20 616e 6420  v"].iloc[2] and 
+0000f730: 5c0d 0a20 2020 2020 2020 2020 2020 2020  \..             
+0000f740: 2020 2020 2020 2064 6174 6143 6f70 795b         dataCopy[
+0000f750: 226d 6152 6576 225d 2e69 6c6f 635b 325d  "maRev"].iloc[2]
+0000f760: 203e 2064 6174 6143 6f70 795b 226d 6152   > dataCopy["maR
+0000f770: 6576 225d 2e69 6c6f 635b 335d 0d0a 2020  ev"].iloc[3]..  
+0000f780: 2020 2020 2020 2020 2020 6973 5265 6365            isRece
+0000f790: 6e74 436c 6f73 6557 6974 6869 6e50 6572  ntCloseWithinPer
+0000f7a0: 6365 6e74 5261 6e67 6520 3d20 6461 7461  centRange = data
+0000f7b0: 436f 7079 2e65 7175 616c 7328 6461 7461  Copy.equals(data
+0000f7c0: 436f 7079 5b28 6461 7461 436f 7079 2e43  Copy[(dataCopy.C
+0000f7d0: 6c6f 7365 203e 3d20 2864 6174 6143 6f70  lose >= (dataCop
+0000f7e0: 792e 6d61 5265 7620 2d20 2864 6174 6143  y.maRev - (dataC
+0000f7f0: 6f70 792e 6d61 5265 7620 2a20 7065 7263  opy.maRev * perc
+0000f800: 656e 7461 6765 2929 2920 2620 2864 6174  entage))) & (dat
+0000f810: 6143 6f70 792e 436c 6f73 6520 3c3d 2028  aCopy.Close <= (
+0000f820: 6461 7461 436f 7079 2e6d 6152 6576 202b  dataCopy.maRev +
+0000f830: 2028 6461 7461 436f 7079 2e6d 6152 6576   (dataCopy.maRev
+0000f840: 202a 2070 6572 6365 6e74 6167 6529 2929   * percentage)))
+0000f850: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+0000f860: 6966 2028 6973 5265 6365 6e74 436c 6f73  if (isRecentClos
+0000f870: 6557 6974 6869 6e50 6572 6365 6e74 5261  eWithinPercentRa
+0000f880: 6e67 6520 616e 6420 6275 6c6c 6973 6843  nge and bullishC
+0000f890: 6c6f 7365 2061 6e64 2062 756c 6c69 7368  lose and bullish
+0000f8a0: 4d41 5265 7665 7273 616c 2920 6f72 205c  MAReversal) or \
+0000f8b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000f8c0: 2020 2869 7352 6563 656e 7443 6c6f 7365    (isRecentClose
+0000f8d0: 5769 7468 696e 5065 7263 656e 7452 616e  WithinPercentRan
+0000f8e0: 6765 2061 6e64 206e 6f74 2062 756c 6c69  ge and not bulli
+0000f8f0: 7368 436c 6f73 6520 616e 6420 6265 6172  shClose and bear
+0000f900: 6973 684d 4152 6576 6572 7361 6c29 3a0d  ishMAReversal):.
+0000f910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f920: 2068 6173 5265 7665 7273 616c 7320 3d20   hasReversals = 
+0000f930: 5472 7565 0d0a 2020 2020 2020 2020 2020  True..          
+0000f940: 2020 2020 2020 7265 7375 6c74 732e 6170        results.ap
+0000f950: 7065 6e64 2873 7472 286d 614c 656e 6774  pend(str(maLengt
+0000f960: 6829 290d 0a20 2020 2020 2020 2069 6620  h))..        if 
+0000f970: 6861 7352 6576 6572 7361 6c73 3a0d 0a20  hasReversals:.. 
+0000f980: 2020 2020 2020 2020 2020 2073 6372 6565             scree
+0000f990: 6e44 6963 745b 224d 412d 5369 676e 616c  nDict["MA-Signal
+0000f9a0: 225d 203d 2028 0d0a 2020 2020 2020 2020  "] = (..        
+0000f9b0: 2020 2020 2020 2020 7361 7665 645b 305d          saved[0]
+0000f9c0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0000f9d0: 2020 202b 2063 6f6c 6f72 5465 7874 2e42     + colorText.B
+0000f9e0: 4f4c 440d 0a20 2020 2020 2020 2020 2020  OLD..           
+0000f9f0: 2020 2020 202b 2028 636f 6c6f 7254 6578       + (colorTex
+0000fa00: 742e 4752 4545 4e20 6966 2062 756c 6c69  t.GREEN if bulli
+0000fa10: 7368 4d41 5265 7665 7273 616c 2065 6c73  shMAReversal els
+0000fa20: 6520 2863 6f6c 6f72 5465 7874 2e46 4149  e (colorText.FAI
+0000fa30: 4c20 6966 2062 6561 7269 7368 4d41 5265  L if bearishMARe
+0000fa40: 7665 7273 616c 2065 6c73 6520 636f 6c6f  versal else colo
+0000fa50: 7254 6578 742e 5741 524e 2929 0d0a 2020  rText.WARN))..  
+0000fa60: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+0000fa70: 6622 5265 7665 7273 616c 2d5b 7b27 2c27  f"Reversal-[{','
+0000fa80: 2e6a 6f69 6e28 7265 7375 6c74 7329 7d5d  .join(results)}]
+0000fa90: 7b27 454d 4127 2069 6620 286d 614c 656e  {'EMA' if (maLen
+0000faa0: 6774 6820 3d3d 2039 206f 7220 7365 6c66  gth == 9 or self
+0000fab0: 2e63 6f6e 6669 674d 616e 6167 6572 2e75  .configManager.u
+0000fac0: 7365 454d 4129 2065 6c73 6520 274d 4127  seEMA) else 'MA'
+0000fad0: 7d22 0d0a 2020 2020 2020 2020 2020 2020  }"..            
+0000fae0: 2020 2020 2b20 636f 6c6f 7254 6578 742e      + colorText.
+0000faf0: 454e 440d 0a20 2020 2020 2020 2020 2020  END..           
+0000fb00: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
+0000fb10: 7361 7665 4469 6374 5b22 4d41 2d53 6967  saveDict["MA-Sig
+0000fb20: 6e61 6c22 5d20 3d20 7361 7665 645b 315d  nal"] = saved[1]
+0000fb30: 202b 2066 2252 6576 6572 7361 6c2d 5b7b   + f"Reversal-[{
+0000fb40: 272c 272e 6a6f 696e 2872 6573 756c 7473  ','.join(results
+0000fb50: 297d 5d7b 2745 4d41 2720 6966 2028 6d61  )}]{'EMA' if (ma
+0000fb60: 4c65 6e67 7468 203d 3d20 3920 6f72 2073  Length == 9 or s
+0000fb70: 656c 662e 636f 6e66 6967 4d61 6e61 6765  elf.configManage
+0000fb80: 722e 7573 6545 4d41 2920 656c 7365 2027  r.useEMA) else '
+0000fb90: 4d41 277d 220d 0a20 2020 2020 2020 2072  MA'}"..        r
+0000fba0: 6574 7572 6e20 6861 7352 6576 6572 7361  eturn hasReversa
+0000fbb0: 6c73 0d0a 0d0a 2020 2020 6465 6620 6669  ls....    def fi
+0000fbc0: 6e64 4375 7272 656e 7453 6176 6564 5661  ndCurrentSavedVa
+0000fbd0: 6c75 6528 7365 6c66 2c20 7363 7265 656e  lue(self, screen
+0000fbe0: 4469 6374 2c20 7361 7665 4469 6374 2c20  Dict, saveDict, 
+0000fbf0: 6b65 7929 3a0d 0a20 2020 2020 2020 2065  key):..        e
+0000fc00: 7869 7374 696e 6753 6372 6565 6e20 3d20  xistingScreen = 
+0000fc10: 7363 7265 656e 4469 6374 2e67 6574 286b  screenDict.get(k
+0000fc20: 6579 290d 0a20 2020 2020 2020 2065 7869  ey)..        exi
+0000fc30: 7374 696e 6753 6176 6520 3d20 7361 7665  stingSave = save
+0000fc40: 4469 6374 2e67 6574 286b 6579 290d 0a20  Dict.get(key).. 
+0000fc50: 2020 2020 2020 2065 7869 7374 696e 6753         existingS
+0000fc60: 6372 6565 6e20 3d20 6622 7b65 7869 7374  creen = f"{exist
+0000fc70: 696e 6753 6372 6565 6e7d 2c20 2220 6966  ingScreen}, " if
+0000fc80: 2028 6578 6973 7469 6e67 5363 7265 656e   (existingScreen
+0000fc90: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
+0000fca0: 206c 656e 2865 7869 7374 696e 6753 6372   len(existingScr
+0000fcb0: 6565 6e29 203e 2030 2920 656c 7365 2022  een) > 0) else "
+0000fcc0: 220d 0a20 2020 2020 2020 2065 7869 7374  "..        exist
+0000fcd0: 696e 6753 6176 6520 3d20 6622 7b65 7869  ingSave = f"{exi
+0000fce0: 7374 696e 6753 6176 657d 2c20 2220 6966  stingSave}, " if
+0000fcf0: 2028 6578 6973 7469 6e67 5361 7665 2069   (existingSave i
+0000fd00: 7320 6e6f 7420 4e6f 6e65 2061 6e64 206c  s not None and l
+0000fd10: 656e 2865 7869 7374 696e 6753 6176 6529  en(existingSave)
+0000fd20: 203e 2030 2920 656c 7365 2022 220d 0a20   > 0) else "".. 
+0000fd30: 2020 2020 2020 2072 6574 7572 6e20 6578         return ex
+0000fd40: 6973 7469 6e67 5363 7265 656e 2c20 6578  istingScreen, ex
+0000fd50: 6973 7469 6e67 5361 7665 0d0a 0d0a 2020  istingSave....  
+0000fd60: 2020 2320 406d 6561 7375 7265 5f74 696d    # @measure_tim
+0000fd70: 650d 0a20 2020 2064 6566 2066 696e 6442  e..    def findB
+0000fd80: 6261 6e64 7353 7175 6565 7a65 2873 656c  bandsSqueeze(sel
+0000fd90: 662c 6675 6c6c 4461 7461 2c20 7363 7265  f,fullData, scre
+0000fda0: 656e 4469 6374 2c20 7361 7665 4469 6374  enDict, saveDict
+0000fdb0: 2c20 6669 6c74 6572 3d34 293a 0d0a 2020  , filter=4):..  
+0000fdc0: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+0000fdd0: 2020 2054 6865 2054 544d 2053 7175 6565     The TTM Squee
+0000fde0: 7a65 2069 6e64 6963 6174 6f72 206d 6561  ze indicator mea
+0000fdf0: 7375 7265 7320 7468 6520 7265 6c61 7469  sures the relati
+0000fe00: 6f6e 7368 6970 2062 6574 7765 656e 2074  onship between t
+0000fe10: 6865 200d 0a20 2020 2020 2020 2042 6f6c  he ..        Bol
+0000fe20: 6c69 6e67 6572 2042 616e 6473 2061 6e64  linger Bands and
+0000fe30: 204b 656c 746e 6572 2773 2043 6861 6e6e   Keltner's Chann
+0000fe40: 656c 2e20 5768 656e 2074 6865 2076 6f6c  el. When the vol
+0000fe50: 6174 696c 6974 7920 696e 6372 6561 7365  atility increase
+0000fe60: 732c 200d 0a20 2020 2020 2020 2073 6f20  s, ..        so 
+0000fe70: 646f 6573 2074 6865 2064 6973 7461 6e63  does the distanc
+0000fe80: 6520 6265 7477 6565 6e20 7468 6520 6261  e between the ba
+0000fe90: 6e64 732c 2061 6e64 2063 6f6e 7665 7273  nds, and convers
+0000fea0: 656c 792c 2077 6865 6e20 7468 6520 0d0a  ely, when the ..
+0000feb0: 2020 2020 2020 2020 766f 6c61 7469 6c69          volatili
+0000fec0: 7479 2064 6563 6c69 6e65 732c 2074 6865  ty declines, the
+0000fed0: 2064 6973 7461 6e63 6520 616c 736f 2064   distance also d
+0000fee0: 6563 7265 6173 6573 2e20 5468 6520 5371  ecreases. The Sq
+0000fef0: 7565 657a 6520 696e 6469 6361 746f 7220  ueeze indicator 
+0000ff00: 0d0a 2020 2020 2020 2020 6669 6e64 7320  ..        finds 
+0000ff10: 7365 6374 696f 6e73 206f 6620 7468 6520  sections of the 
+0000ff20: 426f 6c6c 696e 6765 7220 4261 6e64 7320  Bollinger Bands 
+0000ff30: 7374 7564 7920 7768 6963 6820 6661 6c6c  study which fall
+0000ff40: 2069 6e73 6964 6520 7468 6520 0d0a 2020   inside the ..  
+0000ff50: 2020 2020 2020 4b65 6c74 6e65 7227 7320        Keltner's 
+0000ff60: 4368 616e 6e65 6c73 2e0d 0a20 2020 2020  Channels...     
+0000ff70: 2020 200d 0a20 2020 2020 2020 2041 7420     ..        At 
+0000ff80: 7468 6520 6d6f 6d65 6e74 2074 6869 7320  the moment this 
+0000ff90: 7371 7565 657a 6520 6861 7070 656e 732c  squeeze happens,
+0000ffa0: 2061 2070 7269 6365 2062 7265 616b 6f75   a price breakou
+0000ffb0: 7420 6672 6f6d 2074 6865 2075 7070 6572  t from the upper
+0000ffc0: 200d 0a20 2020 2020 2020 2042 6f6c 6c69   ..        Bolli
+0000ffd0: 6e67 6572 2042 616e 6420 776f 756c 6420  nger Band would 
+0000ffe0: 696e 6469 6361 7465 2074 6865 2070 6f73  indicate the pos
+0000fff0: 7369 6269 6c69 7479 206f 6620 616e 2075  sibility of an u
+00010000: 7074 7265 6e64 2069 6e20 7468 6520 0d0a  ptrend in the ..
+00010010: 2020 2020 2020 2020 6675 7475 7265 2e20          future. 
+00010020: 5468 6973 2069 7320 6261 636b 6564 2062  This is backed b
+00010030: 7920 7468 6520 6661 6374 2074 6861 7420  y the fact that 
+00010040: 6f6e 6365 2074 6865 2070 7269 6365 2073  once the price s
+00010050: 7461 7274 7320 6272 6561 6b69 6e67 200d  tarts breaking .
+00010060: 0a20 2020 2020 2020 206f 7574 206f 6620  .        out of 
+00010070: 7468 6520 6261 6e64 732c 2069 7420 776f  the bands, it wo
+00010080: 756c 6420 6d65 616e 2061 2072 656c 6178  uld mean a relax
+00010090: 6174 696f 6e20 6f66 2074 6865 2073 7175  ation of the squ
+000100a0: 6565 7a65 2061 6e64 2074 6865 200d 0a20  eeze and the .. 
+000100b0: 2020 2020 2020 2070 6f73 7369 6269 6c69         possibili
+000100c0: 7479 206f 6620 6869 6768 206d 6172 6b65  ty of high marke
+000100d0: 7420 766f 6c61 7469 6c69 7479 2061 6e64  t volatility and
+000100e0: 2070 7269 6365 206d 6f76 656d 656e 7420   price movement 
+000100f0: 696e 2074 6865 2066 7574 7572 652e 200d  in the future. .
+00010100: 0a20 2020 2020 2020 2053 696d 696c 6172  .        Similar
+00010110: 6c79 2c20 6120 7072 6963 6520 6272 6561  ly, a price brea
+00010120: 6b6f 7574 2066 726f 6d20 7468 6520 6c6f  kout from the lo
+00010130: 7765 7220 426f 6c6c 696e 6765 7220 4261  wer Bollinger Ba
+00010140: 6e64 2061 6674 6572 2061 2073 7175 6565  nd after a squee
+00010150: 7a65 200d 0a20 2020 2020 2020 2077 6f75  ze ..        wou
+00010160: 6c64 2069 6e64 6963 6174 6520 7468 6520  ld indicate the 
+00010170: 706f 7373 6962 696c 6974 7920 6f66 2061  possibility of a
+00010180: 2064 6f77 6e74 7265 6e64 2069 6e20 7468   downtrend in th
+00010190: 6520 6675 7475 7265 2061 6e64 2061 6e20  e future and an 
+000101a0: 0d0a 2020 2020 2020 2020 696e 6372 6561  ..        increa
+000101b0: 7365 6420 6d61 726b 6574 2076 6f6c 6174  sed market volat
+000101c0: 696c 6974 7920 696e 2074 6865 2073 616d  ility in the sam
+000101d0: 6520 6469 7265 6374 696f 6e2e 2057 6865  e direction. Whe
+000101e0: 6e20 7468 6520 6d61 726b 6574 200d 0a20  n the market .. 
+000101f0: 2020 2020 2020 2066 696e 6973 6865 7320         finishes 
+00010200: 6120 6d6f 7665 2c20 7468 6520 696e 6469  a move, the indi
+00010210: 6361 746f 7220 7475 726e 7320 6f66 662c  cator turns off,
+00010220: 2077 6869 6368 2063 6f72 7265 7370 6f6e   which correspon
+00010230: 6473 2074 6f20 6261 6e64 7320 0d0a 2020  ds to bands ..  
+00010240: 2020 2020 2020 6861 7669 6e67 2070 7573        having pus
+00010250: 6865 6420 7765 6c6c 206f 7574 7369 6465  hed well outside
+00010260: 2074 6865 2072 616e 6765 206f 6620 4b65   the range of Ke
+00010270: 6c74 6e65 7227 7320 4368 616e 6e65 6c73  ltner's Channels
+00010280: 2e0d 0a20 2020 2020 2020 2022 2222 0d0a  ...        """..
+00010290: 2020 2020 2020 2020 6966 2066 756c 6c44          if fullD
+000102a0: 6174 6120 6973 204e 6f6e 6520 6f72 206c  ata is None or l
+000102b0: 656e 2866 756c 6c44 6174 6129 203c 2032  en(fullData) < 2
+000102c0: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
+000102d0: 7265 7475 726e 2046 616c 7365 0d0a 2020  return False..  
+000102e0: 2020 2020 2020 6f6c 6465 7374 5265 636f        oldestReco
+000102f0: 7264 7346 6972 7374 5f64 6620 3d20 6675  rdsFirst_df = fu
+00010300: 6c6c 4461 7461 2e68 6561 6428 3330 292e  llData.head(30).
+00010310: 636f 7079 2829 0d0a 2020 2020 2020 2020  copy()..        
+00010320: 6c61 7465 7374 5265 636f 7264 7346 6972  latestRecordsFir
+00010330: 7374 5f64 6620 3d20 6f6c 6465 7374 5265  st_df = oldestRe
+00010340: 636f 7264 7346 6972 7374 5f64 665b 3a3a  cordsFirst_df[::
+00010350: 2d31 5d2e 7461 696c 2833 3029 0d0a 2020  -1].tail(30)..  
+00010360: 2020 2020 2020 6c61 7465 7374 5265 636f        latestReco
+00010370: 7264 7346 6972 7374 5f64 6620 3d20 6c61  rdsFirst_df = la
+00010380: 7465 7374 5265 636f 7264 7346 6972 7374  testRecordsFirst
+00010390: 5f64 662e 6669 6c6c 6e61 2830 290d 0a20  _df.fillna(0).. 
+000103a0: 2020 2020 2020 206c 6174 6573 7452 6563         latestRec
+000103b0: 6f72 6473 4669 7273 745f 6466 203d 206c  ordsFirst_df = l
+000103c0: 6174 6573 7452 6563 6f72 6473 4669 7273  atestRecordsFirs
+000103d0: 745f 6466 2e72 6570 6c61 6365 285b 6e70  t_df.replace([np
+000103e0: 2e69 6e66 2c20 2d6e 702e 696e 665d 2c20  .inf, -np.inf], 
+000103f0: 3029 0d0a 2020 2020 2020 2020 2320 426f  0)..        # Bo
+00010400: 6c6c 696e 6765 7220 6261 6e64 730d 0a20  llinger bands.. 
+00010410: 2020 2020 2020 206c 6174 6573 7452 6563         latestRec
+00010420: 6f72 6473 4669 7273 745f 6466 2e6c 6f63  ordsFirst_df.loc
+00010430: 5b3a 2c27 4242 616e 6473 2d55 275d 2c20  [:,'BBands-U'], 
+00010440: 6c61 7465 7374 5265 636f 7264 7346 6972  latestRecordsFir
+00010450: 7374 5f64 662e 6c6f 635b 3a2c 2742 4261  st_df.loc[:,'BBa
+00010460: 6e64 732d 4d27 5d2c 206c 6174 6573 7452  nds-M'], latestR
+00010470: 6563 6f72 6473 4669 7273 745f 6466 2e6c  ecordsFirst_df.l
+00010480: 6f63 5b3a 2c27 4242 616e 6473 2d4c 275d  oc[:,'BBands-L']
+00010490: 203d 2070 6b74 616c 6962 2e42 4241 4e44   = pktalib.BBAND
+000104a0: 5328 6c61 7465 7374 5265 636f 7264 7346  S(latestRecordsF
+000104b0: 6972 7374 5f64 665b 2243 6c6f 7365 225d  irst_df["Close"]
+000104c0: 2c20 3230 290d 0a20 2020 2020 2020 2023  , 20)..        #
+000104d0: 2063 6f6d 7075 7465 204b 656c 746e 6572   compute Keltner
+000104e0: 2773 2063 6861 6e6e 656c 0d0a 2020 2020  's channel..    
+000104f0: 2020 2020 6c61 7465 7374 5265 636f 7264      latestRecord
+00010500: 7346 6972 7374 5f64 665b 276c 6f77 5f6b  sFirst_df['low_k
+00010510: 656c 275d 2c20 6c61 7465 7374 5265 636f  el'], latestReco
+00010520: 7264 7346 6972 7374 5f64 665b 2775 7070  rdsFirst_df['upp
+00010530: 5f6b 656c 275d 203d 2070 6b74 616c 6962  _kel'] = pktalib
+00010540: 2e4b 656c 746e 6572 7343 6861 6e6e 656c  .KeltnersChannel
+00010550: 286c 6174 6573 7452 6563 6f72 6473 4669  (latestRecordsFi
+00010560: 7273 745f 6466 5b22 4869 6768 225d 2c20  rst_df["High"], 
+00010570: 6c61 7465 7374 5265 636f 7264 7346 6972  latestRecordsFir
+00010580: 7374 5f64 665b 224c 6f77 225d 2c6c 6174  st_df["Low"],lat
+00010590: 6573 7452 6563 6f72 6473 4669 7273 745f  estRecordsFirst_
+000105a0: 6466 5b22 436c 6f73 6522 5d2c 3230 290d  df["Close"],20).
+000105b0: 0a20 2020 2020 2020 2023 2073 7175 6565  .        # squee
+000105c0: 7a65 2069 6e64 6963 6174 6f72 0d0a 2020  ze indicator..  
+000105d0: 2020 2020 2020 6465 6620 696e 5f73 7175        def in_squ
+000105e0: 6565 7a65 2864 6629 3a0d 0a20 2020 2020  eeze(df):..     
+000105f0: 2020 2020 2020 2072 6574 7572 6e20 6466         return df
+00010600: 5b27 6c6f 775f 6b65 6c27 5d20 3c20 6466  ['low_kel'] < df
+00010610: 5b27 4242 616e 6473 2d4c 275d 203c 2064  ['BBands-L'] < d
+00010620: 665b 2742 4261 6e64 732d 5527 5d20 3c20  f['BBands-U'] < 
+00010630: 6466 5b27 7570 705f 6b65 6c27 5d0d 0a0d  df['upp_kel']...
+00010640: 0a20 2020 2020 2020 206c 6174 6573 7452  .        latestR
+00010650: 6563 6f72 6473 4669 7273 745f 6466 5b27  ecordsFirst_df['
+00010660: 7371 7565 657a 6527 5d20 3d20 6c61 7465  squeeze'] = late
+00010670: 7374 5265 636f 7264 7346 6972 7374 5f64  stRecordsFirst_d
+00010680: 662e 6170 706c 7928 696e 5f73 7175 6565  f.apply(in_squee
+00010690: 7a65 2c20 6178 6973 3d31 290d 0a0d 0a20  ze, axis=1).... 
+000106a0: 2020 2020 2020 2023 204c 6574 2773 2072         # Let's r
+000106b0: 6576 6965 7720 6a75 7374 2074 6865 2070  eview just the p
+000106c0: 7265 7669 6f75 7320 3320 6361 6e64 6c65  revious 3 candle
+000106d0: 7320 696e 636c 7564 696e 6720 746f 6461  s including toda
+000106e0: 7920 2861 7420 7468 6520 656e 6429 0d0a  y (at the end)..
+000106f0: 2020 2020 2020 2020 6c61 7465 7374 5265          latestRe
+00010700: 636f 7264 7346 6972 7374 5f64 6620 3d20  cordsFirst_df = 
+00010710: 6c61 7465 7374 5265 636f 7264 7346 6972  latestRecordsFir
+00010720: 7374 5f64 662e 7461 696c 2833 290d 0a20  st_df.tail(3).. 
+00010730: 2020 2020 2020 2023 2073 746f 636b 2069         # stock i
+00010740: 7320 636f 6d69 6e67 206f 7574 206f 6620  s coming out of 
+00010750: 7468 6520 7371 7565 657a 650d 0a20 2020  the squeeze..   
+00010760: 2020 2020 2073 6176 6564 203d 2073 656c       saved = sel
+00010770: 662e 6669 6e64 4375 7272 656e 7453 6176  f.findCurrentSav
+00010780: 6564 5661 6c75 6528 7363 7265 656e 4469  edValue(screenDi
+00010790: 6374 2c20 7361 7665 4469 6374 2c20 2250  ct, saveDict, "P
+000107a0: 6174 7465 726e 2229 0d0a 2020 2020 2020  attern")..      
+000107b0: 2020 6361 6e64 6c65 3353 717a 203d 206c    candle3Sqz = l
+000107c0: 6174 6573 7452 6563 6f72 6473 4669 7273  atestRecordsFirs
+000107d0: 745f 6466 2e69 6c6f 635b 2d33 5d5b 2273  t_df.iloc[-3]["s
+000107e0: 7175 6565 7a65 225d 0d0a 2020 2020 2020  queeze"]..      
+000107f0: 2020 6361 6e64 6c65 3153 717a 203d 206c    candle1Sqz = l
+00010800: 6174 6573 7452 6563 6f72 6473 4669 7273  atestRecordsFirs
+00010810: 745f 6466 2e69 6c6f 635b 2d31 5d5b 2273  t_df.iloc[-1]["s
+00010820: 7175 6565 7a65 225d 0d0a 2020 2020 2020  queeze"]..      
+00010830: 2020 6361 6e64 6c65 3253 717a 203d 206c    candle2Sqz = l
+00010840: 6174 6573 7452 6563 6f72 6473 4669 7273  atestRecordsFirs
+00010850: 745f 6466 2e69 6c6f 635b 2d32 5d5b 2273  t_df.iloc[-2]["s
+00010860: 7175 6565 7a65 225d 0d0a 2020 2020 2020  queeze"]..      
+00010870: 2020 6966 2063 616e 646c 6533 5371 7a20    if candle3Sqz 
+00010880: 616e 6420 6e6f 7420 6361 6e64 6c65 3153  and not candle1S
+00010890: 717a 3a0d 0a20 2020 2020 2020 2020 2020  qz:..           
+000108a0: 2023 2033 7264 2063 616e 646c 6520 6672   # 3rd candle fr
+000108b0: 6f6d 2074 6865 206d 6f73 7420 7265 6365  om the most rece
+000108c0: 6e74 206f 6e65 2077 6173 2069 6e20 7371  nt one was in sq
+000108d0: 7565 657a 6520 6275 7420 7468 6520 6d6f  ueeze but the mo
+000108e0: 7374 2072 6563 656e 7420 6f6e 6520 6973  st recent one is
+000108f0: 206e 6f74 2e0d 0a20 2020 2020 2020 2020   not...         
+00010900: 2020 2069 6620 6669 6c74 6572 206e 6f74     if filter not
+00010910: 2069 6e20 5b31 2c33 2c34 5d3a 2023 2042   in [1,3,4]: # B
+00010920: 7579 2f53 656c 6c2f 416c 6c0d 0a20 2020  uy/Sell/All..   
+00010930: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00010940: 7572 6e20 4661 6c73 650d 0a20 2020 2020  urn False..     
+00010950: 2020 2020 2020 2023 2064 6563 6964 6520         # decide 
+00010960: 7768 6963 6820 6163 7469 6f6e 2074 6f20  which action to 
+00010970: 7461 6b65 2062 7920 636f 6d70 6172 696e  take by comparin
+00010980: 6720 6469 7374 616e 6365 7320 2020 2020  g distances     
+00010990: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+000109a0: 2020 2020 2020 2020 2064 6973 7461 6e63           distanc
+000109b0: 655f 746f 5f75 7070 6572 203d 2061 6273  e_to_upper = abs
+000109c0: 286c 6174 6573 7452 6563 6f72 6473 4669  (latestRecordsFi
+000109d0: 7273 745f 6466 5b27 4242 616e 6473 2d55  rst_df['BBands-U
+000109e0: 275d 2e76 616c 7565 735b 2d31 5d20 2d20  '].values[-1] - 
+000109f0: 6c61 7465 7374 5265 636f 7264 7346 6972  latestRecordsFir
+00010a00: 7374 5f64 665b 2743 6c6f 7365 275d 2e76  st_df['Close'].v
+00010a10: 616c 7565 735b 2d31 5d29 0d0a 2020 2020  alues[-1])..    
+00010a20: 2020 2020 2020 2020 6469 7374 616e 6365          distance
+00010a30: 5f74 6f5f 6c6f 7765 7220 3d20 6162 7328  _to_lower = abs(
+00010a40: 6c61 7465 7374 5265 636f 7264 7346 6972  latestRecordsFir
+00010a50: 7374 5f64 665b 2742 4261 6e64 732d 4c27  st_df['BBands-L'
+00010a60: 5d2e 7661 6c75 6573 5b2d 315d 202d 206c  ].values[-1] - l
+00010a70: 6174 6573 7452 6563 6f72 6473 4669 7273  atestRecordsFirs
+00010a80: 745f 6466 5b27 436c 6f73 6527 5d2e 7661  t_df['Close'].va
+00010a90: 6c75 6573 5b2d 315d 290d 0a20 2020 2020  lues[-1])..     
+00010aa0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00010ab0: 2020 2020 2061 6374 696f 6e20 3d20 4661       action = Fa
+00010ac0: 6c73 650d 0a20 2020 2020 2020 2020 2020  lse..           
+00010ad0: 2069 6620 6469 7374 616e 6365 5f74 6f5f   if distance_to_
+00010ae0: 7570 7065 7220 3c20 6469 7374 616e 6365  upper < distance
+00010af0: 5f74 6f5f 6c6f 7765 723a 0d0a 2020 2020  _to_lower:..    
+00010b00: 2020 2020 2020 2020 2020 2020 6966 2066              if f
+00010b10: 696c 7465 7220 6e6f 7420 696e 205b 312c  ilter not in [1,
+00010b20: 345d 3a20 2320 4275 792f 416c 6c0d 0a20  4]: # Buy/All.. 
+00010b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b40: 2020 2072 6574 7572 6e20 4661 6c73 650d     return False.
+00010b50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010b60: 2061 6374 696f 6e20 3d20 5472 7565 0d0a   action = True..
+00010b70: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00010b80: 2066 696c 7465 7220 6e6f 7420 696e 205b   filter not in [
+00010b90: 332c 345d 3a20 2320 5365 6c6c 2f41 6c6c  3,4]: # Sell/All
+00010ba0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010bb0: 2020 7265 7475 726e 2046 616c 7365 0d0a    return False..
+00010bc0: 2020 2020 2020 2020 2020 2020 7363 7265              scre
+00010bd0: 656e 4469 6374 5b22 5061 7474 6572 6e22  enDict["Pattern"
+00010be0: 5d20 3d20 7361 7665 645b 305d 202b 2063  ] = saved[0] + c
+00010bf0: 6f6c 6f72 5465 7874 2e42 4f4c 4420 2b20  olorText.BOLD + 
+00010c00: 2863 6f6c 6f72 5465 7874 2e47 5245 454e  (colorText.GREEN
+00010c10: 2069 6620 6163 7469 6f6e 2065 6c73 6520   if action else 
+00010c20: 636f 6c6f 7254 6578 742e 4641 494c 2920  colorText.FAIL) 
+00010c30: 2b20 6622 4242 616e 6473 2d53 515a 2d7b  + f"BBands-SQZ-{
+00010c40: 2742 7579 2720 6966 2061 6374 696f 6e20  'Buy' if action 
+00010c50: 656c 7365 2027 5365 6c6c 277d 2220 2b20  else 'Sell'}" + 
+00010c60: 636f 6c6f 7254 6578 742e 454e 440d 0a20  colorText.END.. 
+00010c70: 2020 2020 2020 2020 2020 2073 6176 6544             saveD
+00010c80: 6963 745b 2250 6174 7465 726e 225d 203d  ict["Pattern"] =
+00010c90: 2073 6176 6564 5b31 5d20 2b20 6622 5454   saved[1] + f"TT
+00010ca0: 4d2d 5351 5a2d 7b27 4275 7927 2069 6620  M-SQZ-{'Buy' if 
+00010cb0: 6163 7469 6f6e 2065 6c73 6520 2753 656c  action else 'Sel
+00010cc0: 6c27 7d22 0d0a 2020 2020 2020 2020 2020  l'}"..          
+00010cd0: 2020 7265 7475 726e 2054 7275 650d 0a20    return True.. 
+00010ce0: 2020 2020 2020 2065 6c69 6620 6361 6e64         elif cand
+00010cf0: 6c65 3353 717a 2061 6e64 2063 616e 646c  le3Sqz and candl
+00010d00: 6532 5371 7a20 616e 6420 6361 6e64 6c65  e2Sqz and candle
+00010d10: 3153 717a 3a0d 0a20 2020 2020 2020 2020  1Sqz:..         
+00010d20: 2020 2023 204c 6173 7420 3320 6361 6e64     # Last 3 cand
+00010d30: 6c65 7320 696e 2073 7175 6565 7a65 0d0a  les in squeeze..
+00010d40: 2020 2020 2020 2020 2020 2020 6966 2066              if f
+00010d50: 696c 7465 7220 6e6f 7420 696e 205b 322c  ilter not in [2,
+00010d60: 345d 3a20 2320 5371 5a2f 416c 6c0d 0a20  4]: # SqZ/All.. 
+00010d70: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00010d80: 6574 7572 6e20 4661 6c73 650d 0a20 2020  eturn False..   
+00010d90: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
+00010da0: 6963 745b 2250 6174 7465 726e 225d 203d  ict["Pattern"] =
+00010db0: 2066 277b 7361 7665 645b 305d 7d7b 636f   f'{saved[0]}{co
+00010dc0: 6c6f 7254 6578 742e 424f 4c44 7d7b 636f  lorText.BOLD}{co
+00010dd0: 6c6f 7254 6578 742e 5741 524e 7d54 544d  lorText.WARN}TTM
+00010de0: 2d53 515a 7b63 6f6c 6f72 5465 7874 2e45  -SQZ{colorText.E
+00010df0: 4e44 7d27 0d0a 2020 2020 2020 2020 2020  ND}'..          
+00010e00: 2020 7361 7665 4469 6374 5b22 5061 7474    saveDict["Patt
+00010e10: 6572 6e22 5d20 3d20 6627 7b73 6176 6564  ern"] = f'{saved
+00010e20: 5b31 5d7d 5454 4d2d 5351 5a27 0d0a 2020  [1]}TTM-SQZ'..  
+00010e30: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00010e40: 2054 7275 650d 0a20 2020 2020 2020 2072   True..        r
+00010e50: 6574 7572 6e20 4661 6c73 650d 0a0d 0a20  eturn False.... 
+00010e60: 2020 2064 6566 2066 696e 6449 6e74 7261     def findIntra
+00010e70: 6461 7948 6967 6843 726f 7373 6f76 6572  dayHighCrossover
+00010e80: 2873 656c 662c 2064 662c 2061 6674 6572  (self, df, after
+00010e90: 5469 6d65 7374 616d 703d 4e6f 6e65 293a  Timestamp=None):
+00010ea0: 0d0a 2020 2020 2020 2020 6966 2064 6620  ..        if df 
+00010eb0: 6973 204e 6f6e 6520 6f72 206c 656e 2864  is None or len(d
+00010ec0: 6629 203d 3d20 303a 0d0a 2020 2020 2020  f) == 0:..      
+00010ed0: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+00010ee0: 7365 0d0a 2020 2020 2020 2020 6461 7461  se..        data
+00010ef0: 203d 2064 662e 636f 7079 2829 0d0a 2020   = df.copy()..  
+00010f00: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
+00010f10: 612e 6669 6c6c 6e61 2830 290d 0a20 2020  a.fillna(0)..   
+00010f20: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
+00010f30: 2e72 6570 6c61 6365 285b 6e70 2e69 6e66  .replace([np.inf
+00010f40: 2c20 2d6e 702e 696e 665d 2c20 3029 0d0a  , -np.inf], 0)..
+00010f50: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
+00010f60: 6174 615b 3a3a 2d31 5d20 2023 2052 6576  ata[::-1]  # Rev
+00010f70: 6572 7365 2074 6865 2064 6174 6166 7261  erse the datafra
+00010f80: 6d65 2073 6f20 7468 6174 2069 7473 2074  me so that its t
+00010f90: 6865 206f 6c64 6573 7420 6461 7465 2066  he oldest date f
+00010fa0: 6972 7374 0d0a 2020 2020 2020 2020 6469  irst..        di
+00010fb0: 6666 5f64 6620 3d20 4e6f 6e65 0d0a 2020  ff_df = None..  
+00010fc0: 2020 2020 2020 7472 793a 0d0a 2020 2020        try:..    
+00010fd0: 2020 2020 2020 2020 2320 4c65 7427 7320          # Let's 
+00010fe0: 6f6e 6c79 2063 6f6e 7369 6465 7220 7468  only consider th
+00010ff0: 6f73 6520 6361 6e64 6c65 7320 7468 6174  ose candles that
+00011000: 2061 7265 2061 6674 6572 2074 6865 2061   are after the a
+00011010: 6c65 7274 2069 7373 7565 2d74 696d 6520  lert issue-time 
+00011020: 696e 2074 6865 206d 6f72 6e69 6e67 7320  in the mornings 
+00011030: 2b20 3220 6361 6e64 6c65 7320 2866 6f72  + 2 candles (for
+00011040: 2062 7579 2f73 656c 6c29 0d0a 2020 2020   buy/sell)..    
+00011050: 2020 2020 2020 2020 6469 6666 5f64 6620          diff_df 
+00011060: 3d20 6461 7461 5b64 6174 612e 696e 6465  = data[data.inde
+00011070: 7820 3e3d 2020 7064 2e74 6f5f 6461 7465  x >=  pd.to_date
+00011080: 7469 6d65 2866 277b 504b 4461 7465 5574  time(f'{PKDateUt
+00011090: 696c 6974 6965 732e 7472 6164 696e 6744  ilities.tradingD
+000110a0: 6174 6528 292e 7374 7266 7469 6d65 2866  ate().strftime(f
+000110b0: 2225 592d 256d 2d25 6422 297d 2030 393a  "%Y-%m-%d")} 09:
+000110c0: 7b31 352b 7365 6c66 2e63 6f6e 6669 674d  {15+self.configM
+000110d0: 616e 6167 6572 2e6d 6f72 6e69 6e67 616e  anager.morningan
+000110e0: 616c 7973 6973 6361 6e64 6c65 6e75 6d62  alysiscandlenumb
+000110f0: 6572 202b 2032 7d3a 3030 2b30 353a 3330  er + 2}:00+05:30
+00011100: 2729 2e74 6f5f 6461 7465 7469 6d65 3634  ').to_datetime64
+00011110: 2829 5d0d 0a20 2020 2020 2020 2020 2020  ()]..           
+00011120: 2023 2062 726f 6b65 7253 7172 4f66 6674   # brokerSqrOfft
+00011130: 696d 6520 3d20 7064 2e74 6f5f 6461 7465  ime = pd.to_date
+00011140: 7469 6d65 2866 277b 504b 4461 7465 5574  time(f'{PKDateUt
+00011150: 696c 6974 6965 732e 7472 6164 696e 6744  ilities.tradingD
+00011160: 6174 6528 292e 7374 7266 7469 6d65 2866  ate().strftime(f
+00011170: 2225 592d 256d 2d25 6422 297d 2031 353a  "%Y-%m-%d")} 15:
+00011180: 3134 3a30 302b 3035 3a33 3027 292e 746f  14:00+05:30').to
+00011190: 5f64 6174 6574 696d 6536 3428 290d 0a20  _datetime64().. 
+000111a0: 2020 2020 2020 2065 7863 6570 743a 0d0a         except:..
+000111b0: 2020 2020 2020 2020 2020 2020 6469 6666              diff
+000111c0: 5f64 6620 3d20 6461 7461 5b64 6174 612e  _df = data[data.
+000111d0: 696e 6465 7820 3e3d 2020 7064 2e74 6f5f  index >=  pd.to_
+000111e0: 6461 7465 7469 6d65 2866 277b 504b 4461  datetime(f'{PKDa
+000111f0: 7465 5574 696c 6974 6965 732e 7472 6164  teUtilities.trad
+00011200: 696e 6744 6174 6528 292e 7374 7266 7469  ingDate().strfti
+00011210: 6d65 2866 2225 592d 256d 2d25 6422 297d  me(f"%Y-%m-%d")}
+00011220: 2030 393a 7b31 352b 7365 6c66 2e63 6f6e   09:{15+self.con
+00011230: 6669 674d 616e 6167 6572 2e6d 6f72 6e69  figManager.morni
+00011240: 6e67 616e 616c 7973 6973 6361 6e64 6c65  nganalysiscandle
+00011250: 6e75 6d62 6572 202b 2032 7d3a 3030 2b30  number + 2}:00+0
+00011260: 353a 3330 272c 2075 7463 3d54 7275 6529  5:30', utc=True)
+00011270: 5d0d 0a20 2020 2020 2020 2020 2020 2023  ]..            #
+00011280: 2062 726f 6b65 7253 7172 4f66 6674 696d   brokerSqrOfftim
+00011290: 6520 3d20 7064 2e74 6f5f 6461 7465 7469  e = pd.to_dateti
+000112a0: 6d65 2866 277b 504b 4461 7465 5574 696c  me(f'{PKDateUtil
+000112b0: 6974 6965 732e 7472 6164 696e 6744 6174  ities.tradingDat
+000112c0: 6528 292e 7374 7266 7469 6d65 2866 2225  e().strftime(f"%
+000112d0: 592d 256d 2d25 6422 297d 2031 353a 3134  Y-%m-%d")} 15:14
+000112e0: 3a30 302b 3035 3a33 3027 2c20 7574 633d  :00+05:30', utc=
+000112f0: 5472 7565 290d 0a20 2020 2020 2020 2020  True)..         
+00011300: 2020 2070 6173 730d 0a20 2020 2020 2020     pass..       
+00011310: 2064 6179 4869 6768 4166 7465 7241 6c65   dayHighAfterAle
+00011320: 7274 203d 2064 6966 665f 6466 5b22 4869  rt = diff_df["Hi
+00011330: 6768 225d 2e6d 6178 2829 0d0a 2020 2020  gh"].max()..    
+00011340: 2020 2020 6869 6768 526f 7720 3d20 6469      highRow = di
+00011350: 6666 5f64 665b 6469 6666 5f64 665b 2248  ff_df[diff_df["H
+00011360: 6967 6822 5d20 3e3d 2064 6179 4869 6768  igh"] >= dayHigh
+00011370: 4166 7465 7241 6c65 7274 5d0d 0a20 2020  AfterAlert]..   
+00011380: 2020 2020 2069 6620 6869 6768 526f 7720       if highRow 
+00011390: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
+000113a0: 6c65 6e28 6869 6768 526f 7729 203e 2030  len(highRow) > 0
+000113b0: 3a0d 0a20 2020 2020 2020 2020 2020 2068  :..            h
+000113c0: 6967 6852 6f77 203d 2068 6967 6852 6f77  ighRow = highRow
+000113d0: 2e74 6169 6c28 3129 0d0a 2020 2020 2020  .tail(1)..      
+000113e0: 2020 7265 7475 726e 2068 6967 6852 6f77    return highRow
+000113f0: 2e69 6e64 6578 5b2d 315d 2c20 6869 6768  .index[-1], high
+00011400: 526f 770d 0a0d 0a0d 0a20 2020 2064 6566  Row......    def
+00011410: 2066 696e 644d 4143 4443 726f 7373 6f76   findMACDCrossov
+00011420: 6572 2873 656c 662c 2064 662c 2061 6674  er(self, df, aft
+00011430: 6572 5469 6d65 7374 616d 703d 4e6f 6e65  erTimestamp=None
+00011440: 2c20 6e74 6843 726f 7373 6f76 6572 3d31  , nthCrossover=1
+00011450: 2c20 7570 4469 7265 6374 696f 6e3d 5472  , upDirection=Tr
+00011460: 7565 2c20 6d69 6e52 5349 3d36 3029 3a0d  ue, minRSI=60):.
+00011470: 0a20 2020 2020 2020 2069 6620 6466 2069  .        if df i
+00011480: 7320 4e6f 6e65 206f 7220 6c65 6e28 6466  s None or len(df
+00011490: 2920 3d3d 2030 3a0d 0a20 2020 2020 2020  ) == 0:..       
+000114a0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+000114b0: 650d 0a20 2020 2020 2020 2064 6174 6120  e..        data 
+000114c0: 3d20 6466 2e63 6f70 7928 290d 0a20 2020  = df.copy()..   
+000114d0: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
+000114e0: 2e66 696c 6c6e 6128 3029 0d0a 2020 2020  .fillna(0)..    
+000114f0: 2020 2020 6461 7461 203d 2064 6174 612e      data = data.
+00011500: 7265 706c 6163 6528 5b6e 702e 696e 662c  replace([np.inf,
+00011510: 202d 6e70 2e69 6e66 5d2c 2030 290d 0a20   -np.inf], 0).. 
+00011520: 2020 2020 2020 2064 6174 612e 6472 6f70         data.drop
+00011530: 6e61 2861 7869 733d 302c 2068 6f77 3d22  na(axis=0, how="
+00011540: 616c 6c22 2c20 696e 706c 6163 653d 5472  all", inplace=Tr
+00011550: 7565 2920 2320 4d61 7962 6520 7468 6572  ue) # Maybe ther
+00011560: 6520 7761 7320 6e6f 2074 7261 6465 2064  e was no trade d
+00011570: 6f6e 6520 6174 2074 6865 7365 2074 696d  one at these tim
+00011580: 6573 3f0d 0a20 2020 2020 2020 2064 6174  es?..        dat
+00011590: 6120 3d20 6461 7461 5b3a 3a2d 315d 2020  a = data[::-1]  
+000115a0: 2320 5265 7665 7273 6520 7468 6520 6461  # Reverse the da
+000115b0: 7461 6672 616d 6520 736f 2074 6861 7420  taframe so that 
+000115c0: 6974 7320 7468 6520 6f6c 6465 7374 2064  its the oldest d
+000115d0: 6174 6520 6669 7273 740d 0a20 2020 2020  ate first..     
+000115e0: 2020 206d 6163 644c 696e 652c 206d 6163     macdLine, mac
+000115f0: 6453 6967 6e61 6c2c 206d 6163 6448 6973  dSignal, macdHis
+00011600: 7420 3d20 706b 7461 6c69 622e 4d41 4344  t = pktalib.MACD
+00011610: 2864 6174 615b 2243 6c6f 7365 225d 2c20  (data["Close"], 
+00011620: 3132 2c20 3236 2c20 3929 0d0a 2020 2020  12, 26, 9)..    
+00011630: 2020 2020 2320 7273 695f 6466 203d 2070      # rsi_df = p
+00011640: 6b74 616c 6962 2e52 5349 2864 6174 615b  ktalib.RSI(data[
+00011650: 2243 6c6f 7365 225d 2c20 3134 290d 0a20  "Close"], 14).. 
+00011660: 2020 2020 2020 206c 696e 655f 6466 203d         line_df =
+00011670: 2070 642e 4461 7461 4672 616d 6528 6d61   pd.DataFrame(ma
+00011680: 6364 4c69 6e65 290d 0a20 2020 2020 2020  cdLine)..       
+00011690: 2073 6967 6e61 6c5f 6466 203d 2070 642e   signal_df = pd.
+000116a0: 4461 7461 4672 616d 6528 6d61 6364 5369  DataFrame(macdSi
+000116b0: 676e 616c 290d 0a20 2020 2020 2020 2076  gnal)..        v
+000116c0: 6f6c 5f64 6620 3d20 6461 7461 5b22 566f  ol_df = data["Vo
+000116d0: 6c75 6d65 225d 0d0a 2020 2020 2020 2020  lume"]..        
+000116e0: 6469 6666 5f64 6620 3d20 7064 2e63 6f6e  diff_df = pd.con
+000116f0: 6361 7428 5b6c 696e 655f 6466 2c20 7369  cat([line_df, si
+00011700: 676e 616c 5f64 662c 2073 6967 6e61 6c5f  gnal_df, signal_
+00011710: 6466 2d6c 696e 655f 6466 2c76 6f6c 5f64  df-line_df,vol_d
+00011720: 665d 2c20 6178 6973 3d31 290d 0a20 2020  f], axis=1)..   
+00011730: 2020 2020 2064 6966 665f 6466 2e63 6f6c       diff_df.col
+00011740: 756d 6e73 203d 205b 226c 696e 6522 2c22  umns = ["line","
+00011750: 7369 676e 616c 222c 2264 6966 6622 2c22  signal","diff","
+00011760: 766f 6c22 5d0d 0a20 2020 2020 2020 2064  vol"]..        d
+00011770: 6966 665f 6466 203d 2064 6966 665f 6466  iff_df = diff_df
+00011780: 5b64 6966 665f 6466 5b22 766f 6c22 5d20  [diff_df["vol"] 
+00011790: 3e20 305d 2023 2057 6527 7265 206e 6f74  > 0] # We're not
+000117a0: 2067 6f69 6e67 2074 6f20 646f 2061 6e79   going to do any
+000117b0: 7468 696e 6720 7769 7468 2061 2063 616e  thing with a can
+000117c0: 646c 6520 7768 6572 6520 7468 6572 6520  dle where there 
+000117d0: 7761 7320 6e6f 2074 7261 6465 2e0d 0a20  was no trade... 
+000117e0: 2020 2020 2020 2023 2062 726f 6b65 7253         # brokerS
+000117f0: 7172 4f66 6674 696d 6520 3d20 4e6f 6e65  qrOfftime = None
+00011800: 0d0a 2020 2020 2020 2020 7472 793a 0d0a  ..        try:..
+00011810: 2020 2020 2020 2020 2020 2020 2320 4c65              # Le
+00011820: 7427 7320 6f6e 6c79 2063 6f6e 7369 6465  t's only conside
+00011830: 7220 7468 6f73 6520 6361 6e64 6c65 7320  r those candles 
+00011840: 7468 6174 2061 7265 2061 6674 6572 2074  that are after t
+00011850: 6865 2061 6c65 7274 2069 7373 7565 2d74  he alert issue-t
+00011860: 696d 6520 696e 2074 6865 206d 6f72 6e69  ime in the morni
+00011870: 6e67 7320 2b20 3220 6361 6e64 6c65 7320  ngs + 2 candles 
+00011880: 2866 6f72 2062 7579 2f73 656c 6c29 0d0a  (for buy/sell)..
+00011890: 2020 2020 2020 2020 2020 2020 6469 6666              diff
+000118a0: 5f64 6620 3d20 6469 6666 5f64 665b 6469  _df = diff_df[di
+000118b0: 6666 5f64 662e 696e 6465 7820 3e3d 2020  ff_df.index >=  
+000118c0: 7064 2e74 6f5f 6461 7465 7469 6d65 2866  pd.to_datetime(f
+000118d0: 277b 504b 4461 7465 5574 696c 6974 6965  '{PKDateUtilitie
+000118e0: 732e 7472 6164 696e 6744 6174 6528 292e  s.tradingDate().
+000118f0: 7374 7266 7469 6d65 2866 2225 592d 256d  strftime(f"%Y-%m
+00011900: 2d25 6422 297d 2030 393a 7b31 352b 7365  -%d")} 09:{15+se
+00011910: 6c66 2e63 6f6e 6669 674d 616e 6167 6572  lf.configManager
+00011920: 2e6d 6f72 6e69 6e67 616e 616c 7973 6973  .morninganalysis
+00011930: 6361 6e64 6c65 6e75 6d62 6572 202b 2032  candlenumber + 2
+00011940: 7d3a 3030 2b30 353a 3330 2729 2e74 6f5f  }:00+05:30').to_
+00011950: 6461 7465 7469 6d65 3634 2829 5d0d 0a20  datetime64()].. 
+00011960: 2020 2020 2020 2020 2020 2023 2062 726f             # bro
+00011970: 6b65 7253 7172 4f66 6674 696d 6520 3d20  kerSqrOfftime = 
+00011980: 7064 2e74 6f5f 6461 7465 7469 6d65 2866  pd.to_datetime(f
+00011990: 277b 504b 4461 7465 5574 696c 6974 6965  '{PKDateUtilitie
+000119a0: 732e 7472 6164 696e 6744 6174 6528 292e  s.tradingDate().
+000119b0: 7374 7266 7469 6d65 2866 2225 592d 256d  strftime(f"%Y-%m
+000119c0: 2d25 6422 297d 2031 353a 3134 3a30 302b  -%d")} 15:14:00+
+000119d0: 3035 3a33 3027 292e 746f 5f64 6174 6574  05:30').to_datet
+000119e0: 696d 6536 3428 290d 0a20 2020 2020 2020  ime64()..       
+000119f0: 2065 7863 6570 743a 0d0a 2020 2020 2020   except:..      
+00011a00: 2020 2020 2020 6469 6666 5f64 6620 3d20        diff_df = 
+00011a10: 6469 6666 5f64 665b 6469 6666 5f64 662e  diff_df[diff_df.
+00011a20: 696e 6465 7820 3e3d 2020 7064 2e74 6f5f  index >=  pd.to_
+00011a30: 6461 7465 7469 6d65 2866 277b 504b 4461  datetime(f'{PKDa
+00011a40: 7465 5574 696c 6974 6965 732e 7472 6164  teUtilities.trad
+00011a50: 696e 6744 6174 6528 292e 7374 7266 7469  ingDate().strfti
+00011a60: 6d65 2866 2225 592d 256d 2d25 6422 297d  me(f"%Y-%m-%d")}
+00011a70: 2030 393a 7b31 352b 7365 6c66 2e63 6f6e   09:{15+self.con
+00011a80: 6669 674d 616e 6167 6572 2e6d 6f72 6e69  figManager.morni
+00011a90: 6e67 616e 616c 7973 6973 6361 6e64 6c65  nganalysiscandle
+00011aa0: 6e75 6d62 6572 202b 2032 7d3a 3030 2b30  number + 2}:00+0
+00011ab0: 353a 3330 272c 2075 7463 3d54 7275 6529  5:30', utc=True)
+00011ac0: 5d0d 0a20 2020 2020 2020 2020 2020 2023  ]..            #
+00011ad0: 2062 726f 6b65 7253 7172 4f66 6674 696d   brokerSqrOfftim
+00011ae0: 6520 3d20 7064 2e74 6f5f 6461 7465 7469  e = pd.to_dateti
+00011af0: 6d65 2866 277b 504b 4461 7465 5574 696c  me(f'{PKDateUtil
+00011b00: 6974 6965 732e 7472 6164 696e 6744 6174  ities.tradingDat
+00011b10: 6528 292e 7374 7266 7469 6d65 2866 2225  e().strftime(f"%
+00011b20: 592d 256d 2d25 6422 297d 2031 353a 3134  Y-%m-%d")} 15:14
+00011b30: 3a30 302b 3035 3a33 3027 2c20 7574 633d  :00+05:30', utc=
+00011b40: 5472 7565 290d 0a20 2020 2020 2020 2020  True)..         
+00011b50: 2020 2070 6173 730d 0a20 2020 2020 2020     pass..       
+00011b60: 2069 6e64 6578 203d 206c 656e 2864 6966   index = len(dif
+00011b70: 665f 6466 290d 0a20 2020 2020 2020 2063  f_df)..        c
+00011b80: 726f 7373 4f76 6572 203d 2030 0d0a 2020  rossOver = 0..  
+00011b90: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00011ba0: 2320 4c6f 6f70 2075 6e74 696c 2077 6527  # Loop until we'
+00011bb0: 7665 2066 6f75 6e64 2074 6865 206e 7468  ve found the nth
+00011bc0: 2063 726f 7373 6f76 6572 2066 6f72 204d   crossover for M
+00011bd0: 4143 4420 6f72 2077 6527 7665 2072 6561  ACD or we've rea
+00011be0: 6368 6564 2074 6865 206c 6173 7420 706f  ched the last po
+00011bf0: 696e 7420 696e 2074 696d 650d 0a20 2020  int in time..   
+00011c00: 2020 2020 2077 6869 6c65 2028 6372 6f73       while (cros
+00011c10: 734f 7665 7220 3c20 6e74 6843 726f 7373  sOver < nthCross
+00011c20: 6f76 6572 2061 6e64 2069 6e64 6578 203e  over and index >
+00011c30: 3d30 293a 0d0a 2020 2020 2020 2020 2020  =0):..          
+00011c40: 2020 6966 2064 6966 665f 6466 5b22 6469    if diff_df["di
+00011c50: 6666 225d 5b69 6e64 6578 2d31 5d20 3c20  ff"][index-1] < 
+00011c60: 303a 2023 2053 6967 6e61 6c20 6c69 6e65  0: # Signal line
+00011c70: 2068 6173 206e 6f74 2063 726f 7373 6564   has not crossed
+00011c80: 2079 6574 2061 6e64 2069 7320 6265 6c6f   yet and is belo
+00011c90: 7720 7468 6520 7a65 726f 206c 696e 650d  w the zero line.
+00011ca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011cb0: 2077 6869 6c65 2828 6469 6666 5f64 665b   while((diff_df[
+00011cc0: 2264 6966 6622 5d5b 696e 6465 782d 315d  "diff"][index-1]
+00011cd0: 203c 2030 2061 6e64 2069 6e64 6578 203e   < 0 and index >
+00011ce0: 3d30 2929 3a20 2320 616e 6420 6469 6666  =0)): # and diff
+00011cf0: 5f64 662e 696e 6465 7820 3c3d 2062 726f  _df.index <= bro
+00011d00: 6b65 7253 7172 4f66 6674 696d 6529 3a20  kerSqrOfftime): 
+00011d10: 2320 6f72 2064 6966 665f 6466 5b22 7273  # or diff_df["rs
+00011d20: 6922 5d5b 696e 6465 782d 315d 203c 3d20  i"][index-1] <= 
+00011d30: 6d69 6e52 5349 293a 0d0a 2020 2020 2020  minRSI):..      
+00011d40: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00011d50: 4c6f 6f70 2077 6869 6c65 2053 6967 6e61  Loop while Signa
+00011d60: 6c20 6c69 6e65 2068 6173 206e 6f74 2063  l line has not c
+00011d70: 726f 7373 6564 2079 6574 2061 6e64 2069  rossed yet and i
+00011d80: 7320 6265 6c6f 7720 7468 6520 7a65 726f  s below the zero
+00011d90: 206c 696e 6520 616e 6420 7765 2776 6520   line and we've 
+00011da0: 6e6f 7420 7265 6163 6865 6420 7468 6520  not reached the 
+00011db0: 6c61 7374 2070 6f69 6e74 0d0a 2020 2020  last point..    
+00011dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011dd0: 696e 6465 7820 2d3d 2031 0d0a 2020 2020  index -= 1..    
+00011de0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+00011df0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+00011e00: 6869 6c65 2828 6469 6666 5f64 665b 2264  hile((diff_df["d
+00011e10: 6966 6622 5d5b 696e 6465 782d 315d 203e  iff"][index-1] >
+00011e20: 3d20 3020 616e 6420 696e 6465 7820 3e3d  = 0 and index >=
+00011e30: 3029 293a 2023 2061 6e64 2064 6966 665f  0)): # and diff_
+00011e40: 6466 2e69 6e64 6578 203c 3d20 6272 6f6b  df.index <= brok
+00011e50: 6572 5371 724f 6666 7469 6d65 293a 2023  erSqrOfftime): #
+00011e60: 206f 7220 6469 6666 5f64 665b 2272 7369   or diff_df["rsi
+00011e70: 225d 5b69 6e64 6578 2d31 5d20 3c3d 206d  "][index-1] <= m
+00011e80: 696e 5253 4929 3a0d 0a20 2020 2020 2020  inRSI):..       
+00011e90: 2020 2020 2020 2020 2020 2020 2023 204c               # L
+00011ea0: 6f6f 7020 756e 7469 6c20 7369 676e 616c  oop until signal
+00011eb0: 206c 696e 6520 6861 7320 6e6f 7420 6372   line has not cr
+00011ec0: 6f73 7365 6420 7965 7420 616e 6420 6973  ossed yet and is
+00011ed0: 2061 626f 7665 2074 6865 207a 6572 6f20   above the zero 
+00011ee0: 6c69 6e65 0d0a 2020 2020 2020 2020 2020  line..          
+00011ef0: 2020 2020 2020 2020 2020 696e 6465 7820            index 
+00011f00: 2d3d 2031 0d0a 2020 2020 2020 2020 2020  -= 1..          
+00011f10: 2020 6372 6f73 734f 7665 7220 2b3d 2031    crossOver += 1
+00011f20: 0d0a 2020 2020 2020 2020 7473 203d 2064  ..        ts = d
+00011f30: 6966 665f 6466 2e74 6169 6c28 6c65 6e28  iff_df.tail(len(
+00011f40: 6469 6666 5f64 6629 2d69 6e64 6578 202b  diff_df)-index +
+00011f50: 3129 2e68 6561 6428 3129 2e69 6e64 6578  1).head(1).index
+00011f60: 5b2d 315d 0d0a 2020 2020 2020 2020 7265  [-1]..        re
+00011f70: 7475 726e 2074 732c 2064 6174 615b 6461  turn ts, data[da
+00011f80: 7461 2e69 6e64 6578 203d 3d20 7473 5d20  ta.index == ts] 
+00011f90: 2364 662e 6865 6164 286c 656e 2864 6629  #df.head(len(df)
+00011fa0: 202d 696e 6465 7820 2b31 292e 7461 696c   -index +1).tail
+00011fb0: 2831 290d 0a20 2020 200d 0a20 2020 2023  (1)..    ..    #
+00011fc0: 2046 696e 6420 7374 6f63 6b20 7368 6f77   Find stock show
+00011fd0: 696e 6720 5253 4920 6372 6f73 7369 6e67  ing RSI crossing
+00011fe0: 2077 6974 6820 5253 4920 3920 534d 410d   with RSI 9 SMA.
+00011ff0: 0a20 2020 2064 6566 2066 696e 6452 5349  .    def findRSI
+00012000: 4372 6f73 7369 6e67 4d41 2873 656c 662c  CrossingMA(self,
+00012010: 2064 662c 2073 6372 6565 6e44 6963 742c   df, screenDict,
+00012020: 2073 6176 6544 6963 742c 6c6f 6f6b 466f   saveDict,lookFo
+00012030: 723d 312c 206d 614c 656e 6774 683d 392c  r=1, maLength=9,
+00012040: 2072 7369 4b65 793d 2252 5349 2229 3a0d   rsiKey="RSI"):.
+00012050: 0a20 2020 2020 2020 2069 6620 6466 2069  .        if df i
+00012060: 7320 4e6f 6e65 206f 7220 6c65 6e28 6466  s None or len(df
+00012070: 2920 3d3d 2030 3a0d 0a20 2020 2020 2020  ) == 0:..       
+00012080: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+00012090: 650d 0a20 2020 2020 2020 2069 6620 7273  e..        if rs
+000120a0: 694b 6579 206e 6f74 2069 6e20 6466 2e63  iKey not in df.c
+000120b0: 6f6c 756d 6e73 3a0d 0a20 2020 2020 2020  olumns:..       
+000120c0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+000120d0: 650d 0a20 2020 2020 2020 2064 6174 6120  e..        data 
+000120e0: 3d20 6466 2e63 6f70 7928 290d 0a20 2020  = df.copy()..   
+000120f0: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
+00012100: 5b3a 3a2d 315d 0d0a 2020 2020 2020 2020  [::-1]..        
+00012110: 6d61 5273 6920 3d20 706b 7461 6c69 622e  maRsi = pktalib.
+00012120: 4d41 2864 6174 615b 7273 694b 6579 5d2c  MA(data[rsiKey],
+00012130: 2074 696d 6570 6572 696f 643d 6d61 4c65   timeperiod=maLe
+00012140: 6e67 7468 290d 0a20 2020 2020 2020 2064  ngth)..        d
+00012150: 6174 6120 3d20 6461 7461 5b3a 3a2d 315d  ata = data[::-1]
+00012160: 2e68 6561 6428 3329 0d0a 2020 2020 2020  .head(3)..      
+00012170: 2020 6d61 5273 6920 3d20 6d61 5273 695b    maRsi = maRsi[
+00012180: 3a3a 2d31 5d2e 6865 6164 2833 290d 0a20  ::-1].head(3).. 
+00012190: 2020 2020 2020 2073 6176 6564 203d 2073         saved = s
+000121a0: 656c 662e 6669 6e64 4375 7272 656e 7453  elf.findCurrentS
+000121b0: 6176 6564 5661 6c75 6528 7363 7265 656e  avedValue(screen
+000121c0: 4469 6374 2c73 6176 6544 6963 742c 2254  Dict,saveDict,"T
+000121d0: 7265 6e64 2229 0d0a 2020 2020 2020 2020  rend")..        
+000121e0: 6966 206c 6f6f 6b46 6f72 2069 6e20 5b31  if lookFor in [1
+000121f0: 2c33 5d20 616e 6420 6d61 5273 692e 696c  ,3] and maRsi.il
+00012200: 6f63 5b30 5d20 3c3d 2064 6174 615b 7273  oc[0] <= data[rs
+00012210: 694b 6579 5d2e 696c 6f63 5b30 5d20 616e  iKey].iloc[0] an
+00012220: 6420 6d61 5273 692e 696c 6f63 5b31 5d20  d maRsi.iloc[1] 
+00012230: 3e20 6461 7461 5b72 7369 4b65 795d 2e69  > data[rsiKey].i
+00012240: 6c6f 635b 315d 3a0d 0a20 2020 2020 2020  loc[1]:..       
+00012250: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
+00012260: 274d 412d 5369 676e 616c 275d 203d 2073  'MA-Signal'] = s
+00012270: 6176 6564 5b30 5d20 2b20 636f 6c6f 7254  aved[0] + colorT
+00012280: 6578 742e 424f 4c44 202b 2063 6f6c 6f72  ext.BOLD + color
+00012290: 5465 7874 2e47 5245 454e 202b 2066 2752  Text.GREEN + f'R
+000122a0: 5349 2d4d 412d 4275 7927 202b 2063 6f6c  SI-MA-Buy' + col
+000122b0: 6f72 5465 7874 2e45 4e44 0d0a 2020 2020  orText.END..    
+000122c0: 2020 2020 2020 2020 7361 7665 4469 6374          saveDict
+000122d0: 5b27 4d41 2d53 6967 6e61 6c27 5d20 3d20  ['MA-Signal'] = 
+000122e0: 7361 7665 645b 315d 202b 2066 2752 5349  saved[1] + f'RSI
+000122f0: 2d4d 412d 4275 7927 0d0a 2020 2020 2020  -MA-Buy'..      
+00012300: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
+00012310: 6520 6966 2028 7273 694b 6579 203d 3d20  e if (rsiKey == 
+00012320: 2252 5349 6922 2920 656c 7365 2028 7365  "RSIi") else (se
+00012330: 6c66 2e66 696e 6452 5349 4372 6f73 7369  lf.findRSICrossi
+00012340: 6e67 4d41 2864 662c 2073 6372 6565 6e44  ngMA(df, screenD
+00012350: 6963 742c 2073 6176 6544 6963 742c 6c6f  ict, saveDict,lo
+00012360: 6f6b 466f 723d 6c6f 6f6b 466f 722c 206d  okFor=lookFor, m
+00012370: 614c 656e 6774 683d 6d61 4c65 6e67 7468  aLength=maLength
+00012380: 2c20 7273 694b 6579 3d22 5253 4969 2229  , rsiKey="RSIi")
+00012390: 206f 7220 5472 7565 290d 0a20 2020 2020   or True)..     
+000123a0: 2020 2065 6c69 6620 6c6f 6f6b 466f 7220     elif lookFor 
+000123b0: 696e 205b 322c 335d 2061 6e64 206d 6152  in [2,3] and maR
+000123c0: 7369 2e69 6c6f 635b 305d 203e 3d20 6461  si.iloc[0] >= da
+000123d0: 7461 5b72 7369 4b65 795d 2e69 6c6f 635b  ta[rsiKey].iloc[
+000123e0: 305d 2061 6e64 206d 6152 7369 2e69 6c6f  0] and maRsi.ilo
+000123f0: 635b 315d 203c 2064 6174 615b 7273 694b  c[1] < data[rsiK
+00012400: 6579 5d2e 696c 6f63 5b31 5d3a 0d0a 2020  ey].iloc[1]:..  
+00012410: 2020 2020 2020 2020 2020 7363 7265 656e            screen
+00012420: 4469 6374 5b27 4d41 2d53 6967 6e61 6c27  Dict['MA-Signal'
+00012430: 5d20 3d20 7361 7665 645b 305d 202b 2063  ] = saved[0] + c
+00012440: 6f6c 6f72 5465 7874 2e42 4f4c 4420 2b20  olorText.BOLD + 
+00012450: 636f 6c6f 7254 6578 742e 4641 494c 202b  colorText.FAIL +
+00012460: 2066 2752 5349 2d4d 412d 5365 6c6c 2720   f'RSI-MA-Sell' 
+00012470: 2b20 636f 6c6f 7254 6578 742e 454e 440d  + colorText.END.
+00012480: 0a20 2020 2020 2020 2020 2020 2073 6176  .            sav
+00012490: 6544 6963 745b 274d 412d 5369 676e 616c  eDict['MA-Signal
+000124a0: 275d 203d 2073 6176 6564 5b31 5d20 2b20  '] = saved[1] + 
+000124b0: 6627 5253 492d 4d41 2d53 656c 6c27 0d0a  f'RSI-MA-Sell'..
+000124c0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000124d0: 726e 2054 7275 6520 6966 2028 7273 694b  rn True if (rsiK
+000124e0: 6579 203d 3d20 2252 5349 6922 2920 656c  ey == "RSIi") el
+000124f0: 7365 2028 7365 6c66 2e66 696e 6452 5349  se (self.findRSI
+00012500: 4372 6f73 7369 6e67 4d41 2864 662c 2073  CrossingMA(df, s
+00012510: 6372 6565 6e44 6963 742c 2073 6176 6544  creenDict, saveD
+00012520: 6963 742c 6c6f 6f6b 466f 723d 6c6f 6f6b  ict,lookFor=look
+00012530: 466f 722c 206d 614c 656e 6774 683d 6d61  For, maLength=ma
+00012540: 4c65 6e67 7468 2c20 7273 694b 6579 3d22  Length, rsiKey="
+00012550: 5253 4969 2229 206f 7220 5472 7565 290d  RSIi") or True).
+00012560: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00012570: 4661 6c73 6520 6966 2028 7273 694b 6579  False if (rsiKey
+00012580: 203d 3d20 2252 5349 6922 2920 656c 7365   == "RSIi") else
+00012590: 2028 7365 6c66 2e66 696e 6452 5349 4372   (self.findRSICr
+000125a0: 6f73 7369 6e67 4d41 2864 662c 2073 6372  ossingMA(df, scr
+000125b0: 6565 6e44 6963 742c 2073 6176 6544 6963  eenDict, saveDic
+000125c0: 742c 6c6f 6f6b 466f 723d 6c6f 6f6b 466f  t,lookFor=lookFo
+000125d0: 722c 206d 614c 656e 6774 683d 6d61 4c65  r, maLength=maLe
+000125e0: 6e67 7468 2c20 7273 694b 6579 3d22 5253  ngth, rsiKey="RS
+000125f0: 4969 2229 290d 0a20 2020 200d 0a20 2020  Ii"))..    ..   
+00012600: 2023 2046 696e 6420 7374 6f63 6b73 2077   # Find stocks w
+00012610: 6974 6820 7269 7369 6e67 2052 5349 2066  ith rising RSI f
+00012620: 726f 6d20 6c6f 7765 7220 6c65 7665 6c73  rom lower levels
+00012630: 0d0a 2020 2020 6465 6620 6669 6e64 5269  ..    def findRi
+00012640: 7369 6e67 5253 4928 7365 6c66 2c20 6466  singRSI(self, df
+00012650: 2c20 7273 694b 6579 3d22 5253 4922 293a  , rsiKey="RSI"):
+00012660: 0d0a 2020 2020 2020 2020 6966 2064 6620  ..        if df 
+00012670: 6973 204e 6f6e 6520 6f72 206c 656e 2864  is None or len(d
+00012680: 6629 203d 3d20 303a 0d0a 2020 2020 2020  f) == 0:..      
+00012690: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+000126a0: 7365 0d0a 2020 2020 2020 2020 6966 2072  se..        if r
+000126b0: 7369 4b65 7920 6e6f 7420 696e 2064 662e  siKey not in df.
+000126c0: 636f 6c75 6d6e 733a 0d0a 2020 2020 2020  columns:..      
+000126d0: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+000126e0: 7365 0d0a 2020 2020 2020 2020 6461 7461  se..        data
+000126f0: 203d 2064 662e 636f 7079 2829 0d0a 2020   = df.copy()..  
+00012700: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
+00012710: 615b 3a3a 2d31 5d0d 0a20 2020 2020 2020  a[::-1]..       
+00012720: 2064 6174 6120 3d20 6461 7461 2e74 6169   data = data.tai
+00012730: 6c28 3329 0d0a 2020 2020 2020 2020 6966  l(3)..        if
+00012740: 206c 656e 2864 6174 6129 203c 2033 3a0d   len(data) < 3:.
+00012750: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00012760: 7572 6e20 4661 6c73 650d 0a20 2020 2020  urn False..     
+00012770: 2020 2064 6179 4d69 6e75 7332 5253 4920     dayMinus2RSI 
+00012780: 3d20 6461 7461 5b22 5253 4922 5d2e 696c  = data["RSI"].il
+00012790: 6f63 5b30 5d0d 0a20 2020 2020 2020 2064  oc[0]..        d
+000127a0: 6179 4d69 6e75 7331 5253 4920 3d20 6461  ayMinus1RSI = da
+000127b0: 7461 5b22 5253 4922 5d2e 696c 6f63 5b31  ta["RSI"].iloc[1
+000127c0: 5d0d 0a20 2020 2020 2020 2064 6179 5253  ]..        dayRS
+000127d0: 4920 3d20 6461 7461 5b22 5253 4922 5d2e  I = data["RSI"].
+000127e0: 696c 6f63 5b32 5d0d 0a20 2020 2020 2020  iloc[2]..       
+000127f0: 2072 6574 7572 6e56 616c 7565 203d 2028   returnValue = (
+00012800: 6461 794d 696e 7573 3252 5349 203c 3d20  dayMinus2RSI <= 
+00012810: 3335 2061 6e64 2064 6179 4d69 6e75 7331  35 and dayMinus1
+00012820: 5253 4920 3e20 6461 794d 696e 7573 3252  RSI > dayMinus2R
+00012830: 5349 2061 6e64 2064 6179 5253 4920 3e20  SI and dayRSI > 
+00012840: 6461 794d 696e 7573 3152 5349 2920 6f72  dayMinus1RSI) or
+00012850: 205c 0d0a 2020 2020 2020 2020 2020 2020   \..            
+00012860: 2020 2020 2864 6179 4d69 6e75 7331 5253      (dayMinus1RS
+00012870: 4920 3c3d 2033 3520 616e 6420 6461 7952  I <= 35 and dayR
+00012880: 5349 203e 2064 6179 4d69 6e75 7331 5253  SI > dayMinus1RS
+00012890: 4929 0d0a 2020 2020 2020 2020 6966 2072  I)..        if r
+000128a0: 7369 4b65 7920 3d3d 2022 5253 4922 3a0d  siKey == "RSI":.
+000128b0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000128c0: 7572 6e56 616c 7565 203d 2073 656c 662e  urnValue = self.
+000128d0: 6669 6e64 5269 7369 6e67 5253 4928 6466  findRisingRSI(df
+000128e0: 2c20 7273 694b 6579 3d22 5253 4969 2229  , rsiKey="RSIi")
+000128f0: 206f 7220 7265 7475 726e 5661 6c75 650d   or returnValue.
+00012900: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00012910: 7265 7475 726e 5661 6c75 650d 0a0d 0a20  returnValue.... 
+00012920: 2020 2023 406d 6561 7375 7265 5f74 696d     #@measure_tim
+00012930: 650d 0a20 2020 2023 2046 696e 6420 6f75  e..    # Find ou
+00012940: 7420 7472 656e 6420 666f 7220 6461 7973  t trend for days
+00012950: 2074 6f20 6c6f 6f6b 6261 636b 0d0a 2020   to lookback..  
+00012960: 2020 6465 6620 6669 6e64 5472 656e 6428    def findTrend(
+00012970: 7365 6c66 2c20 6466 2c20 7363 7265 656e  self, df, screen
+00012980: 4469 6374 2c20 7361 7665 4469 6374 2c20  Dict, saveDict, 
+00012990: 6461 7973 546f 4c6f 6f6b 6261 636b 3d4e  daysToLookback=N
+000129a0: 6f6e 652c 2073 746f 636b 4e61 6d65 3d22  one, stockName="
+000129b0: 2229 3a0d 0a20 2020 2020 2020 2069 6620  "):..        if 
+000129c0: 6466 2069 7320 4e6f 6e65 206f 7220 6c65  df is None or le
+000129d0: 6e28 6466 2920 3d3d 2030 3a0d 0a20 2020  n(df) == 0:..   
+000129e0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000129f0: 2255 6e6b 6e6f 776e 220d 0a20 2020 2020  "Unknown"..     
+00012a00: 2020 2064 6174 6120 3d20 6466 2e63 6f70     data = df.cop
+00012a10: 7928 290d 0a20 2020 2020 2020 2069 6620  y()..        if 
+00012a20: 6461 7973 546f 4c6f 6f6b 6261 636b 2069  daysToLookback i
+00012a30: 7320 4e6f 6e65 3a0d 0a20 2020 2020 2020  s None:..       
+00012a40: 2020 2020 2064 6179 7354 6f4c 6f6f 6b62       daysToLookb
+00012a50: 6163 6b20 3d20 7365 6c66 2e63 6f6e 6669  ack = self.confi
+00012a60: 674d 616e 6167 6572 2e64 6179 7354 6f4c  gManager.daysToL
+00012a70: 6f6f 6b62 6163 6b0d 0a20 2020 2020 2020  ookback..       
+00012a80: 2064 6174 6120 3d20 6461 7461 2e68 6561   data = data.hea
+00012a90: 6428 6461 7973 546f 4c6f 6f6b 6261 636b  d(daysToLookback
+00012aa0: 290d 0a20 2020 2020 2020 2064 6174 6120  )..        data 
+00012ab0: 3d20 6461 7461 5b3a 3a2d 315d 0d0a 2020  = data[::-1]..  
+00012ac0: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
+00012ad0: 612e 7365 745f 696e 6465 7828 6e70 2e61  a.set_index(np.a
+00012ae0: 7261 6e67 6528 6c65 6e28 6461 7461 2929  range(len(data))
+00012af0: 290d 0a20 2020 2020 2020 2064 6174 6120  )..        data 
+00012b00: 3d20 6461 7461 2e66 696c 6c6e 6128 3029  = data.fillna(0)
+00012b10: 0d0a 2020 2020 2020 2020 6461 7461 203d  ..        data =
+00012b20: 2064 6174 612e 7265 706c 6163 6528 5b6e   data.replace([n
+00012b30: 702e 696e 662c 202d 6e70 2e69 6e66 5d2c  p.inf, -np.inf],
+00012b40: 2030 290d 0a20 2020 2020 2020 2073 6176   0)..        sav
+00012b50: 6564 203d 2073 656c 662e 6669 6e64 4375  ed = self.findCu
+00012b60: 7272 656e 7453 6176 6564 5661 6c75 6528  rrentSavedValue(
+00012b70: 7363 7265 656e 4469 6374 2c73 6176 6544  screenDict,saveD
+00012b80: 6963 742c 2254 7265 6e64 2229 0d0a 2020  ict,"Trend")..  
+00012b90: 2020 2020 2020 7472 793a 0d0a 2020 2020        try:..    
+00012ba0: 2020 2020 2020 2020 7769 7468 2053 7570          with Sup
+00012bb0: 7072 6573 734f 7574 7075 7428 7375 7070  pressOutput(supp
+00012bc0: 7265 7373 5f73 7464 6f75 743d 5472 7565  ress_stdout=True
+00012bd0: 2c20 7375 7070 7265 7373 5f73 7464 6572  , suppress_stder
+00012be0: 723d 5472 7565 293a 0d0a 2020 2020 2020  r=True):..      
+00012bf0: 2020 2020 2020 2020 2020 6461 7461 5b22            data["
+00012c00: 746f 7073 225d 203d 2064 6174 615b 2243  tops"] = data["C
+00012c10: 6c6f 7365 225d 2e69 6c6f 635b 0d0a 2020  lose"].iloc[..  
+00012c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c30: 2020 6c69 7374 280d 0a20 2020 2020 2020    list(..       
+00012c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c50: 2070 6b74 616c 6962 2e61 7267 7265 6c65   pktalib.argrele
+00012c60: 7874 7265 6d61 280d 0a20 2020 2020 2020  xtrema(..       
+00012c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c80: 2020 2020 206e 702e 6172 7261 7928 6461       np.array(da
+00012c90: 7461 5b22 436c 6f73 6522 5d29 2c20 6e70  ta["Close"]), np
+00012ca0: 2e67 7265 6174 6572 5f65 7175 616c 2c20  .greater_equal, 
+00012cb0: 6f72 6465 723d 310d 0a20 2020 2020 2020  order=1..       
+00012cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012cd0: 2029 5b30 5d0d 0a20 2020 2020 2020 2020   )[0]..         
+00012ce0: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
+00012cf0: 2020 2020 2020 2020 2020 2020 2020 5d0d                ].
+00012d00: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+00012d10: 6120 3d20 6461 7461 2e66 696c 6c6e 6128  a = data.fillna(
+00012d20: 3029 0d0a 2020 2020 2020 2020 2020 2020  0)..            
+00012d30: 6461 7461 203d 2064 6174 612e 7265 706c  data = data.repl
+00012d40: 6163 6528 5b6e 702e 696e 662c 202d 6e70  ace([np.inf, -np
+00012d50: 2e69 6e66 5d2c 2030 290d 0a0d 0a20 2020  .inf], 0)....   
+00012d60: 2020 2020 2020 2020 2074 7279 3a0d 0a20           try:.. 
+00012d70: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00012d80: 2069 6620 6c65 6e28 6461 7461 2920 3c20   if len(data) < 
+00012d90: 6461 7973 546f 4c6f 6f6b 6261 636b 3a0d  daysToLookback:.
+00012da0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012db0: 2023 2020 2020 2073 656c 662e 6465 6661   #     self.defa
+00012dc0: 756c 745f 6c6f 6767 6572 2e64 6562 7567  ult_logger.debug
+00012dd0: 2864 6174 6129 0d0a 2020 2020 2020 2020  (data)..        
+00012de0: 2020 2020 2020 2020 2320 2020 2020 7261          #     ra
+00012df0: 6973 6520 5374 6f63 6b44 6174 614e 6f74  ise StockDataNot
+00012e00: 4164 6571 7561 7465 0d0a 2020 2020 2020  Adequate..      
+00012e10: 2020 2020 2020 2020 2020 6461 7461 203d            data =
+00012e20: 2064 6174 612e 7265 706c 6163 6528 6e70   data.replace(np
+00012e30: 2e69 6e66 2c20 6e70 2e6e 616e 292e 7265  .inf, np.nan).re
+00012e40: 706c 6163 6528 2d6e 702e 696e 662c 206e  place(-np.inf, n
+00012e50: 702e 6e61 6e29 2e64 726f 706e 6128 290d  p.nan).dropna().
+00012e60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012e70: 2069 6620 6c65 6e28 6461 7461 5b22 746f   if len(data["to
+00012e80: 7073 225d 5b64 6174 612e 746f 7073 203e  ps"][data.tops >
+00012e90: 2030 5d29 203e 2031 3a0d 0a20 2020 2020   0]) > 1:..     
+00012ea0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00012eb0: 6c6f 7065 203d 206e 702e 706f 6c79 6669  lope = np.polyfi
+00012ec0: 7428 0d0a 2020 2020 2020 2020 2020 2020  t(..            
+00012ed0: 2020 2020 2020 2020 2020 2020 6461 7461              data
+00012ee0: 2e69 6e64 6578 5b64 6174 612e 746f 7073  .index[data.tops
+00012ef0: 203e 2030 5d2c 2064 6174 615b 2274 6f70   > 0], data["top
+00012f00: 7322 5d5b 6461 7461 2e74 6f70 7320 3e20  s"][data.tops > 
+00012f10: 305d 2c20 310d 0a20 2020 2020 2020 2020  0], 1..         
+00012f20: 2020 2020 2020 2020 2020 2029 5b30 5d0d             )[0].
+00012f30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012f40: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+00012f50: 2020 2020 2020 2020 2020 2020 736c 6f70              slop
+00012f60: 6520 3d20 300d 0a20 2020 2020 2020 2020  e = 0..         
+00012f70: 2020 2065 7863 6570 7420 6e70 2e6c 696e     except np.lin
+00012f80: 616c 672e 4c69 6e41 6c67 4572 726f 7220  alg.LinAlgError 
+00012f90: 6173 2065 3a20 2320 7072 6167 6d61 3a20  as e: # pragma: 
+00012fa0: 6e6f 2063 6f76 6572 0d0a 2020 2020 2020  no cover..      
+00012fb0: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+00012fc0: 6566 6175 6c74 5f6c 6f67 6765 722e 6465  efault_logger.de
+00012fd0: 6275 6728 652c 2065 7863 5f69 6e66 6f3d  bug(e, exc_info=
+00012fe0: 5472 7565 290d 0a20 2020 2020 2020 2020  True)..         
+00012ff0: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
+00013000: 745b 2254 7265 6e64 225d 203d 2028 0d0a  t["Trend"] = (..
+00013010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013020: 2020 2020 7361 7665 645b 305d 202b 2063      saved[0] + c
+00013030: 6f6c 6f72 5465 7874 2e42 4f4c 4420 2b20  olorText.BOLD + 
+00013040: 636f 6c6f 7254 6578 742e 5741 524e 202b  colorText.WARN +
+00013050: 2022 556e 6b6e 6f77 6e22 202b 2063 6f6c   "Unknown" + col
+00013060: 6f72 5465 7874 2e45 4e44 0d0a 2020 2020  orText.END..    
+00013070: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
+00013080: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00013090: 6176 6544 6963 745b 2254 7265 6e64 225d  aveDict["Trend"]
+000130a0: 203d 2073 6176 6564 5b31 5d20 2b20 2255   = saved[1] + "U
+000130b0: 6e6b 6e6f 776e 220d 0a20 2020 2020 2020  nknown"..       
+000130c0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000130d0: 7361 7665 4469 6374 5b22 5472 656e 6422  saveDict["Trend"
+000130e0: 5d0d 0a20 2020 2020 2020 2020 2020 2065  ]..            e
+000130f0: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
+00013100: 6173 2065 3a20 2023 2070 7261 676d 613a  as e:  # pragma:
+00013110: 206e 6f20 636f 7665 720d 0a20 2020 2020   no cover..     
+00013120: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00013130: 6465 6661 756c 745f 6c6f 6767 6572 2e64  default_logger.d
+00013140: 6562 7567 2865 2c20 6578 635f 696e 666f  ebug(e, exc_info
+00013150: 3d54 7275 6529 0d0a 2020 2020 2020 2020  =True)..        
+00013160: 2020 2020 2020 2020 736c 6f70 652c 205f          slope, _
+00013170: 203d 2030 2c20 300d 0a20 2020 2020 2020   = 0, 0..       
+00013180: 2020 2020 2061 6e67 6c65 203d 206e 702e       angle = np.
+00013190: 7261 6432 6465 6728 6e70 2e61 7263 7461  rad2deg(np.arcta
+000131a0: 6e28 736c 6f70 6529 290d 0a20 2020 2020  n(slope))..     
+000131b0: 2020 2020 2020 2069 6620 616e 676c 6520         if angle 
+000131c0: 3d3d 2030 3a0d 0a20 2020 2020 2020 2020  == 0:..         
+000131d0: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
+000131e0: 745b 2254 7265 6e64 225d 203d 2028 0d0a  t["Trend"] = (..
+000131f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013200: 2020 2020 7361 7665 645b 305d 202b 2063      saved[0] + c
+00013210: 6f6c 6f72 5465 7874 2e42 4f4c 4420 2b20  olorText.BOLD + 
+00013220: 636f 6c6f 7254 6578 742e 5741 524e 202b  colorText.WARN +
+00013230: 2022 556e 6b6e 6f77 6e22 202b 2063 6f6c   "Unknown" + col
+00013240: 6f72 5465 7874 2e45 4e44 0d0a 2020 2020  orText.END..    
+00013250: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
+00013260: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00013270: 6176 6544 6963 745b 2254 7265 6e64 225d  aveDict["Trend"]
+00013280: 203d 2073 6176 6564 5b31 5d20 2b20 2255   = saved[1] + "U
+00013290: 6e6b 6e6f 776e 220d 0a20 2020 2020 2020  nknown"..       
+000132a0: 2020 2020 2065 6c69 6620 616e 676c 6520       elif angle 
+000132b0: 3c3d 2033 3020 616e 6420 616e 676c 6520  <= 30 and angle 
+000132c0: 3e3d 202d 3330 3a0d 0a20 2020 2020 2020  >= -30:..       
+000132d0: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
+000132e0: 6963 745b 2254 7265 6e64 225d 203d 2028  ict["Trend"] = (
+000132f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013300: 2020 2020 2020 7361 7665 645b 305d 202b        saved[0] +
+00013310: 2063 6f6c 6f72 5465 7874 2e42 4f4c 4420   colorText.BOLD 
+00013320: 2b20 636f 6c6f 7254 6578 742e 5741 524e  + colorText.WARN
+00013330: 202b 2022 5369 6465 7761 7973 2220 2b20   + "Sideways" + 
+00013340: 636f 6c6f 7254 6578 742e 454e 440d 0a20  colorText.END.. 
+00013350: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00013360: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013370: 2020 7361 7665 4469 6374 5b22 5472 656e    saveDict["Tren
+00013380: 6422 5d20 3d20 7361 7665 645b 315d 202b  d"] = saved[1] +
+00013390: 2022 5369 6465 7761 7973 220d 0a20 2020   "Sideways"..   
+000133a0: 2020 2020 2020 2020 2065 6c69 6620 616e           elif an
+000133b0: 676c 6520 3e3d 2033 3020 616e 6420 616e  gle >= 30 and an
+000133c0: 676c 6520 3c20 3631 3a0d 0a20 2020 2020  gle < 61:..     
+000133d0: 2020 2020 2020 2020 2020 2073 6372 6565             scree
+000133e0: 6e44 6963 745b 2254 7265 6e64 225d 203d  nDict["Trend"] =
+000133f0: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
+00013400: 2020 2020 2020 2020 7361 7665 645b 305d          saved[0]
+00013410: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
+00013420: 4420 2b20 636f 6c6f 7254 6578 742e 4752  D + colorText.GR
+00013430: 4545 4e20 2b20 2257 6561 6b20 5570 2220  EEN + "Weak Up" 
+00013440: 2b20 636f 6c6f 7254 6578 742e 454e 440d  + colorText.END.
+00013450: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013460: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
+00013470: 2020 2020 7361 7665 4469 6374 5b22 5472      saveDict["Tr
+00013480: 656e 6422 5d20 3d20 7361 7665 645b 315d  end"] = saved[1]
+00013490: 202b 2022 5765 616b 2055 7022 0d0a 2020   + "Weak Up"..  
+000134a0: 2020 2020 2020 2020 2020 656c 6966 2061            elif a
+000134b0: 6e67 6c65 203e 3d20 3630 3a0d 0a20 2020  ngle >= 60:..   
+000134c0: 2020 2020 2020 2020 2020 2020 2073 6372               scr
+000134d0: 6565 6e44 6963 745b 2254 7265 6e64 225d  eenDict["Trend"]
+000134e0: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
+000134f0: 2020 2020 2020 2020 2020 7361 7665 645b            saved[
+00013500: 305d 202b 2063 6f6c 6f72 5465 7874 2e42  0] + colorText.B
+00013510: 4f4c 4420 2b20 636f 6c6f 7254 6578 742e  OLD + colorText.
+00013520: 4752 4545 4e20 2b20 2253 7472 6f6e 6720  GREEN + "Strong 
+00013530: 5570 2220 2b20 636f 6c6f 7254 6578 742e  Up" + colorText.
+00013540: 454e 440d 0a20 2020 2020 2020 2020 2020  END..           
+00013550: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+00013560: 2020 2020 2020 2020 7361 7665 4469 6374          saveDict
+00013570: 5b22 5472 656e 6422 5d20 3d20 7361 7665  ["Trend"] = save
+00013580: 645b 315d 202b 2022 5374 726f 6e67 2055  d[1] + "Strong U
+00013590: 7022 0d0a 2020 2020 2020 2020 2020 2020  p"..            
+000135a0: 656c 6966 2061 6e67 6c65 203c 3d20 2d33  elif angle <= -3
+000135b0: 3020 616e 6420 616e 676c 6520 3e20 2d36  0 and angle > -6
+000135c0: 313a 0d0a 2020 2020 2020 2020 2020 2020  1:..            
+000135d0: 2020 2020 7363 7265 656e 4469 6374 5b22      screenDict["
+000135e0: 5472 656e 6422 5d20 3d20 280d 0a20 2020  Trend"] = (..   
+000135f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013600: 2073 6176 6564 5b30 5d20 2b20 636f 6c6f   saved[0] + colo
+00013610: 7254 6578 742e 424f 4c44 202b 2063 6f6c  rText.BOLD + col
+00013620: 6f72 5465 7874 2e46 4149 4c20 2b20 2257  orText.FAIL + "W
+00013630: 6561 6b20 446f 776e 2220 2b20 636f 6c6f  eak Down" + colo
+00013640: 7254 6578 742e 454e 440d 0a20 2020 2020  rText.END..     
+00013650: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
+00013660: 2020 2020 2020 2020 2020 2020 2020 7361                sa
+00013670: 7665 4469 6374 5b22 5472 656e 6422 5d20  veDict["Trend"] 
+00013680: 3d20 7361 7665 645b 315d 202b 2022 5765  = saved[1] + "We
+00013690: 616b 2044 6f77 6e22 0d0a 2020 2020 2020  ak Down"..      
+000136a0: 2020 2020 2020 656c 6966 2061 6e67 6c65        elif angle
+000136b0: 203c 202d 3630 3a0d 0a20 2020 2020 2020   < -60:..       
+000136c0: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
+000136d0: 6963 745b 2254 7265 6e64 225d 203d 2028  ict["Trend"] = (
+000136e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000136f0: 2020 2020 2020 7361 7665 645b 305d 202b        saved[0] +
+00013700: 2063 6f6c 6f72 5465 7874 2e42 4f4c 4420   colorText.BOLD 
+00013710: 2b20 636f 6c6f 7254 6578 742e 4641 494c  + colorText.FAIL
+00013720: 202b 2022 5374 726f 6e67 2044 6f77 6e22   + "Strong Down"
+00013730: 202b 2063 6f6c 6f72 5465 7874 2e45 4e44   + colorText.END
+00013740: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013750: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
+00013760: 2020 2020 2073 6176 6544 6963 745b 2254       saveDict["T
+00013770: 7265 6e64 225d 203d 2073 6176 6564 5b31  rend"] = saved[1
+00013780: 5d20 2b20 2253 7472 6f6e 6720 446f 776e  ] + "Strong Down
+00013790: 220d 0a20 2020 2020 2020 2065 7863 6570  "..        excep
+000137a0: 7420 6e70 2e6c 696e 616c 672e 4c69 6e41  t np.linalg.LinA
+000137b0: 6c67 4572 726f 7220 6173 2065 3a20 2320  lgError as e: # 
+000137c0: 7072 6167 6d61 3a20 6e6f 2063 6f76 6572  pragma: no cover
+000137d0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+000137e0: 6c66 2e64 6566 6175 6c74 5f6c 6f67 6765  lf.default_logge
+000137f0: 722e 6465 6275 6728 652c 2065 7863 5f69  r.debug(e, exc_i
+00013800: 6e66 6f3d 5472 7565 290d 0a20 2020 2020  nfo=True)..     
+00013810: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
+00013820: 745b 2254 7265 6e64 225d 203d 2028 0d0a  t["Trend"] = (..
+00013830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013840: 7361 7665 645b 305d 202b 2063 6f6c 6f72  saved[0] + color
+00013850: 5465 7874 2e42 4f4c 4420 2b20 636f 6c6f  Text.BOLD + colo
+00013860: 7254 6578 742e 5741 524e 202b 2022 556e  rText.WARN + "Un
+00013870: 6b6e 6f77 6e22 202b 2063 6f6c 6f72 5465  known" + colorTe
+00013880: 7874 2e45 4e44 0d0a 2020 2020 2020 2020  xt.END..        
+00013890: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
+000138a0: 2020 2073 6176 6544 6963 745b 2254 7265     saveDict["Tre
+000138b0: 6e64 225d 203d 2073 6176 6564 5b31 5d20  nd"] = saved[1] 
+000138c0: 2b20 2255 6e6b 6e6f 776e 220d 0a20 2020  + "Unknown"..   
+000138d0: 2020 2020 2072 6574 7572 6e20 7361 7665       return save
+000138e0: 4469 6374 5b22 5472 656e 6422 5d0d 0a0d  Dict["Trend"]...
+000138f0: 0a20 2020 2023 2046 696e 6420 7374 6f63  .    # Find stoc
+00013900: 6b73 2061 7070 726f 6368 696e 6720 746f  ks approching to
+00013910: 206c 6f6e 6720 7465 726d 2074 7265 6e64   long term trend
+00013920: 6c69 6e65 730d 0a20 2020 2064 6566 2066  lines..    def f
+00013930: 696e 6454 7265 6e64 6c69 6e65 7328 7365  indTrendlines(se
+00013940: 6c66 2c20 6466 2c20 7363 7265 656e 4469  lf, df, screenDi
+00013950: 6374 2c20 7361 7665 4469 6374 2c20 7065  ct, saveDict, pe
+00013960: 7263 656e 7461 6765 3d30 2e30 3529 3a0d  rcentage=0.05):.
+00013970: 0a20 2020 2020 2020 2023 2070 6572 696f  .        # perio
+00013980: 6420 3d20 696e 7428 2222 2e6a 6f69 6e28  d = int("".join(
+00013990: 6320 666f 7220 6320 696e 2073 656c 662e  c for c in self.
+000139a0: 636f 6e66 6967 4d61 6e61 6765 722e 7065  configManager.pe
+000139b0: 7269 6f64 2069 6620 632e 6973 6469 6769  riod if c.isdigi
+000139c0: 7428 2929 290d 0a20 2020 2020 2020 2023  t()))..        #
+000139d0: 2069 6620 6c65 6e28 6461 7461 2920 3c20   if len(data) < 
+000139e0: 7065 7269 6f64 3a0d 0a20 2020 2020 2020  period:..       
+000139f0: 2023 2020 2020 2072 6574 7572 6e20 4661   #     return Fa
+00013a00: 6c73 650d 0a20 2020 2020 2020 2064 6174  lse..        dat
+00013a10: 6120 3d20 6466 2e63 6f70 7928 290d 0a20  a = df.copy().. 
+00013a20: 2020 2020 2020 2064 6174 6120 3d20 6461         data = da
+00013a30: 7461 5b3a 3a2d 315d 0d0a 2020 2020 2020  ta[::-1]..      
+00013a40: 2020 6461 7461 5b22 4e75 6d62 6572 225d    data["Number"]
+00013a50: 203d 206e 702e 6172 616e 6765 286c 656e   = np.arange(len
+00013a60: 2864 6174 6129 2920 2b20 310d 0a20 2020  (data)) + 1..   
+00013a70: 2020 2020 2064 6174 615f 6c6f 7720 3d20       data_low = 
+00013a80: 6461 7461 2e63 6f70 7928 290d 0a20 2020  data.copy()..   
+00013a90: 2020 2020 2070 6f69 6e74 7320 3d20 3330       points = 30
+00013aa0: 0d0a 0d0a 2020 2020 2020 2020 2222 2220  ....        """ 
+00013ab0: 4967 6e6f 7269 6e67 2074 6865 2052 6573  Ignoring the Res
+00013ac0: 6974 616e 6365 2066 6f72 206c 6f6e 672d  itance for long-
+00013ad0: 7465 726d 2070 7572 706f 7365 0d0a 2020  term purpose..  
+00013ae0: 2020 2020 2020 7768 696c 6520 6c65 6e28        while len(
+00013af0: 6461 7461 5f68 6967 6829 203e 2070 6f69  data_high) > poi
+00013b00: 6e74 733a 0d0a 2020 2020 2020 2020 2020  nts:..          
+00013b10: 2020 736c 6f70 652c 2069 6e74 6572 6365    slope, interce
+00013b20: 7074 2c20 725f 7661 6c75 652c 2070 5f76  pt, r_value, p_v
+00013b30: 616c 7565 2c20 7374 645f 6572 7220 3d20  alue, std_err = 
+00013b40: 6c69 6e72 6567 7265 7373 2878 3d64 6174  linregress(x=dat
+00013b50: 615f 6869 6768 5b27 4e75 6d62 6572 275d  a_high['Number']
+00013b60: 2c20 793d 6461 7461 5f68 6967 685b 2748  , y=data_high['H
+00013b70: 6967 6827 5d29 0d0a 2020 2020 2020 2020  igh'])..        
+00013b80: 2020 2020 6461 7461 5f68 6967 6820 3d20      data_high = 
+00013b90: 6461 7461 5f68 6967 682e 6c6f 635b 6461  data_high.loc[da
+00013ba0: 7461 5f68 6967 685b 2748 6967 6827 5d20  ta_high['High'] 
+00013bb0: 3e20 736c 6f70 6520 2a20 6461 7461 5f68  > slope * data_h
+00013bc0: 6967 685b 274e 756d 6265 7227 5d20 2b20  igh['Number'] + 
+00013bd0: 696e 7465 7263 6570 745d 0d0a 2020 2020  intercept]..    
+00013be0: 2020 2020 736c 6f70 652c 2069 6e74 6572      slope, inter
+00013bf0: 6365 7074 2c20 725f 7661 6c75 652c 2070  cept, r_value, p
+00013c00: 5f76 616c 7565 2c20 7374 645f 6572 7220  _value, std_err 
+00013c10: 3d20 6c69 6e72 6567 7265 7373 2878 3d64  = linregress(x=d
+00013c20: 6174 615f 6869 6768 5b27 4e75 6d62 6572  ata_high['Number
+00013c30: 275d 2c20 793d 6461 7461 5f68 6967 685b  '], y=data_high[
+00013c40: 2743 6c6f 7365 275d 290d 0a20 2020 2020  'Close'])..     
+00013c50: 2020 2064 6174 615b 2752 6573 6973 7461     data['Resista
+00013c60: 6e63 6527 5d20 3d20 736c 6f70 6520 2a20  nce'] = slope * 
+00013c70: 6461 7461 5b27 4e75 6d62 6572 275d 202b  data['Number'] +
+00013c80: 2069 6e74 6572 6365 7074 0d0a 2020 2020   intercept..    
+00013c90: 2020 2020 2222 220d 0a0d 0a20 2020 2020      """....     
+00013ca0: 2020 2077 6869 6c65 206c 656e 2864 6174     while len(dat
+00013cb0: 615f 6c6f 7729 203e 2070 6f69 6e74 733a  a_low) > points:
+00013cc0: 0d0a 2020 2020 2020 2020 2020 2020 7472  ..            tr
+00013cd0: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
+00013ce0: 2020 2020 736c 6f70 652c 2069 6e74 6572      slope, inter
+00013cf0: 6365 7074 2c20 725f 7661 6c75 652c 2070  cept, r_value, p
+00013d00: 5f76 616c 7565 2c20 7374 645f 6572 7220  _value, std_err 
+00013d10: 3d20 6c69 6e72 6567 7265 7373 280d 0a20  = linregress(.. 
+00013d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013d30: 2020 2078 3d64 6174 615f 6c6f 775b 224e     x=data_low["N
+00013d40: 756d 6265 7222 5d2c 2079 3d64 6174 615f  umber"], y=data_
+00013d50: 6c6f 775b 224c 6f77 225d 0d0a 2020 2020  low["Low"]..    
+00013d60: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
+00013d70: 2020 2020 2020 2020 2020 2065 7863 6570             excep
+00013d80: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
+00013d90: 3a20 2023 2070 7261 676d 613a 206e 6f20  :  # pragma: no 
+00013da0: 636f 7665 720d 0a20 2020 2020 2020 2020  cover..         
+00013db0: 2020 2020 2020 2073 656c 662e 6465 6661         self.defa
+00013dc0: 756c 745f 6c6f 6767 6572 2e64 6562 7567  ult_logger.debug
+00013dd0: 2865 2c20 6578 635f 696e 666f 3d54 7275  (e, exc_info=Tru
+00013de0: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
+00013df0: 2020 2020 636f 6e74 696e 7565 0d0a 2020      continue..  
+00013e00: 2020 2020 2020 2020 2020 6461 7461 5f6c            data_l
+00013e10: 6f77 203d 2064 6174 615f 6c6f 772e 6c6f  ow = data_low.lo
+00013e20: 635b 0d0a 2020 2020 2020 2020 2020 2020  c[..            
+00013e30: 2020 2020 6461 7461 5f6c 6f77 5b22 4c6f      data_low["Lo
+00013e40: 7722 5d20 3c20 736c 6f70 6520 2a20 6461  w"] < slope * da
+00013e50: 7461 5f6c 6f77 5b22 4e75 6d62 6572 225d  ta_low["Number"]
+00013e60: 202b 2069 6e74 6572 6365 7074 0d0a 2020   + intercept..  
+00013e70: 2020 2020 2020 2020 2020 5d0d 0a0d 0a20            ].... 
+00013e80: 2020 2020 2020 2073 6c6f 7065 2c20 696e         slope, in
+00013e90: 7465 7263 6570 742c 2072 5f76 616c 7565  tercept, r_value
+00013ea0: 2c20 705f 7661 6c75 652c 2073 7464 5f65  , p_value, std_e
+00013eb0: 7272 203d 206c 696e 7265 6772 6573 7328  rr = linregress(
+00013ec0: 0d0a 2020 2020 2020 2020 2020 2020 783d  ..            x=
+00013ed0: 6461 7461 5f6c 6f77 5b22 4e75 6d62 6572  data_low["Number
+00013ee0: 225d 2c20 793d 6461 7461 5f6c 6f77 5b22  "], y=data_low["
+00013ef0: 436c 6f73 6522 5d0d 0a20 2020 2020 2020  Close"]..       
+00013f00: 2029 0d0a 2020 2020 2020 2020 6461 7461   )..        data
+00013f10: 5b22 5375 7070 6f72 7422 5d20 3d20 736c  ["Support"] = sl
+00013f20: 6f70 6520 2a20 6461 7461 5b22 4e75 6d62  ope * data["Numb
+00013f30: 6572 225d 202b 2069 6e74 6572 6365 7074  er"] + intercept
+00013f40: 0d0a 2020 2020 2020 2020 6e6f 7720 3d20  ..        now = 
+00013f50: 6461 7461 2e74 6169 6c28 3129 0d0a 0d0a  data.tail(1)....
+00013f60: 2020 2020 2020 2020 6c69 6d69 745f 7570          limit_up
+00013f70: 7065 7220 3d20 6e6f 775b 2253 7570 706f  per = now["Suppo
+00013f80: 7274 225d 2e69 6c6f 635b 305d 202b 2028  rt"].iloc[0] + (
+00013f90: 6e6f 775b 2253 7570 706f 7274 225d 2e69  now["Support"].i
+00013fa0: 6c6f 635b 305d 202a 2070 6572 6365 6e74  loc[0] * percent
+00013fb0: 6167 6529 0d0a 2020 2020 2020 2020 6c69  age)..        li
+00013fc0: 6d69 745f 6c6f 7765 7220 3d20 6e6f 775b  mit_lower = now[
+00013fd0: 2253 7570 706f 7274 225d 2e69 6c6f 635b  "Support"].iloc[
+00013fe0: 305d 202d 2028 6e6f 775b 2253 7570 706f  0] - (now["Suppo
+00013ff0: 7274 225d 2e69 6c6f 635b 305d 202a 2070  rt"].iloc[0] * p
+00014000: 6572 6365 6e74 6167 6529 0d0a 2020 2020  ercentage)..    
+00014010: 2020 2020 7361 7665 6420 3d20 7365 6c66      saved = self
+00014020: 2e66 696e 6443 7572 7265 6e74 5361 7665  .findCurrentSave
+00014030: 6456 616c 7565 2873 6372 6565 6e44 6963  dValue(screenDic
+00014040: 742c 2073 6176 6544 6963 742c 2022 5061  t, saveDict, "Pa
+00014050: 7474 6572 6e22 290d 0a20 2020 2020 2020  ttern")..       
+00014060: 2069 6620 6c69 6d69 745f 6c6f 7765 7220   if limit_lower 
+00014070: 3c20 6e6f 775b 2243 6c6f 7365 225d 2e69  < now["Close"].i
+00014080: 6c6f 635b 305d 203c 206c 696d 6974 5f75  loc[0] < limit_u
+00014090: 7070 6572 2061 6e64 2073 6c6f 7065 203e  pper and slope >
+000140a0: 2030 2e31 353a 0d0a 2020 2020 2020 2020   0.15:..        
+000140b0: 2020 2020 7363 7265 656e 4469 6374 5b22      screenDict["
+000140c0: 5061 7474 6572 6e22 5d20 3d20 280d 0a20  Pattern"] = (.. 
+000140d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000140e0: 6176 6564 5b30 5d20 2b20 636f 6c6f 7254  aved[0] + colorT
+000140f0: 6578 742e 424f 4c44 202b 2063 6f6c 6f72  ext.BOLD + color
+00014100: 5465 7874 2e47 5245 454e 202b 2022 5472  Text.GREEN + "Tr
+00014110: 656e 646c 696e 652d 5375 7070 6f72 7422  endline-Support"
+00014120: 202b 2063 6f6c 6f72 5465 7874 2e45 4e44   + colorText.END
+00014130: 0d0a 2020 2020 2020 2020 2020 2020 290d  ..            ).
+00014140: 0a20 2020 2020 2020 2020 2020 2073 6176  .            sav
+00014150: 6544 6963 745b 2250 6174 7465 726e 225d  eDict["Pattern"]
+00014160: 203d 2073 6176 6564 5b31 5d20 2b20 2254   = saved[1] + "T
+00014170: 7265 6e64 6c69 6e65 2d53 7570 706f 7274  rendline-Support
+00014180: 220d 0a20 2020 2020 2020 2020 2020 2072  "..            r
+00014190: 6574 7572 6e20 5472 7565 0d0a 0d0a 2020  eturn True....  
+000141a0: 2020 2020 2020 2222 2220 506c 6f74 7320        """ Plots 
+000141b0: 666f 7220 6465 6275 6767 696e 670d 0a20  for debugging.. 
+000141c0: 2020 2020 2020 2069 6d70 6f72 7420 6d61         import ma
+000141d0: 7470 6c6f 746c 6962 2e70 7970 6c6f 7420  tplotlib.pyplot 
+000141e0: 6173 2070 6c74 0d0a 2020 2020 2020 2020  as plt..        
+000141f0: 6669 672c 2061 7831 203d 2070 6c74 2e73  fig, ax1 = plt.s
+00014200: 7562 706c 6f74 7328 6669 6773 697a 653d  ubplots(figsize=
+00014210: 2831 352c 3130 2929 0d0a 2020 2020 2020  (15,10))..      
+00014220: 2020 636f 6c6f 7220 3d20 2774 6162 3a67    color = 'tab:g
+00014230: 7265 656e 270d 0a20 2020 2020 2020 2078  reen'..        x
+00014240: 6461 7465 203d 205b 782e 6461 7465 2829  date = [x.date()
+00014250: 2066 6f72 2078 2069 6e20 6461 7461 2e69   for x in data.i
+00014260: 6e64 6578 5d0d 0a20 2020 2020 2020 2061  ndex]..        a
+00014270: 7831 2e73 6574 5f78 6c61 6265 6c28 2744  x1.set_xlabel('D
+00014280: 6174 6527 2c20 636f 6c6f 723d 636f 6c6f  ate', color=colo
+00014290: 7229 0d0a 2020 2020 2020 2020 6178 312e  r)..        ax1.
+000142a0: 706c 6f74 2878 6461 7465 2c20 6461 7461  plot(xdate, data
+000142b0: 2e43 6c6f 7365 2c20 6c61 6265 6c3d 2263  .Close, label="c
+000142c0: 6c6f 7365 222c 2063 6f6c 6f72 3d63 6f6c  lose", color=col
+000142d0: 6f72 290d 0a20 2020 2020 2020 2061 7831  or)..        ax1
+000142e0: 2e74 6963 6b5f 7061 7261 6d73 2861 7869  .tick_params(axi
+000142f0: 733d 2778 272c 206c 6162 656c 636f 6c6f  s='x', labelcolo
+00014300: 723d 636f 6c6f 7229 0d0a 0d0a 2020 2020  r=color)....    
+00014310: 2020 2020 6178 3220 3d20 6178 312e 7477      ax2 = ax1.tw
+00014320: 696e 7928 2920 2320 6178 3220 616e 6420  iny() # ax2 and 
+00014330: 6178 3120 7769 6c6c 2068 6176 6520 636f  ax1 will have co
+00014340: 6d6d 6f6e 2079 2061 7869 7320 616e 6420  mmon y axis and 
+00014350: 6469 6666 6572 656e 7420 7820 6178 6973  different x axis
+00014360: 2c20 7477 696e 790d 0a20 2020 2020 2020  , twiny..       
+00014370: 2061 7832 2e70 6c6f 7428 6461 7461 2e4e   ax2.plot(data.N
+00014380: 756d 6265 722c 2064 6174 612e 5265 7369  umber, data.Resi
+00014390: 7374 616e 6365 2c20 6c61 6265 6c3d 2252  stance, label="R
+000143a0: 6573 2229 0d0a 2020 2020 2020 2020 6178  es")..        ax
+000143b0: 322e 706c 6f74 2864 6174 612e 4e75 6d62  2.plot(data.Numb
+000143c0: 6572 2c20 6461 7461 2e53 7570 706f 7274  er, data.Support
+000143d0: 2c20 6c61 6265 6c3d 2253 7570 2229 0d0a  , label="Sup")..
+000143e0: 0d0a 2020 2020 2020 2020 706c 742e 6c65  ..        plt.le
+000143f0: 6765 6e64 2829 0d0a 2020 2020 2020 2020  gend()..        
+00014400: 706c 742e 6772 6964 2829 0d0a 2020 2020  plt.grid()..    
+00014410: 2020 2020 706c 742e 7368 6f77 2829 0d0a      plt.show()..
+00014420: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+00014430: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+00014440: 650d 0a0d 0a20 2020 2023 2040 6d65 6173  e....    # @meas
+00014450: 7572 655f 7469 6d65 0d0a 2020 2020 6465  ure_time..    de
+00014460: 6620 6669 6e64 5570 7472 656e 6428 7365  f findUptrend(se
+00014470: 6c66 2c20 6466 2c20 7363 7265 656e 4469  lf, df, screenDi
+00014480: 6374 2c20 7361 7665 4469 6374 2c20 7465  ct, saveDict, te
+00014490: 7374 696e 672c 2073 746f 636b 2c6f 6e6c  sting, stock,onl
+000144a0: 794d 463d 4661 6c73 652c 686f 7374 4461  yMF=False,hostDa
+000144b0: 7461 3d4e 6f6e 652c 6578 6368 616e 6765  ta=None,exchange
+000144c0: 4e61 6d65 3d22 494e 4449 4122 293a 0d0a  Name="INDIA"):..
+000144d0: 2020 2020 2020 2020 2320 7368 6f75 6c64          # should
+000144e0: 5072 6f63 6565 6420 3d20 5472 7565 0d0a  Proceed = True..
+000144f0: 2020 2020 2020 2020 6973 5570 7472 656e          isUptren
+00014500: 6420 3d20 4661 6c73 650d 0a20 2020 2020  d = False..     
+00014510: 2020 2069 7344 6f77 6e74 7265 6e64 203d     isDowntrend =
+00014520: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
+00014530: 6973 3530 444d 4155 7074 7265 6e64 203d  is50DMAUptrend =
+00014540: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
+00014550: 6973 3530 444d 4144 6f77 6e74 7265 6e64  is50DMADowntrend
+00014560: 203d 2046 616c 7365 0d0a 2020 2020 2020   = False..      
+00014570: 2020 6465 6369 7369 6f6e 203d 2022 220d    decision = "".
+00014580: 0a20 2020 2020 2020 2064 6d61 3530 6465  .        dma50de
+00014590: 6369 7369 6f6e 203d 2022 220d 0a20 2020  cision = ""..   
+000145a0: 2020 2020 2066 6169 7256 616c 7565 203d       fairValue =
+000145b0: 2030 0d0a 2020 2020 2020 2020 6661 6972   0..        fair
+000145c0: 5661 6c75 6544 6966 6620 3d20 300d 0a20  ValueDiff = 0.. 
+000145d0: 2020 2020 2020 2023 2069 6620 6466 2069         # if df i
+000145e0: 7320 4e6f 6e65 206f 7220 6c65 6e28 6466  s None or len(df
+000145f0: 2920 3c20 3232 3020 6f72 2074 6573 7469  ) < 220 or testi
+00014600: 6e67 3a0d 0a20 2020 2020 2020 2023 2020  ng:..        #  
+00014610: 2020 2073 686f 756c 6450 726f 6365 6564     shouldProceed
+00014620: 203d 2046 616c 7365 0d0a 2020 2020 2020   = False..      
+00014630: 2020 6966 2064 6620 6973 206e 6f74 204e    if df is not N
+00014640: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+00014650: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
+00014660: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
+00014670: 662e 636f 7079 2829 0d0a 2020 2020 2020  f.copy()..      
+00014680: 2020 2020 2020 2020 2020 6461 7461 203d            data =
+00014690: 2064 6174 615b 3a3a 2d31 5d0d 0a20 2020   data[::-1]..   
+000146a0: 2020 2020 2020 2020 2020 2020 2074 6f64               tod
+000146b0: 6179 5f73 6d61 203d 2070 6b74 616c 6962  ay_sma = pktalib
+000146c0: 2e53 4d41 2864 6174 615b 2243 6c6f 7365  .SMA(data["Close
+000146d0: 225d 2c20 7469 6d65 7065 7269 6f64 3d35  "], timeperiod=5
+000146e0: 3029 0d0a 2020 2020 2020 2020 2020 2020  0)..            
+000146f0: 2020 2020 736d 615f 6d69 6e75 7339 203d      sma_minus9 =
+00014700: 2070 6b74 616c 6962 2e53 4d41 2864 6174   pktalib.SMA(dat
+00014710: 612e 6865 6164 286c 656e 2864 6174 6129  a.head(len(data)
+00014720: 2d39 295b 2243 6c6f 7365 225d 2c20 7469  -9)["Close"], ti
+00014730: 6d65 7065 7269 6f64 3d35 3029 0d0a 2020  meperiod=50)..  
+00014740: 2020 2020 2020 2020 2020 2020 2020 736d                sm
+00014750: 615f 6d69 6e75 7331 3420 3d20 706b 7461  a_minus14 = pkta
+00014760: 6c69 622e 534d 4128 6461 7461 2e68 6561  lib.SMA(data.hea
+00014770: 6428 6c65 6e28 6461 7461 292d 3134 295b  d(len(data)-14)[
+00014780: 2243 6c6f 7365 225d 2c20 7469 6d65 7065  "Close"], timepe
+00014790: 7269 6f64 3d35 3029 0d0a 2020 2020 2020  riod=50)..      
+000147a0: 2020 2020 2020 2020 2020 736d 615f 6d69            sma_mi
+000147b0: 6e75 7332 3020 3d20 706b 7461 6c69 622e  nus20 = pktalib.
+000147c0: 534d 4128 6461 7461 2e68 6561 6428 6c65  SMA(data.head(le
+000147d0: 6e28 6461 7461 292d 3230 295b 2243 6c6f  n(data)-20)["Clo
+000147e0: 7365 225d 2c20 7469 6d65 7065 7269 6f64  se"], timeperiod
+000147f0: 3d35 3029 0d0a 2020 2020 2020 2020 2020  =50)..          
+00014800: 2020 2020 2020 746f 6461 795f 6c6d 6120        today_lma 
+00014810: 3d20 706b 7461 6c69 622e 534d 4128 6461  = pktalib.SMA(da
+00014820: 7461 5b22 436c 6f73 6522 5d2c 2074 696d  ta["Close"], tim
+00014830: 6570 6572 696f 643d 3230 3029 0d0a 2020  eperiod=200)..  
+00014840: 2020 2020 2020 2020 2020 2020 2020 6c6d                lm
+00014850: 615f 6d69 6e75 7332 3020 3d20 706b 7461  a_minus20 = pkta
+00014860: 6c69 622e 534d 4128 6461 7461 2e68 6561  lib.SMA(data.hea
+00014870: 6428 6c65 6e28 6461 7461 292d 3230 295b  d(len(data)-20)[
+00014880: 2243 6c6f 7365 225d 2c20 7469 6d65 7065  "Close"], timepe
+00014890: 7269 6f64 3d32 3030 290d 0a20 2020 2020  riod=200)..     
+000148a0: 2020 2020 2020 2020 2020 206c 6d61 5f6d             lma_m
+000148b0: 696e 7573 3830 203d 2070 6b74 616c 6962  inus80 = pktalib
+000148c0: 2e53 4d41 2864 6174 612e 6865 6164 286c  .SMA(data.head(l
+000148d0: 656e 2864 6174 6129 2d38 3029 5b22 436c  en(data)-80)["Cl
+000148e0: 6f73 6522 5d2c 2074 696d 6570 6572 696f  ose"], timeperio
+000148f0: 643d 3230 3029 0d0a 2020 2020 2020 2020  d=200)..        
+00014900: 2020 2020 2020 2020 6c6d 615f 6d69 6e75          lma_minu
+00014910: 7331 3030 203d 2070 6b74 616c 6962 2e53  s100 = pktalib.S
+00014920: 4d41 2864 6174 612e 6865 6164 286c 656e  MA(data.head(len
+00014930: 2864 6174 6129 2d31 3030 295b 2243 6c6f  (data)-100)["Clo
+00014940: 7365 225d 2c20 7469 6d65 7065 7269 6f64  se"], timeperiod
+00014950: 3d32 3030 290d 0a20 2020 2020 2020 2020  =200)..         
+00014960: 2020 2020 2020 2074 6f64 6179 5f6c 6d61         today_lma
+00014970: 203d 2074 6f64 6179 5f6c 6d61 2e69 6c6f   = today_lma.ilo
+00014980: 635b 6c65 6e28 746f 6461 795f 6c6d 6129  c[len(today_lma)
+00014990: 2d31 5d20 6966 2074 6f64 6179 5f6c 6d61  -1] if today_lma
+000149a0: 2069 7320 6e6f 7420 4e6f 6e65 2065 6c73   is not None els
+000149b0: 6520 300d 0a20 2020 2020 2020 2020 2020  e 0..           
+000149c0: 2020 2020 206c 6d61 5f6d 696e 7573 3230       lma_minus20
+000149d0: 203d 206c 6d61 5f6d 696e 7573 3230 2e69   = lma_minus20.i
+000149e0: 6c6f 635b 6c65 6e28 6c6d 615f 6d69 6e75  loc[len(lma_minu
+000149f0: 7332 3029 2d31 5d20 6966 206c 6d61 5f6d  s20)-1] if lma_m
+00014a00: 696e 7573 3230 2069 7320 6e6f 7420 4e6f  inus20 is not No
+00014a10: 6e65 2065 6c73 6520 300d 0a20 2020 2020  ne else 0..     
+00014a20: 2020 2020 2020 2020 2020 206c 6d61 5f6d             lma_m
+00014a30: 696e 7573 3830 203d 206c 6d61 5f6d 696e  inus80 = lma_min
+00014a40: 7573 3830 2e69 6c6f 635b 6c65 6e28 6c6d  us80.iloc[len(lm
+00014a50: 615f 6d69 6e75 7338 3029 2d31 5d20 6966  a_minus80)-1] if
+00014a60: 206c 6d61 5f6d 696e 7573 3830 2069 7320   lma_minus80 is 
+00014a70: 6e6f 7420 4e6f 6e65 2065 6c73 6520 300d  not None else 0.
+00014a80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014a90: 206c 6d61 5f6d 696e 7573 3130 3020 3d20   lma_minus100 = 
+00014aa0: 6c6d 615f 6d69 6e75 7331 3030 2e69 6c6f  lma_minus100.ilo
+00014ab0: 635b 6c65 6e28 6c6d 615f 6d69 6e75 7331  c[len(lma_minus1
+00014ac0: 3030 292d 315d 2069 6620 6c6d 615f 6d69  00)-1] if lma_mi
+00014ad0: 6e75 7331 3030 2069 7320 6e6f 7420 4e6f  nus100 is not No
+00014ae0: 6e65 2065 6c73 6520 300d 0a20 2020 2020  ne else 0..     
+00014af0: 2020 2020 2020 2020 2020 2074 6f64 6179             today
+00014b00: 5f73 6d61 203d 2074 6f64 6179 5f73 6d61  _sma = today_sma
+00014b10: 2e69 6c6f 635b 6c65 6e28 746f 6461 795f  .iloc[len(today_
+00014b20: 736d 6129 2d31 5d20 6966 2074 6f64 6179  sma)-1] if today
+00014b30: 5f73 6d61 2069 7320 6e6f 7420 4e6f 6e65  _sma is not None
+00014b40: 2065 6c73 6520 300d 0a20 2020 2020 2020   else 0..       
+00014b50: 2020 2020 2020 2020 2073 6d61 5f6d 696e           sma_min
+00014b60: 7573 3920 3d20 736d 615f 6d69 6e75 7339  us9 = sma_minus9
+00014b70: 2e69 6c6f 635b 6c65 6e28 736d 615f 6d69  .iloc[len(sma_mi
+00014b80: 6e75 7339 292d 315d 2069 6620 736d 615f  nus9)-1] if sma_
+00014b90: 6d69 6e75 7339 2069 7320 6e6f 7420 4e6f  minus9 is not No
+00014ba0: 6e65 2065 6c73 6520 300d 0a20 2020 2020  ne else 0..     
+00014bb0: 2020 2020 2020 2020 2020 2073 6d61 5f6d             sma_m
+00014bc0: 696e 7573 3134 203d 2073 6d61 5f6d 696e  inus14 = sma_min
+00014bd0: 7573 3134 2e69 6c6f 635b 6c65 6e28 736d  us14.iloc[len(sm
+00014be0: 615f 6d69 6e75 7331 3429 2d31 5d20 6966  a_minus14)-1] if
+00014bf0: 2073 6d61 5f6d 696e 7573 3134 2069 7320   sma_minus14 is 
+00014c00: 6e6f 7420 4e6f 6e65 2065 6c73 6520 300d  not None else 0.
+00014c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014c20: 2073 6d61 5f6d 696e 7573 3230 203d 2073   sma_minus20 = s
+00014c30: 6d61 5f6d 696e 7573 3230 2e69 6c6f 635b  ma_minus20.iloc[
+00014c40: 6c65 6e28 736d 615f 6d69 6e75 7332 3029  len(sma_minus20)
+00014c50: 2d31 5d20 6966 2073 6d61 5f6d 696e 7573  -1] if sma_minus
+00014c60: 3230 2069 7320 6e6f 7420 4e6f 6e65 2065  20 is not None e
+00014c70: 6c73 6520 300d 0a20 2020 2020 2020 2020  lse 0..         
+00014c80: 2020 2020 2020 2069 7355 7074 7265 6e64         isUptrend
+00014c90: 203d 2028 746f 6461 795f 6c6d 6120 3e20   = (today_lma > 
+00014ca0: 6c6d 615f 6d69 6e75 7332 3029 206f 7220  lma_minus20) or 
+00014cb0: 2874 6f64 6179 5f6c 6d61 203e 206c 6d61  (today_lma > lma
+00014cc0: 5f6d 696e 7573 3830 2920 6f72 2028 746f  _minus80) or (to
+00014cd0: 6461 795f 6c6d 6120 3e20 6c6d 615f 6d69  day_lma > lma_mi
+00014ce0: 6e75 7331 3030 290d 0a20 2020 2020 2020  nus100)..       
+00014cf0: 2020 2020 2020 2020 2069 7344 6f77 6e74           isDownt
+00014d00: 7265 6e64 203d 2028 746f 6461 795f 6c6d  rend = (today_lm
+00014d10: 6120 3c20 6c6d 615f 6d69 6e75 7332 3029  a < lma_minus20)
+00014d20: 2061 6e64 2028 746f 6461 795f 6c6d 6120   and (today_lma 
+00014d30: 3c20 6c6d 615f 6d69 6e75 7338 3029 2061  < lma_minus80) a
+00014d40: 6e64 2028 746f 6461 795f 6c6d 6120 3c20  nd (today_lma < 
+00014d50: 6c6d 615f 6d69 6e75 7331 3030 290d 0a20  lma_minus100).. 
+00014d60: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00014d70: 7335 3044 4d41 5570 7472 656e 6420 3d20  s50DMAUptrend = 
+00014d80: 2874 6f64 6179 5f73 6d61 203e 2073 6d61  (today_sma > sma
+00014d90: 5f6d 696e 7573 3929 206f 7220 2874 6f64  _minus9) or (tod
+00014da0: 6179 5f73 6d61 203e 2073 6d61 5f6d 696e  ay_sma > sma_min
+00014db0: 7573 3134 2920 6f72 2028 746f 6461 795f  us14) or (today_
+00014dc0: 736d 6120 3e20 736d 615f 6d69 6e75 7332  sma > sma_minus2
+00014dd0: 3029 0d0a 2020 2020 2020 2020 2020 2020  0)..            
+00014de0: 2020 2020 6973 3530 444d 4144 6f77 6e74      is50DMADownt
+00014df0: 7265 6e64 203d 2028 746f 6461 795f 736d  rend = (today_sm
+00014e00: 6120 3c20 736d 615f 6d69 6e75 7339 2920  a < sma_minus9) 
+00014e10: 616e 6420 2874 6f64 6179 5f73 6d61 203c  and (today_sma <
+00014e20: 2073 6d61 5f6d 696e 7573 3134 2920 616e   sma_minus14) an
+00014e30: 6420 2874 6f64 6179 5f73 6d61 203c 2073  d (today_sma < s
+00014e40: 6d61 5f6d 696e 7573 3230 290d 0a20 2020  ma_minus20)..   
+00014e50: 2020 2020 2020 2020 2065 7863 6570 7420           except 
+00014e60: 4578 6365 7074 696f 6e3a 2020 2320 7072  Exception:  # pr
+00014e70: 6167 6d61 3a20 6e6f 2063 6f76 6572 0d0a  agma: no cover..
+00014e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014e90: 2320 7365 6c66 2e64 6566 6175 6c74 5f6c  # self.default_l
+00014ea0: 6f67 6765 722e 6465 6275 6728 652c 2065  ogger.debug(e, e
+00014eb0: 7863 5f69 6e66 6f3d 5472 7565 290d 0a20  xc_info=True).. 
+00014ec0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00014ed0: 6173 730d 0a20 2020 2020 2020 2064 6563  ass..        dec
+00014ee0: 6973 696f 6e20 3d20 2754 3ae2 96b2 2720  ision = 'T:...' 
+00014ef0: 6966 2069 7355 7074 7265 6e64 2065 6c73  if isUptrend els
+00014f00: 6520 2827 543a e296 bc27 2069 6620 6973  e ('T:...' if is
+00014f10: 446f 776e 7472 656e 6420 656c 7365 2027  Downtrend else '
+00014f20: 2729 0d0a 2020 2020 2020 2020 646d 6135  ')..        dma5
+00014f30: 3064 6563 6973 696f 6e20 3d20 2774 3ae2  0decision = 't:.
+00014f40: 96b2 2720 6966 2069 7335 3044 4d41 5570  ..' if is50DMAUp
+00014f50: 7472 656e 6420 656c 7365 2028 2774 3ae2  trend else ('t:.
+00014f60: 96bc 2720 6966 2069 7335 3044 4d41 446f  ..' if is50DMADo
+00014f70: 776e 7472 656e 6420 656c 7365 2027 2729  wntrend else '')
+00014f80: 0d0a 2020 2020 2020 2020 6d66 5f69 6e73  ..        mf_ins
+00014f90: 745f 6f77 6e65 7273 6869 7043 6861 6e67  t_ownershipChang
+00014fa0: 6520 3d20 300d 0a20 2020 2020 2020 2063  e = 0..        c
+00014fb0: 6861 6e67 655f 6d69 6c6c 696f 6e73 203d  hange_millions =
+00014fc0: 2222 0d0a 2020 2020 2020 2020 7472 793a  ""..        try:
+00014fd0: 0d0a 2020 2020 2020 2020 2020 2020 6d66  ..            mf
+00014fe0: 5f69 6e73 745f 6f77 6e65 7273 6869 7043  _inst_ownershipC
+00014ff0: 6861 6e67 6520 3d20 7365 6c66 2e67 6574  hange = self.get
+00015000: 4d75 7475 616c 4675 6e64 5374 6174 7573  MutualFundStatus
+00015010: 2873 746f 636b 2c6f 6e6c 794d 463d 6f6e  (stock,onlyMF=on
+00015020: 6c79 4d46 2c68 6f73 7444 6174 613d 686f  lyMF,hostData=ho
+00015030: 7374 4461 7461 2c66 6f72 6365 3d28 686f  stData,force=(ho
+00015040: 7374 4461 7461 2069 7320 4e6f 6e65 206f  stData is None o
+00015050: 7220 686f 7374 4461 7461 2e65 6d70 7479  r hostData.empty
+00015060: 206f 7220 6e6f 7420 2822 4d46 2220 696e   or not ("MF" in
+00015070: 2068 6f73 7444 6174 612e 636f 6c75 6d6e   hostData.column
+00015080: 7320 6f72 2022 4649 4922 2069 6e20 686f  s or "FII" in ho
+00015090: 7374 4461 7461 2e63 6f6c 756d 6e73 2929  stData.columns))
+000150a0: 2c65 7863 6861 6e67 654e 616d 653d 6578  ,exchangeName=ex
+000150b0: 6368 616e 6765 4e61 6d65 290d 0a20 2020  changeName)..   
+000150c0: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
+000150d0: 7374 616e 6365 286d 665f 696e 7374 5f6f  stance(mf_inst_o
+000150e0: 776e 6572 7368 6970 4368 616e 6765 2c20  wnershipChange, 
+000150f0: 7064 2e53 6572 6965 7329 3a0d 0a20 2020  pd.Series):..   
+00015100: 2020 2020 2020 2020 2020 2020 206d 665f               mf_
+00015110: 696e 7374 5f6f 776e 6572 7368 6970 4368  inst_ownershipCh
+00015120: 616e 6765 203d 2030 0d0a 2020 2020 2020  ange = 0..      
+00015130: 2020 2020 2020 726f 756e 644f 6666 203d        roundOff =
+00015140: 2032 0d0a 2020 2020 2020 2020 2020 2020   2..            
+00015150: 6d69 6c6c 696f 6e73 203d 2072 6f75 6e64  millions = round
+00015160: 286d 665f 696e 7374 5f6f 776e 6572 7368  (mf_inst_ownersh
+00015170: 6970 4368 616e 6765 2f31 3030 3030 3030  ipChange/1000000
+00015180: 2c72 6f75 6e64 4f66 6629 0d0a 2020 2020  ,roundOff)..    
+00015190: 2020 2020 2020 2020 7768 696c 6520 666c          while fl
+000151a0: 6f61 7428 6d69 6c6c 696f 6e73 2920 3d3d  oat(millions) ==
+000151b0: 2030 2061 6e64 2072 6f75 6e64 4f66 6620   0 and roundOff 
+000151c0: 3c3d 353a 0d0a 2020 2020 2020 2020 2020  <=5:..          
+000151d0: 2020 2020 2020 726f 756e 644f 6666 202b        roundOff +
+000151e0: 3d31 0d0a 2020 2020 2020 2020 2020 2020  =1..            
+000151f0: 2020 2020 6d69 6c6c 696f 6e73 203d 2072      millions = r
+00015200: 6f75 6e64 286d 665f 696e 7374 5f6f 776e  ound(mf_inst_own
+00015210: 6572 7368 6970 4368 616e 6765 2f31 3030  ershipChange/100
+00015220: 3030 3030 2c72 6f75 6e64 4f66 6629 0d0a  0000,roundOff)..
+00015230: 2020 2020 2020 2020 2020 2020 6368 616e              chan
+00015240: 6765 5f6d 696c 6c69 6f6e 7320 3d20 6622  ge_millions = f"
+00015250: 287b 6d69 6c6c 696f 6e73 7d4d 2922 0d0a  ({millions}M)"..
+00015260: 2020 2020 2020 2020 6578 6365 7074 2045          except E
+00015270: 7863 6570 7469 6f6e 2061 7320 653a 2020  xception as e:  
+00015280: 2320 7072 6167 6d61 3a20 6e6f 2063 6f76  # pragma: no cov
+00015290: 6572 0d0a 2020 2020 2020 2020 2020 2020  er..            
+000152a0: 7365 6c66 2e64 6566 6175 6c74 5f6c 6f67  self.default_log
+000152b0: 6765 722e 6465 6275 6728 652c 2065 7863  ger.debug(e, exc
+000152c0: 5f69 6e66 6f3d 5472 7565 290d 0a20 2020  _info=True)..   
+000152d0: 2020 2020 2020 2020 2070 6173 730d 0a20           pass.. 
+000152e0: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
+000152f0: 2020 2020 2020 2020 2023 4c65 7427 7320           #Let's 
+00015300: 6765 7420 7468 6520 6661 6972 2076 616c  get the fair val
+00015310: 7565 2c20 6569 7468 6572 2073 6176 6564  ue, either saved
+00015320: 206f 7220 6672 6573 6820 6672 6f6d 2073   or fresh from s
+00015330: 6572 7669 6365 0d0a 2020 2020 2020 2020  ervice..        
+00015340: 2020 2020 6661 6972 5661 6c75 6520 3d20      fairValue = 
+00015350: 7365 6c66 2e67 6574 4661 6972 5661 6c75  self.getFairValu
+00015360: 6528 7374 6f63 6b2c 686f 7374 4461 7461  e(stock,hostData
+00015370: 2c66 6f72 6365 3d28 686f 7374 4461 7461  ,force=(hostData
+00015380: 2069 7320 4e6f 6e65 206f 7220 686f 7374   is None or host
+00015390: 4461 7461 2e65 6d70 7479 206f 7220 2246  Data.empty or "F
+000153a0: 6169 7256 616c 7565 2220 6e6f 7420 696e  airValue" not in
+000153b0: 2068 6f73 7444 6174 612e 636f 6c75 6d6e   hostData.column
+000153c0: 7329 2c65 7863 6861 6e67 654e 616d 653d  s),exchangeName=
+000153d0: 6578 6368 616e 6765 4e61 6d65 290d 0a20  exchangeName).. 
+000153e0: 2020 2020 2020 2020 2020 2069 6620 6661             if fa
+000153f0: 6972 5661 6c75 6520 6973 206e 6f74 204e  irValue is not N
+00015400: 6f6e 6520 616e 6420 6661 6972 5661 6c75  one and fairValu
+00015410: 6520 213d 2030 3a0d 0a20 2020 2020 2020  e != 0:..       
+00015420: 2020 2020 2020 2020 206c 7470 203d 2073           ltp = s
+00015430: 6176 6544 6963 745b 224c 5450 225d 0d0a  aveDict["LTP"]..
+00015440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015450: 6661 6972 5661 6c75 6544 6966 6620 3d20  fairValueDiff = 
+00015460: 726f 756e 6428 6661 6972 5661 6c75 6520  round(fairValue 
+00015470: 2d20 6c74 702c 3029 0d0a 2020 2020 2020  - ltp,0)..      
+00015480: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
+00015490: 6374 5b22 4661 6972 5661 6c75 6522 5d20  ct["FairValue"] 
+000154a0: 3d20 7374 7228 6661 6972 5661 6c75 6529  = str(fairValue)
+000154b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000154c0: 2020 7361 7665 4469 6374 5b22 4656 4469    saveDict["FVDi
+000154d0: 6666 225d 203d 2066 6169 7256 616c 7565  ff"] = fairValue
+000154e0: 4469 6666 0d0a 2020 2020 2020 2020 2020  Diff..          
+000154f0: 2020 2020 2020 7363 7265 656e 4469 6374        screenDict
+00015500: 5b22 4656 4469 6666 225d 203d 2066 6169  ["FVDiff"] = fai
+00015510: 7256 616c 7565 4469 6666 0d0a 2020 2020  rValueDiff..    
+00015520: 2020 2020 2020 2020 2020 2020 7363 7265              scre
+00015530: 656e 4469 6374 5b22 4661 6972 5661 6c75  enDict["FairValu
+00015540: 6522 5d20 3d20 2863 6f6c 6f72 5465 7874  e"] = (colorText
+00015550: 2e47 5245 454e 2069 6620 6661 6972 5661  .GREEN if fairVa
+00015560: 6c75 6520 3e3d 206c 7470 2065 6c73 6520  lue >= ltp else 
+00015570: 636f 6c6f 7254 6578 742e 4641 494c 2920  colorText.FAIL) 
+00015580: 2b20 7361 7665 4469 6374 5b22 4661 6972  + saveDict["Fair
+00015590: 5661 6c75 6522 5d20 2b20 636f 6c6f 7254  Value"] + colorT
+000155a0: 6578 742e 454e 440d 0a20 2020 2020 2020  ext.END..       
+000155b0: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+000155c0: 6e20 6173 2065 3a20 2023 2070 7261 676d  n as e:  # pragm
+000155d0: 613a 206e 6f20 636f 7665 720d 0a20 2020  a: no cover..   
+000155e0: 2020 2020 2020 2020 2073 656c 662e 6465           self.de
+000155f0: 6661 756c 745f 6c6f 6767 6572 2e64 6562  fault_logger.deb
+00015600: 7567 2865 2c20 6578 635f 696e 666f 3d54  ug(e, exc_info=T
+00015610: 7275 6529 0d0a 2020 2020 2020 2020 2020  rue)..          
+00015620: 2020 7061 7373 0d0a 2020 2020 2020 2020    pass..        
+00015630: 6d66 203d 2022 220d 0a20 2020 2020 2020  mf = ""..       
+00015640: 206d 6673 203d 2022 220d 0a20 2020 2020   mfs = ""..     
+00015650: 2020 2069 6620 6d66 5f69 6e73 745f 6f77     if mf_inst_ow
+00015660: 6e65 7273 6869 7043 6861 6e67 6520 3e20  nershipChange > 
+00015670: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
+00015680: 6d66 203d 2066 224d 4649 3ae2 96b2 207b  mf = f"MFI:... {
+00015690: 6368 616e 6765 5f6d 696c 6c69 6f6e 737d  change_millions}
+000156a0: 220d 0a20 2020 2020 2020 2020 2020 206d  "..            m
+000156b0: 6673 203d 2063 6f6c 6f72 5465 7874 2e47  fs = colorText.G
+000156c0: 5245 454e 202b 206d 6620 2b20 636f 6c6f  REEN + mf + colo
+000156d0: 7254 6578 742e 454e 440d 0a20 2020 2020  rText.END..     
+000156e0: 2020 2065 6c69 6620 6d66 5f69 6e73 745f     elif mf_inst_
+000156f0: 6f77 6e65 7273 6869 7043 6861 6e67 6520  ownershipChange 
+00015700: 3c20 303a 0d0a 2020 2020 2020 2020 2020  < 0:..          
+00015710: 2020 6d66 203d 2066 224d 4649 3ae2 96bc    mf = f"MFI:...
+00015720: 207b 6368 616e 6765 5f6d 696c 6c69 6f6e   {change_million
+00015730: 737d 220d 0a20 2020 2020 2020 2020 2020  s}"..           
+00015740: 206d 6673 203d 2063 6f6c 6f72 5465 7874   mfs = colorText
+00015750: 2e46 4149 4c20 2b20 6d66 202b 2063 6f6c  .FAIL + mf + col
+00015760: 6f72 5465 7874 2e45 4e44 0d0a 0d0a 2020  orText.END....  
+00015770: 2020 2020 2020 7361 7665 6420 3d20 7365        saved = se
+00015780: 6c66 2e66 696e 6443 7572 7265 6e74 5361  lf.findCurrentSa
+00015790: 7665 6456 616c 7565 2873 6372 6565 6e44  vedValue(screenD
+000157a0: 6963 742c 7361 7665 4469 6374 2c22 5472  ict,saveDict,"Tr
+000157b0: 656e 6422 290d 0a20 2020 2020 2020 2064  end")..        d
+000157c0: 6563 6973 696f 6e5f 7363 7220 3d20 2863  ecision_scr = (c
+000157d0: 6f6c 6f72 5465 7874 2e47 5245 454e 2069  olorText.GREEN i
+000157e0: 6620 6973 5570 7472 656e 6420 656c 7365  f isUptrend else
+000157f0: 2028 636f 6c6f 7254 6578 742e 4641 494c   (colorText.FAIL
+00015800: 2069 6620 6973 446f 776e 7472 656e 6420   if isDowntrend 
+00015810: 656c 7365 2063 6f6c 6f72 5465 7874 2e57  else colorText.W
+00015820: 4152 4e29 2920 2b20 6622 7b64 6563 6973  ARN)) + f"{decis
+00015830: 696f 6e7d 2220 2b20 636f 6c6f 7254 6578  ion}" + colorTex
+00015840: 742e 454e 440d 0a20 2020 2020 2020 2064  t.END..        d
+00015850: 6d61 3530 6465 6369 7369 6f6e 5f73 6372  ma50decision_scr
+00015860: 203d 2028 636f 6c6f 7254 6578 742e 4752   = (colorText.GR
+00015870: 4545 4e20 6966 2069 7335 3044 4d41 5570  EEN if is50DMAUp
+00015880: 7472 656e 6420 656c 7365 2028 636f 6c6f  trend else (colo
+00015890: 7254 6578 742e 4641 494c 2069 6620 6973  rText.FAIL if is
+000158a0: 3530 444d 4144 6f77 6e74 7265 6e64 2065  50DMADowntrend e
+000158b0: 6c73 6520 636f 6c6f 7254 6578 742e 5741  lse colorText.WA
+000158c0: 524e 2929 202b 2066 227b 646d 6135 3064  RN)) + f"{dma50d
+000158d0: 6563 6973 696f 6e7d 2220 2b20 636f 6c6f  ecision}" + colo
+000158e0: 7254 6578 742e 454e 440d 0a20 2020 2020  rText.END..     
+000158f0: 2020 2073 6176 6544 6963 745b 2254 7265     saveDict["Tre
+00015900: 6e64 225d 203d 2066 227b 7361 7665 645b  nd"] = f"{saved[
+00015910: 315d 7d20 7b64 6563 6973 696f 6e7d 207b  1]} {decision} {
+00015920: 646d 6135 3064 6563 6973 696f 6e7d 207b  dma50decision} {
+00015930: 6d66 7d22 0d0a 2020 2020 2020 2020 7363  mf}"..        sc
+00015940: 7265 656e 4469 6374 5b22 5472 656e 6422  reenDict["Trend"
+00015950: 5d20 3d20 6622 7b73 6176 6564 5b30 5d7d  ] = f"{saved[0]}
+00015960: 207b 6465 6369 7369 6f6e 5f73 6372 7d20   {decision_scr} 
+00015970: 7b64 6d61 3530 6465 6369 7369 6f6e 5f73  {dma50decision_s
+00015980: 6372 7d20 7b6d 6673 7d22 0d0a 2020 2020  cr} {mfs}"..    
+00015990: 2020 2020 7361 7665 4469 6374 5b22 4d46      saveDict["MF
+000159a0: 4922 5d20 3d20 6d66 5f69 6e73 745f 6f77  I"] = mf_inst_ow
+000159b0: 6e65 7273 6869 7043 6861 6e67 650d 0a20  nershipChange.. 
+000159c0: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
+000159d0: 745b 224d 4649 225d 203d 206d 665f 696e  t["MFI"] = mf_in
+000159e0: 7374 5f6f 776e 6572 7368 6970 4368 616e  st_ownershipChan
+000159f0: 6765 0d0a 2020 2020 2020 2020 7265 7475  ge..        retu
+00015a00: 726e 2069 7355 7074 7265 6e64 2c20 6d66  rn isUptrend, mf
+00015a10: 5f69 6e73 745f 6f77 6e65 7273 6869 7043  _inst_ownershipC
+00015a20: 6861 6e67 652c 2066 6169 7256 616c 7565  hange, fairValue
+00015a30: 4469 6666 0d0a 2020 2020 0d0a 2020 2020  Diff..    ..    
+00015a40: 2320 5072 6976 6174 6520 6d65 7468 6f64  # Private method
+00015a50: 2074 6f20 6669 6e64 2063 616e 646c 6520   to find candle 
+00015a60: 7479 7065 0d0a 2020 2020 2320 5472 7565  type..    # True
+00015a70: 203d 2042 756c 6c69 7368 2c20 4661 6c73   = Bullish, Fals
+00015a80: 6520 3d20 4265 6172 6973 680d 0a20 2020  e = Bearish..   
+00015a90: 2064 6566 2067 6574 4361 6e64 6c65 5479   def getCandleTy
+00015aa0: 7065 2873 656c 662c 2064 6169 6c79 4461  pe(self, dailyDa
+00015ab0: 7461 293a 0d0a 2020 2020 2020 2020 7265  ta):..        re
+00015ac0: 7475 726e 2062 6f6f 6c28 6461 696c 7944  turn bool(dailyD
+00015ad0: 6174 615b 2243 6c6f 7365 225d 2e69 6c6f  ata["Close"].ilo
+00015ae0: 635b 305d 203e 3d20 6461 696c 7944 6174  c[0] >= dailyDat
+00015af0: 615b 224f 7065 6e22 5d2e 696c 6f63 5b30  a["Open"].iloc[0
+00015b00: 5d29 0d0a 0d0a 2020 2020 6465 6620 6765  ])....    def ge
+00015b10: 7443 616e 646c 6542 6f64 7948 6569 6768  tCandleBodyHeigh
+00015b20: 7428 7365 6c66 2c20 6461 696c 7944 6174  t(self, dailyDat
+00015b30: 6129 3a0d 0a20 2020 2020 2020 2062 6f64  a):..        bod
+00015b40: 7948 6569 6768 7420 3d20 6461 696c 7944  yHeight = dailyD
+00015b50: 6174 615b 2243 6c6f 7365 225d 2e69 6c6f  ata["Close"].ilo
+00015b60: 635b 305d 202d 2064 6169 6c79 4461 7461  c[0] - dailyData
+00015b70: 5b22 4f70 656e 225d 2e69 6c6f 635b 305d  ["Open"].iloc[0]
+00015b80: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00015b90: 2062 6f64 7948 6569 6768 740d 0a0d 0a20   bodyHeight.... 
+00015ba0: 2020 2064 6566 2067 6574 4661 6972 5661     def getFairVa
+00015bb0: 6c75 6528 7365 6c66 2c20 7374 6f63 6b2c  lue(self, stock,
+00015bc0: 2068 6f73 7444 6174 613d 4e6f 6e65 2c20   hostData=None, 
+00015bd0: 666f 7263 653d 4661 6c73 652c 6578 6368  force=False,exch
+00015be0: 616e 6765 4e61 6d65 3d22 494e 4449 4122  angeName="INDIA"
+00015bf0: 293a 0d0a 2020 2020 2020 2020 6966 2068  ):..        if h
+00015c00: 6f73 7444 6174 6120 6973 204e 6f6e 6520  ostData is None 
+00015c10: 6f72 206c 656e 2868 6f73 7444 6174 6129  or len(hostData)
+00015c20: 203c 2031 3a0d 0a20 2020 2020 2020 2020   < 1:..         
+00015c30: 2020 2068 6f73 7444 6174 6120 3d20 7064     hostData = pd
+00015c40: 2e44 6174 6146 7261 6d65 2829 0d0a 2020  .DataFrame()..  
+00015c50: 2020 2020 2020 2320 4c65 7427 7320 6c6f        # Let's lo
+00015c60: 6f6b 2066 6f72 2066 6169 7220 7661 6c75  ok for fair valu
+00015c70: 6573 0d0a 2020 2020 2020 2020 6661 6972  es..        fair
+00015c80: 5661 6c75 6520 3d20 300d 0a20 2020 2020  Value = 0..     
+00015c90: 2020 2069 6620 2246 6169 7256 616c 7565     if "FairValue
+00015ca0: 2220 696e 2068 6f73 7444 6174 612e 636f  " in hostData.co
+00015cb0: 6c75 6d6e 7320 616e 6420 504b 4461 7465  lumns and PKDate
+00015cc0: 5574 696c 6974 6965 732e 6375 7272 656e  Utilities.curren
+00015cd0: 7444 6174 6554 696d 6528 292e 7765 656b  tDateTime().week
+00015ce0: 6461 7928 2920 3c3d 2034 3a0d 0a20 2020  day() <= 4:..   
+00015cf0: 2020 2020 2020 2020 2074 7279 3a0d 0a20           try:.. 
+00015d00: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00015d10: 6169 7256 616c 7565 203d 2068 6f73 7444  airValue = hostD
+00015d20: 6174 612e 6c6f 635b 686f 7374 4461 7461  ata.loc[hostData
+00015d30: 2e69 6e64 6578 5b2d 315d 2c22 4661 6972  .index[-1],"Fair
+00015d40: 5661 6c75 6522 5d0d 0a20 2020 2020 2020  Value"]..       
+00015d50: 2020 2020 2065 7863 6570 7420 284b 6579       except (Key
+00015d60: 4572 726f 722c 496e 6465 7845 7272 6f72  Error,IndexError
+00015d70: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00015d80: 2020 2020 2020 2020 7061 7373 0d0a 2020          pass..  
+00015d90: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+00015da0: 2020 2020 2020 2020 2069 6620 504b 4461           if PKDa
+00015db0: 7465 5574 696c 6974 6965 732e 6375 7272  teUtilities.curr
+00015dc0: 656e 7444 6174 6554 696d 6528 292e 7765  entDateTime().we
+00015dd0: 656b 6461 7928 2920 3e3d 2035 206f 7220  ekday() >= 5 or 
+00015de0: 666f 7263 653a 0d0a 2020 2020 2020 2020  force:..        
+00015df0: 2020 2020 2020 2020 7365 6375 7269 7479          security
+00015e00: 203d 204e 6f6e 650d 0a20 2020 2020 2020   = None..       
+00015e10: 2020 2020 2020 2020 2023 2052 6566 7265           # Refre
+00015e20: 7368 2065 6163 6820 7361 7475 7264 6179  sh each saturday
+00015e30: 206f 7220 7375 6e64 6179 206f 7220 7768   or sunday or wh
+00015e40: 656e 206e 6f74 2066 6f75 6e64 2069 6e20  en not found in 
+00015e50: 7361 7665 6420 6461 7461 0d0a 2020 2020  saved data..    
+00015e60: 2020 2020 2020 2020 2020 2020 7472 793a              try:
+00015e70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015e80: 2020 2020 2020 7769 7468 2053 7570 7072        with Suppr
+00015e90: 6573 734f 7574 7075 7428 7375 7070 7265  essOutput(suppre
+00015ea0: 7373 5f73 7464 6572 723d 5472 7565 2c20  ss_stderr=True, 
+00015eb0: 7375 7070 7265 7373 5f73 7464 6f75 743d  suppress_stdout=
+00015ec0: 5472 7565 293a 0d0a 2020 2020 2020 2020  True):..        
+00015ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015ee0: 7365 6375 7269 7479 203d 2053 746f 636b  security = Stock
+00015ef0: 2873 746f 636b 2c65 7863 6861 6e67 653d  (stock,exchange=
+00015f00: 6578 6368 616e 6765 4e61 6d65 290d 0a20  exchangeName).. 
+00015f10: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00015f20: 7863 6570 7420 5661 6c75 6545 7272 6f72  xcept ValueError
+00015f30: 3a20 2320 7072 6167 6d61 3a20 6e6f 2063  : # pragma: no c
+00015f40: 6f76 6572 0d0a 2020 2020 2020 2020 2020  over..          
+00015f50: 2020 2020 2020 2020 2020 2320 5765 2064            # We d
+00015f60: 6964 206e 6f74 2066 696e 6420 7468 6520  id not find the 
+00015f70: 7374 6f63 6b3f 2049 7427 7320 6f6b 6179  stock? It's okay
+00015f80: 2e20 4d6f 7665 206f 6e20 746f 2074 6865  . Move on to the
+00015f90: 206e 6578 7420 6f6e 652e 0d0a 2020 2020   next one...    
+00015fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015fb0: 7061 7373 0d0a 2020 2020 2020 2020 2020  pass..          
+00015fc0: 2020 2020 2020 6966 2073 6563 7572 6974        if securit
+00015fd0: 7920 6973 206e 6f74 204e 6f6e 653a 0d0a  y is not None:..
 00015fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015ff0: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
-00016000: 2020 2020 2020 2020 2020 2020 2020 686f                ho
-00016010: 7374 4461 7461 2e6c 6f63 5b68 6f73 7444  stData.loc[hostD
-00016020: 6174 612e 696e 6465 785b 2d31 5d2c 2246  ata.index[-1],"F
-00016030: 6169 7256 616c 7565 225d 203d 2066 6169  airValue"] = fai
-00016040: 7256 616c 7565 0d0a 2020 2020 2020 2020  rValue..        
-00016050: 2020 2020 2020 2020 2020 2020 6578 6365              exce
-00016060: 7074 2028 4b65 7945 7272 6f72 2c49 6e64  pt (KeyError,Ind
-00016070: 6578 4572 726f 7229 3a0d 0a20 2020 2020  exError):..     
-00016080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016090: 2020 2070 6173 730d 0a20 2020 2020 2020     pass..       
-000160a0: 2072 6574 7572 6e20 6661 6972 5661 6c75   return fairValu
-000160b0: 650d 0a0d 0a20 2020 2064 6566 2067 6574  e....    def get
-000160c0: 4d75 7475 616c 4675 6e64 5374 6174 7573  MutualFundStatus
-000160d0: 2873 656c 662c 2073 746f 636b 2c6f 6e6c  (self, stock,onl
-000160e0: 794d 463d 4661 6c73 652c 2068 6f73 7444  yMF=False, hostD
-000160f0: 6174 613d 4e6f 6e65 2c20 666f 7263 653d  ata=None, force=
-00016100: 4661 6c73 652c 6578 6368 616e 6765 4e61  False,exchangeNa
-00016110: 6d65 3d22 494e 4449 4122 293a 0d0a 2020  me="INDIA"):..  
-00016120: 2020 2020 2020 6966 2068 6f73 7444 6174        if hostDat
-00016130: 6120 6973 204e 6f6e 6520 6f72 206c 656e  a is None or len
-00016140: 2868 6f73 7444 6174 6129 203c 2031 3a0d  (hostData) < 1:.
-00016150: 0a20 2020 2020 2020 2020 2020 2068 6f73  .            hos
-00016160: 7444 6174 6120 3d20 7064 2e44 6174 6146  tData = pd.DataF
-00016170: 7261 6d65 2829 0d0a 2020 2020 2020 2020  rame()..        
-00016180: 0d0a 2020 2020 2020 2020 6e65 7443 6861  ..        netCha
-00016190: 6e67 654d 4620 3d20 300d 0a20 2020 2020  ngeMF = 0..     
-000161a0: 2020 206e 6574 4368 616e 6765 496e 7374     netChangeInst
-000161b0: 203d 2030 0d0a 2020 2020 2020 2020 6c61   = 0..        la
-000161c0: 7465 7374 5f6d 6664 6174 6520 3d20 4e6f  test_mfdate = No
-000161d0: 6e65 0d0a 2020 2020 2020 2020 6c61 7465  ne..        late
-000161e0: 7374 5f69 6e73 7464 6174 6520 3d20 4e6f  st_instdate = No
-000161f0: 6e65 0d0a 2020 2020 2020 2020 6e65 6564  ne..        need
-00016200: 7346 7265 7368 5570 6461 7465 203d 2054  sFreshUpdate = T
-00016210: 7275 650d 0a20 2020 2020 2020 206c 6173  rue..        las
-00016220: 7444 6179 4c61 7374 4d6f 6e74 6820 3d20  tDayLastMonth = 
-00016230: 504b 4461 7465 5574 696c 6974 6965 732e  PKDateUtilities.
-00016240: 6c61 7374 5f64 6179 5f6f 665f 7072 6576  last_day_of_prev
-00016250: 696f 7573 5f6d 6f6e 7468 2850 4b44 6174  ious_month(PKDat
-00016260: 6555 7469 6c69 7469 6573 2e63 7572 7265  eUtilities.curre
-00016270: 6e74 4461 7465 5469 6d65 2829 290d 0a20  ntDateTime()).. 
-00016280: 2020 2020 2020 2069 6620 686f 7374 4461         if hostDa
-00016290: 7461 2069 7320 6e6f 7420 4e6f 6e65 2061  ta is not None a
-000162a0: 6e64 206c 656e 2868 6f73 7444 6174 6129  nd len(hostData)
-000162b0: 203e 2030 3a0d 0a20 2020 2020 2020 2020   > 0:..         
-000162c0: 2020 2069 6620 224d 4622 2069 6e20 686f     if "MF" in ho
-000162d0: 7374 4461 7461 2e63 6f6c 756d 6e73 206f  stData.columns o
-000162e0: 7220 2246 4949 2220 696e 2068 6f73 7444  r "FII" in hostD
-000162f0: 6174 612e 636f 6c75 6d6e 733a 0d0a 2020  ata.columns:..  
-00016300: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-00016310: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
-00016320: 2020 2020 2020 2020 6e65 7443 6861 6e67          netChang
-00016330: 654d 4620 3d20 686f 7374 4461 7461 2e6c  eMF = hostData.l
-00016340: 6f63 5b68 6f73 7444 6174 612e 696e 6465  oc[hostData.inde
-00016350: 785b 2d31 5d2c 224d 4622 5d0d 0a20 2020  x[-1],"MF"]..   
-00016360: 2020 2020 2020 2020 2020 2020 2065 7863               exc
-00016370: 6570 7420 284b 6579 4572 726f 722c 496e  ept (KeyError,In
-00016380: 6465 7845 7272 6f72 293a 0d0a 2020 2020  dexError):..    
-00016390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000163a0: 7061 7373 0d0a 2020 2020 2020 2020 2020  pass..          
-000163b0: 2020 2020 2020 7472 793a 0d0a 2020 2020        try:..    
-000163c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000163d0: 6e65 7443 6861 6e67 6549 6e73 7420 3d20  netChangeInst = 
-000163e0: 686f 7374 4461 7461 2e6c 6f63 5b68 6f73  hostData.loc[hos
-000163f0: 7444 6174 612e 696e 6465 785b 2d31 5d2c  tData.index[-1],
-00016400: 2246 4949 225d 0d0a 2020 2020 2020 2020  "FII"]..        
-00016410: 2020 2020 2020 2020 6578 6365 7074 2028          except (
-00016420: 4b65 7945 7272 6f72 2c49 6e64 6578 4572  KeyError,IndexEr
-00016430: 726f 7229 3a0d 0a20 2020 2020 2020 2020  ror):..         
-00016440: 2020 2020 2020 2020 2020 2070 6173 730d             pass.
-00016450: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016460: 2074 7279 3a0d 0a20 2020 2020 2020 2020   try:..         
-00016470: 2020 2020 2020 2020 2020 206c 6174 6573             lates
-00016480: 745f 6d66 6461 7465 203d 2068 6f73 7444  t_mfdate = hostD
-00016490: 6174 612e 6c6f 635b 686f 7374 4461 7461  ata.loc[hostData
-000164a0: 2e69 6e64 6578 5b2d 315d 2c22 4d46 5f44  .index[-1],"MF_D
-000164b0: 6174 6522 5d0d 0a20 2020 2020 2020 2020  ate"]..         
-000164c0: 2020 2020 2020 2065 7863 6570 7420 284b         except (K
-000164d0: 6579 4572 726f 722c 496e 6465 7845 7272  eyError,IndexErr
-000164e0: 6f72 293a 0d0a 2020 2020 2020 2020 2020  or):..          
-000164f0: 2020 2020 2020 2020 2020 7061 7373 0d0a            pass..
-00016500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016510: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
-00016520: 2020 2020 2020 2020 2020 6c61 7465 7374            latest
-00016530: 5f69 6e73 7464 6174 6520 3d20 686f 7374  _instdate = host
-00016540: 4461 7461 2e6c 6f63 5b68 6f73 7444 6174  Data.loc[hostDat
-00016550: 612e 696e 6465 785b 2d31 5d2c 2246 4949  a.index[-1],"FII
-00016560: 5f44 6174 6522 5d0d 0a20 2020 2020 2020  _Date"]..       
-00016570: 2020 2020 2020 2020 2065 7863 6570 7420           except 
-00016580: 284b 6579 4572 726f 722c 496e 6465 7845  (KeyError,IndexE
-00016590: 7272 6f72 293a 0d0a 2020 2020 2020 2020  rror):..        
-000165a0: 2020 2020 2020 2020 2020 2020 7061 7373              pass
-000165b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000165c0: 2020 6966 206c 6174 6573 745f 6d66 6461    if latest_mfda
-000165d0: 7465 2069 7320 6e6f 7420 4e6f 6e65 3a0d  te is not None:.
-000165e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000165f0: 2020 2020 2073 6176 6564 5f6d 6664 6174       saved_mfdat
-00016600: 6520 3d20 504b 4461 7465 5574 696c 6974  e = PKDateUtilit
-00016610: 6965 732e 6461 7465 4672 6f6d 596d 6453  ies.dateFromYmdS
-00016620: 7472 696e 6728 6c61 7465 7374 5f6d 6664  tring(latest_mfd
-00016630: 6174 652e 7370 6c69 7428 2254 2229 5b30  ate.split("T")[0
-00016640: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-00016650: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00016660: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00016670: 6176 6564 5f6d 6664 6174 6520 3d20 6c61  aved_mfdate = la
-00016680: 7374 4461 794c 6173 744d 6f6e 7468 202d  stDayLastMonth -
-00016690: 2064 6174 6574 696d 652e 7469 6d65 6465   datetime.timede
-000166a0: 6c74 6128 3129 0d0a 2020 2020 2020 2020  lta(1)..        
-000166b0: 2020 2020 2020 2020 6966 206c 6174 6573          if lates
-000166c0: 745f 696e 7374 6461 7465 2069 7320 6e6f  t_instdate is no
-000166d0: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
-000166e0: 2020 2020 2020 2020 2020 2020 2073 6176               sav
-000166f0: 6564 5f69 6e73 7464 6174 6520 3d20 504b  ed_instdate = PK
-00016700: 4461 7465 5574 696c 6974 6965 732e 6461  DateUtilities.da
-00016710: 7465 4672 6f6d 596d 6453 7472 696e 6728  teFromYmdString(
-00016720: 6c61 7465 7374 5f69 6e73 7464 6174 652e  latest_instdate.
-00016730: 7370 6c69 7428 2254 2229 5b30 5d29 0d0a  split("T")[0])..
-00016740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016750: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-00016760: 2020 2020 2020 2020 2020 2073 6176 6564             saved
-00016770: 5f69 6e73 7464 6174 6520 3d20 6c61 7374  _instdate = last
-00016780: 4461 794c 6173 744d 6f6e 7468 202d 2064  DayLastMonth - d
-00016790: 6174 6574 696d 652e 7469 6d65 6465 6c74  atetime.timedelt
-000167a0: 6128 3129 0d0a 2020 2020 2020 2020 2020  a(1)..          
-000167b0: 2020 2020 2020 746f 6461 7920 3d20 504b        today = PK
-000167c0: 4461 7465 5574 696c 6974 6965 732e 6375  DateUtilities.cu
-000167d0: 7272 656e 7444 6174 6554 696d 6528 290d  rrentDateTime().
-000167e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000167f0: 206e 6565 6473 4672 6573 6855 7064 6174   needsFreshUpdat
-00016800: 6520 3d20 2873 6176 6564 5f6d 6664 6174  e = (saved_mfdat
-00016810: 652e 6461 7465 2829 203c 206c 6173 7444  e.date() < lastD
-00016820: 6179 4c61 7374 4d6f 6e74 682e 6461 7465  ayLastMonth.date
-00016830: 2829 2920 616e 6420 2873 6176 6564 5f69  ()) and (saved_i
-00016840: 6e73 7464 6174 652e 6461 7465 2829 203c  nstdate.date() <
-00016850: 206c 6173 7444 6179 4c61 7374 4d6f 6e74   lastDayLastMont
-00016860: 682e 6461 7465 2829 290d 0a20 2020 2020  h.date())..     
-00016870: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-00016880: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
-00016890: 6564 7346 7265 7368 5570 6461 7465 203d  edsFreshUpdate =
-000168a0: 2054 7275 650d 0a0d 0a20 2020 2020 2020   True....       
-000168b0: 2069 6620 6e65 6564 7346 7265 7368 5570   if needsFreshUp
-000168c0: 6461 7465 2061 6e64 2066 6f72 6365 3a0d  date and force:.
-000168d0: 0a20 2020 2020 2020 2020 2020 206e 6574  .            net
-000168e0: 4368 616e 6765 4d46 2c20 6e65 7443 6861  ChangeMF, netCha
-000168f0: 6e67 6549 6e73 742c 206c 6174 6573 745f  ngeInst, latest_
-00016900: 6d66 6461 7465 2c20 6c61 7465 7374 5f69  mfdate, latest_i
-00016910: 6e73 7464 6174 6520 3d20 7365 6c66 2e67  nstdate = self.g
-00016920: 6574 4672 6573 684d 4649 5374 6174 7573  etFreshMFIStatus
-00016930: 2873 746f 636b 2c65 7863 6861 6e67 654e  (stock,exchangeN
-00016940: 616d 653d 6578 6368 616e 6765 4e61 6d65  ame=exchangeName
-00016950: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
-00016960: 6620 6e65 7443 6861 6e67 654d 4620 6973  f netChangeMF is
-00016970: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
-00016980: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-00016990: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000169a0: 2020 2020 2020 686f 7374 4461 7461 2e6c        hostData.l
-000169b0: 6f63 5b68 6f73 7444 6174 612e 696e 6465  oc[hostData.inde
-000169c0: 785b 2d31 5d2c 224d 4622 5d20 3d20 6e65  x[-1],"MF"] = ne
-000169d0: 7443 6861 6e67 654d 460d 0a20 2020 2020  tChangeMF..     
-000169e0: 2020 2020 2020 2020 2020 2065 7863 6570             excep
-000169f0: 7420 284b 6579 4572 726f 722c 496e 6465  t (KeyError,Inde
-00016a00: 7845 7272 6f72 293a 0d0a 2020 2020 2020  xError):..      
-00016a10: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-00016a20: 7373 0d0a 2020 2020 2020 2020 2020 2020  ss..            
-00016a30: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-00016a40: 2020 2020 2020 206e 6574 4368 616e 6765         netChange
-00016a50: 4d46 203d 2030 0d0a 2020 2020 2020 2020  MF = 0..        
-00016a60: 2020 2020 6966 206c 6174 6573 745f 6d66      if latest_mf
-00016a70: 6461 7465 2069 7320 6e6f 7420 4e6f 6e65  date is not None
-00016a80: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00016a90: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
-00016aa0: 2020 2020 2020 2020 2020 2020 2068 6f73               hos
-00016ab0: 7444 6174 612e 6c6f 635b 686f 7374 4461  tData.loc[hostDa
-00016ac0: 7461 2e69 6e64 6578 5b2d 315d 2c22 4d46  ta.index[-1],"MF
-00016ad0: 5f44 6174 6522 5d20 3d20 6c61 7465 7374  _Date"] = latest
-00016ae0: 5f6d 6664 6174 650d 0a20 2020 2020 2020  _mfdate..       
-00016af0: 2020 2020 2020 2020 2065 7863 6570 7420           except 
-00016b00: 284b 6579 4572 726f 722c 496e 6465 7845  (KeyError,IndexE
-00016b10: 7272 6f72 293a 0d0a 2020 2020 2020 2020  rror):..        
-00016b20: 2020 2020 2020 2020 2020 2020 7061 7373              pass
-00016b30: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00016b40: 206e 6574 4368 616e 6765 496e 7374 2069   netChangeInst i
-00016b50: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
-00016b60: 2020 2020 2020 2020 2020 2020 2074 7279               try
-00016b70: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00016b80: 2020 2020 2020 2068 6f73 7444 6174 612e         hostData.
-00016b90: 6c6f 635b 686f 7374 4461 7461 2e69 6e64  loc[hostData.ind
-00016ba0: 6578 5b2d 315d 2c22 4649 4922 5d20 3d20  ex[-1],"FII"] = 
-00016bb0: 6e65 7443 6861 6e67 6549 6e73 740d 0a20  netChangeInst.. 
-00016bc0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00016bd0: 7863 6570 7420 284b 6579 4572 726f 722c  xcept (KeyError,
-00016be0: 496e 6465 7845 7272 6f72 293a 0d0a 2020  IndexError):..  
-00016bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016c00: 2020 7061 7373 0d0a 2020 2020 2020 2020    pass..        
-00016c10: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00016c20: 2020 2020 2020 2020 2020 206e 6574 4368             netCh
-00016c30: 616e 6765 496e 7374 203d 2030 0d0a 2020  angeInst = 0..  
-00016c40: 2020 2020 2020 2020 2020 6966 206c 6174            if lat
-00016c50: 6573 745f 696e 7374 6461 7465 2069 7320  est_instdate is 
-00016c60: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
-00016c70: 2020 2020 2020 2020 2020 2074 7279 3a0d             try:.
-00016c80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016c90: 2020 2020 2068 6f73 7444 6174 612e 6c6f       hostData.lo
-00016ca0: 635b 686f 7374 4461 7461 2e69 6e64 6578  c[hostData.index
-00016cb0: 5b2d 315d 2c22 4649 495f 4461 7465 225d  [-1],"FII_Date"]
-00016cc0: 203d 206c 6174 6573 745f 696e 7374 6461   = latest_instda
-00016cd0: 7465 0d0a 2020 2020 2020 2020 2020 2020  te..            
-00016ce0: 2020 2020 6578 6365 7074 2028 4b65 7945      except (KeyE
-00016cf0: 7272 6f72 2c49 6e64 6578 4572 726f 7229  rror,IndexError)
-00016d00: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00016d10: 2020 2020 2020 2070 6173 730d 0a20 2020         pass..   
-00016d20: 2020 2020 206c 6173 7444 6179 4c61 7374       lastDayLast
-00016d30: 4d6f 6e74 6820 3d20 6c61 7374 4461 794c  Month = lastDayL
-00016d40: 6173 744d 6f6e 7468 2e73 7472 6674 696d  astMonth.strftim
-00016d50: 6528 2225 592d 256d 2d25 6454 3030 3a30  e("%Y-%m-%dT00:0
-00016d60: 303a 3030 2e30 3030 2229 0d0a 2020 2020  0:00.000")..    
-00016d70: 2020 2020 6966 206f 6e6c 794d 463a 0d0a      if onlyMF:..
-00016d80: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00016d90: 726e 206e 6574 4368 616e 6765 4d46 0d0a  rn netChangeMF..
-00016da0: 2020 2020 2020 2020 6966 206c 6174 6573          if lates
-00016db0: 745f 696e 7374 6461 7465 203d 3d20 6c61  t_instdate == la
-00016dc0: 7465 7374 5f6d 6664 6174 653a 0d0a 2020  test_mfdate:..  
-00016dd0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00016de0: 2028 6e65 7443 6861 6e67 654d 4620 2b20   (netChangeMF + 
-00016df0: 6e65 7443 6861 6e67 6549 6e73 7429 0d0a  netChangeInst)..
-00016e00: 2020 2020 2020 2020 656c 6966 206c 6174          elif lat
-00016e10: 6573 745f 6d66 6461 7465 203d 3d20 6c61  est_mfdate == la
-00016e20: 7374 4461 794c 6173 744d 6f6e 7468 3a0d  stDayLastMonth:.
-00016e30: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00016e40: 7572 6e20 6e65 7443 6861 6e67 654d 460d  urn netChangeMF.
-00016e50: 0a20 2020 2020 2020 2065 6c69 6620 6c61  .        elif la
-00016e60: 7465 7374 5f69 6e73 7464 6174 6520 3d3d  test_instdate ==
-00016e70: 206c 6173 7444 6179 4c61 7374 4d6f 6e74   lastDayLastMont
-00016e80: 683a 0d0a 2020 2020 2020 2020 2020 2020  h:..            
-00016e90: 7265 7475 726e 206e 6574 4368 616e 6765  return netChange
-00016ea0: 496e 7374 0d0a 2020 2020 2020 2020 656c  Inst..        el
-00016eb0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-00016ec0: 2023 2066 696e 6420 7468 6520 6c61 7465   # find the late
-00016ed0: 7374 2064 6174 650d 0a20 2020 2020 2020  st date..       
-00016ee0: 2020 2020 2069 6620 6c61 7465 7374 5f6d       if latest_m
-00016ef0: 6664 6174 6520 6973 206e 6f74 204e 6f6e  fdate is not Non
-00016f00: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00016f10: 2020 2020 6c61 7465 7374 5f6d 6664 6174      latest_mfdat
-00016f20: 6520 3d20 504b 4461 7465 5574 696c 6974  e = PKDateUtilit
-00016f30: 6965 732e 6461 7465 4672 6f6d 596d 6453  ies.dateFromYmdS
-00016f40: 7472 696e 6728 6c61 7465 7374 5f6d 6664  tring(latest_mfd
-00016f50: 6174 652e 7370 6c69 7428 2254 2229 5b30  ate.split("T")[0
-00016f60: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-00016f70: 6966 206c 6174 6573 745f 696e 7374 6461  if latest_instda
-00016f80: 7465 2069 7320 6e6f 7420 4e6f 6e65 3a0d  te is not None:.
+00015ff0: 2020 2020 7769 7468 2053 7570 7072 6573      with Suppres
+00016000: 734f 7574 7075 7428 7375 7070 7265 7373  sOutput(suppress
+00016010: 5f73 7464 6572 723d 5472 7565 2c20 7375  _stderr=True, su
+00016020: 7070 7265 7373 5f73 7464 6f75 743d 5472  ppress_stdout=Tr
+00016030: 7565 293a 0d0a 2020 2020 2020 2020 2020  ue):..          
+00016040: 2020 2020 2020 2020 2020 2020 2020 6676                fv
+00016050: 203d 2073 6563 7572 6974 792e 6661 6972   = security.fair
+00016060: 5661 6c75 6528 290d 0a20 2020 2020 2020  Value()..       
+00016070: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00016080: 6676 2069 7320 6e6f 7420 4e6f 6e65 3a0d  fv is not None:.
+00016090: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000160a0: 2020 2020 2020 2020 2074 7279 3a0d 0a20           try:.. 
+000160b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000160c0: 2020 2020 2020 2020 2020 2066 7652 6573             fvRes
+000160d0: 706f 6e73 6556 616c 7565 203d 2066 765b  ponseValue = fv[
+000160e0: 226c 6174 6573 7446 6169 7256 616c 7565  "latestFairValue
+000160f0: 225d 0d0a 2020 2020 2020 2020 2020 2020  "]..            
+00016100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016110: 6966 2066 7652 6573 706f 6e73 6556 616c  if fvResponseVal
+00016120: 7565 2069 7320 6e6f 7420 4e6f 6e65 3a0d  ue is not None:.
+00016130: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016150: 2066 6169 7256 616c 7565 203d 2066 6c6f   fairValue = flo
+00016160: 6174 2866 7652 6573 706f 6e73 6556 616c  at(fvResponseVal
+00016170: 7565 290d 0a20 2020 2020 2020 2020 2020  ue)..           
+00016180: 2020 2020 2020 2020 2020 2020 2065 7863               exc
+00016190: 6570 743a 2023 2070 7261 676d 613a 206e  ept: # pragma: n
+000161a0: 6f20 636f 7665 720d 0a20 2020 2020 2020  o cover..       
+000161b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000161c0: 2020 2020 2070 6173 730d 0a20 2020 2020       pass..     
+000161d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000161e0: 2020 2020 2020 2023 2073 656c 662e 6465         # self.de
+000161f0: 6661 756c 745f 6c6f 6767 6572 2e64 6562  fault_logger.deb
+00016200: 7567 2866 227b 657d 5c6e 5265 7370 6f6e  ug(f"{e}\nRespon
+00016210: 7365 3a66 763a 5c6e 7b66 767d 222c 2065  se:fv:\n{fv}", e
+00016220: 7863 5f69 6e66 6f3d 5472 7565 290d 0a20  xc_info=True).. 
+00016230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016240: 2020 2066 6169 7256 616c 7565 203d 2072     fairValue = r
+00016250: 6f75 6e64 2866 6c6f 6174 2866 6169 7256  ound(float(fairV
+00016260: 616c 7565 292c 3129 0d0a 2020 2020 2020  alue),1)..      
+00016270: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+00016280: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
+00016290: 2020 2020 2020 2020 2020 2020 686f 7374              host
+000162a0: 4461 7461 2e6c 6f63 5b68 6f73 7444 6174  Data.loc[hostDat
+000162b0: 612e 696e 6465 785b 2d31 5d2c 2246 6169  a.index[-1],"Fai
+000162c0: 7256 616c 7565 225d 203d 2066 6169 7256  rValue"] = fairV
+000162d0: 616c 7565 0d0a 2020 2020 2020 2020 2020  alue..          
+000162e0: 2020 2020 2020 2020 2020 6578 6365 7074            except
+000162f0: 2028 4b65 7945 7272 6f72 2c49 6e64 6578   (KeyError,Index
+00016300: 4572 726f 7229 3a0d 0a20 2020 2020 2020  Error):..       
+00016310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016320: 2070 6173 730d 0a20 2020 2020 2020 2072   pass..        r
+00016330: 6574 7572 6e20 6661 6972 5661 6c75 650d  eturn fairValue.
+00016340: 0a0d 0a20 2020 2064 6566 2067 6574 4d75  ...    def getMu
+00016350: 7475 616c 4675 6e64 5374 6174 7573 2873  tualFundStatus(s
+00016360: 656c 662c 2073 746f 636b 2c6f 6e6c 794d  elf, stock,onlyM
+00016370: 463d 4661 6c73 652c 2068 6f73 7444 6174  F=False, hostDat
+00016380: 613d 4e6f 6e65 2c20 666f 7263 653d 4661  a=None, force=Fa
+00016390: 6c73 652c 6578 6368 616e 6765 4e61 6d65  lse,exchangeName
+000163a0: 3d22 494e 4449 4122 293a 0d0a 2020 2020  ="INDIA"):..    
+000163b0: 2020 2020 6966 2068 6f73 7444 6174 6120      if hostData 
+000163c0: 6973 204e 6f6e 6520 6f72 206c 656e 2868  is None or len(h
+000163d0: 6f73 7444 6174 6129 203c 2031 3a0d 0a20  ostData) < 1:.. 
+000163e0: 2020 2020 2020 2020 2020 2068 6f73 7444             hostD
+000163f0: 6174 6120 3d20 7064 2e44 6174 6146 7261  ata = pd.DataFra
+00016400: 6d65 2829 0d0a 2020 2020 2020 2020 0d0a  me()..        ..
+00016410: 2020 2020 2020 2020 6e65 7443 6861 6e67          netChang
+00016420: 654d 4620 3d20 300d 0a20 2020 2020 2020  eMF = 0..       
+00016430: 206e 6574 4368 616e 6765 496e 7374 203d   netChangeInst =
+00016440: 2030 0d0a 2020 2020 2020 2020 6c61 7465   0..        late
+00016450: 7374 5f6d 6664 6174 6520 3d20 4e6f 6e65  st_mfdate = None
+00016460: 0d0a 2020 2020 2020 2020 6c61 7465 7374  ..        latest
+00016470: 5f69 6e73 7464 6174 6520 3d20 4e6f 6e65  _instdate = None
+00016480: 0d0a 2020 2020 2020 2020 6e65 6564 7346  ..        needsF
+00016490: 7265 7368 5570 6461 7465 203d 2054 7275  reshUpdate = Tru
+000164a0: 650d 0a20 2020 2020 2020 206c 6173 7444  e..        lastD
+000164b0: 6179 4c61 7374 4d6f 6e74 6820 3d20 504b  ayLastMonth = PK
+000164c0: 4461 7465 5574 696c 6974 6965 732e 6c61  DateUtilities.la
+000164d0: 7374 5f64 6179 5f6f 665f 7072 6576 696f  st_day_of_previo
+000164e0: 7573 5f6d 6f6e 7468 2850 4b44 6174 6555  us_month(PKDateU
+000164f0: 7469 6c69 7469 6573 2e63 7572 7265 6e74  tilities.current
+00016500: 4461 7465 5469 6d65 2829 290d 0a20 2020  DateTime())..   
+00016510: 2020 2020 2069 6620 686f 7374 4461 7461       if hostData
+00016520: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
+00016530: 206c 656e 2868 6f73 7444 6174 6129 203e   len(hostData) >
+00016540: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
+00016550: 2069 6620 224d 4622 2069 6e20 686f 7374   if "MF" in host
+00016560: 4461 7461 2e63 6f6c 756d 6e73 206f 7220  Data.columns or 
+00016570: 2246 4949 2220 696e 2068 6f73 7444 6174  "FII" in hostDat
+00016580: 612e 636f 6c75 6d6e 733a 0d0a 2020 2020  a.columns:..    
+00016590: 2020 2020 2020 2020 2020 2020 7472 793a              try:
+000165a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000165b0: 2020 2020 2020 6e65 7443 6861 6e67 654d        netChangeM
+000165c0: 4620 3d20 686f 7374 4461 7461 2e6c 6f63  F = hostData.loc
+000165d0: 5b68 6f73 7444 6174 612e 696e 6465 785b  [hostData.index[
+000165e0: 2d31 5d2c 224d 4622 5d0d 0a20 2020 2020  -1],"MF"]..     
+000165f0: 2020 2020 2020 2020 2020 2065 7863 6570             excep
+00016600: 7420 284b 6579 4572 726f 722c 496e 6465  t (KeyError,Inde
+00016610: 7845 7272 6f72 293a 0d0a 2020 2020 2020  xError):..      
+00016620: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+00016630: 7373 0d0a 2020 2020 2020 2020 2020 2020  ss..            
+00016640: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
+00016650: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
+00016660: 7443 6861 6e67 6549 6e73 7420 3d20 686f  tChangeInst = ho
+00016670: 7374 4461 7461 2e6c 6f63 5b68 6f73 7444  stData.loc[hostD
+00016680: 6174 612e 696e 6465 785b 2d31 5d2c 2246  ata.index[-1],"F
+00016690: 4949 225d 0d0a 2020 2020 2020 2020 2020  II"]..          
+000166a0: 2020 2020 2020 6578 6365 7074 2028 4b65        except (Ke
+000166b0: 7945 7272 6f72 2c49 6e64 6578 4572 726f  yError,IndexErro
+000166c0: 7229 3a0d 0a20 2020 2020 2020 2020 2020  r):..           
+000166d0: 2020 2020 2020 2020 2070 6173 730d 0a20           pass.. 
+000166e0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+000166f0: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
+00016700: 2020 2020 2020 2020 206c 6174 6573 745f           latest_
+00016710: 6d66 6461 7465 203d 2068 6f73 7444 6174  mfdate = hostDat
+00016720: 612e 6c6f 635b 686f 7374 4461 7461 2e69  a.loc[hostData.i
+00016730: 6e64 6578 5b2d 315d 2c22 4d46 5f44 6174  ndex[-1],"MF_Dat
+00016740: 6522 5d0d 0a20 2020 2020 2020 2020 2020  e"]..           
+00016750: 2020 2020 2065 7863 6570 7420 284b 6579       except (Key
+00016760: 4572 726f 722c 496e 6465 7845 7272 6f72  Error,IndexError
+00016770: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00016780: 2020 2020 2020 2020 7061 7373 0d0a 2020          pass..  
+00016790: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+000167a0: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
+000167b0: 2020 2020 2020 2020 6c61 7465 7374 5f69          latest_i
+000167c0: 6e73 7464 6174 6520 3d20 686f 7374 4461  nstdate = hostDa
+000167d0: 7461 2e6c 6f63 5b68 6f73 7444 6174 612e  ta.loc[hostData.
+000167e0: 696e 6465 785b 2d31 5d2c 2246 4949 5f44  index[-1],"FII_D
+000167f0: 6174 6522 5d0d 0a20 2020 2020 2020 2020  ate"]..         
+00016800: 2020 2020 2020 2065 7863 6570 7420 284b         except (K
+00016810: 6579 4572 726f 722c 496e 6465 7845 7272  eyError,IndexErr
+00016820: 6f72 293a 0d0a 2020 2020 2020 2020 2020  or):..          
+00016830: 2020 2020 2020 2020 2020 7061 7373 0d0a            pass..
+00016840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016850: 6966 206c 6174 6573 745f 6d66 6461 7465  if latest_mfdate
+00016860: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
+00016870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016880: 2020 2073 6176 6564 5f6d 6664 6174 6520     saved_mfdate 
+00016890: 3d20 504b 4461 7465 5574 696c 6974 6965  = PKDateUtilitie
+000168a0: 732e 6461 7465 4672 6f6d 596d 6453 7472  s.dateFromYmdStr
+000168b0: 696e 6728 6c61 7465 7374 5f6d 6664 6174  ing(latest_mfdat
+000168c0: 652e 7370 6c69 7428 2254 2229 5b30 5d29  e.split("T")[0])
+000168d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000168e0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+000168f0: 2020 2020 2020 2020 2020 2020 2073 6176               sav
+00016900: 6564 5f6d 6664 6174 6520 3d20 6c61 7374  ed_mfdate = last
+00016910: 4461 794c 6173 744d 6f6e 7468 202d 2064  DayLastMonth - d
+00016920: 6174 6574 696d 652e 7469 6d65 6465 6c74  atetime.timedelt
+00016930: 6128 3129 0d0a 2020 2020 2020 2020 2020  a(1)..          
+00016940: 2020 2020 2020 6966 206c 6174 6573 745f        if latest_
+00016950: 696e 7374 6461 7465 2069 7320 6e6f 7420  instdate is not 
+00016960: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+00016970: 2020 2020 2020 2020 2020 2073 6176 6564             saved
+00016980: 5f69 6e73 7464 6174 6520 3d20 504b 4461  _instdate = PKDa
+00016990: 7465 5574 696c 6974 6965 732e 6461 7465  teUtilities.date
+000169a0: 4672 6f6d 596d 6453 7472 696e 6728 6c61  FromYmdString(la
+000169b0: 7465 7374 5f69 6e73 7464 6174 652e 7370  test_instdate.sp
+000169c0: 6c69 7428 2254 2229 5b30 5d29 0d0a 2020  lit("T")[0])..  
+000169d0: 2020 2020 2020 2020 2020 2020 2020 656c                el
+000169e0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+000169f0: 2020 2020 2020 2020 2073 6176 6564 5f69           saved_i
+00016a00: 6e73 7464 6174 6520 3d20 6c61 7374 4461  nstdate = lastDa
+00016a10: 794c 6173 744d 6f6e 7468 202d 2064 6174  yLastMonth - dat
+00016a20: 6574 696d 652e 7469 6d65 6465 6c74 6128  etime.timedelta(
+00016a30: 3129 0d0a 2020 2020 2020 2020 2020 2020  1)..            
+00016a40: 2020 2020 746f 6461 7920 3d20 504b 4461      today = PKDa
+00016a50: 7465 5574 696c 6974 6965 732e 6375 7272  teUtilities.curr
+00016a60: 656e 7444 6174 6554 696d 6528 290d 0a20  entDateTime().. 
+00016a70: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00016a80: 6565 6473 4672 6573 6855 7064 6174 6520  eedsFreshUpdate 
+00016a90: 3d20 2873 6176 6564 5f6d 6664 6174 652e  = (saved_mfdate.
+00016aa0: 6461 7465 2829 203c 206c 6173 7444 6179  date() < lastDay
+00016ab0: 4c61 7374 4d6f 6e74 682e 6461 7465 2829  LastMonth.date()
+00016ac0: 2920 616e 6420 2873 6176 6564 5f69 6e73  ) and (saved_ins
+00016ad0: 7464 6174 652e 6461 7465 2829 203c 206c  tdate.date() < l
+00016ae0: 6173 7444 6179 4c61 7374 4d6f 6e74 682e  astDayLastMonth.
+00016af0: 6461 7465 2829 290d 0a20 2020 2020 2020  date())..       
+00016b00: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+00016b10: 2020 2020 2020 2020 2020 2020 6e65 6564              need
+00016b20: 7346 7265 7368 5570 6461 7465 203d 2054  sFreshUpdate = T
+00016b30: 7275 650d 0a0d 0a20 2020 2020 2020 2069  rue....        i
+00016b40: 6620 6e65 6564 7346 7265 7368 5570 6461  f needsFreshUpda
+00016b50: 7465 2061 6e64 2066 6f72 6365 3a0d 0a20  te and force:.. 
+00016b60: 2020 2020 2020 2020 2020 206e 6574 4368             netCh
+00016b70: 616e 6765 4d46 2c20 6e65 7443 6861 6e67  angeMF, netChang
+00016b80: 6549 6e73 742c 206c 6174 6573 745f 6d66  eInst, latest_mf
+00016b90: 6461 7465 2c20 6c61 7465 7374 5f69 6e73  date, latest_ins
+00016ba0: 7464 6174 6520 3d20 7365 6c66 2e67 6574  tdate = self.get
+00016bb0: 4672 6573 684d 4649 5374 6174 7573 2873  FreshMFIStatus(s
+00016bc0: 746f 636b 2c65 7863 6861 6e67 654e 616d  tock,exchangeNam
+00016bd0: 653d 6578 6368 616e 6765 4e61 6d65 290d  e=exchangeName).
+00016be0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00016bf0: 6e65 7443 6861 6e67 654d 4620 6973 206e  netChangeMF is n
+00016c00: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
+00016c10: 2020 2020 2020 2020 2020 7472 793a 0d0a            try:..
+00016c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016c30: 2020 2020 686f 7374 4461 7461 2e6c 6f63      hostData.loc
+00016c40: 5b68 6f73 7444 6174 612e 696e 6465 785b  [hostData.index[
+00016c50: 2d31 5d2c 224d 4622 5d20 3d20 6e65 7443  -1],"MF"] = netC
+00016c60: 6861 6e67 654d 460d 0a20 2020 2020 2020  hangeMF..       
+00016c70: 2020 2020 2020 2020 2065 7863 6570 7420           except 
+00016c80: 284b 6579 4572 726f 722c 496e 6465 7845  (KeyError,IndexE
+00016c90: 7272 6f72 293a 0d0a 2020 2020 2020 2020  rror):..        
+00016ca0: 2020 2020 2020 2020 2020 2020 7061 7373              pass
+00016cb0: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
+00016cc0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00016cd0: 2020 2020 206e 6574 4368 616e 6765 4d46       netChangeMF
+00016ce0: 203d 2030 0d0a 2020 2020 2020 2020 2020   = 0..          
+00016cf0: 2020 6966 206c 6174 6573 745f 6d66 6461    if latest_mfda
+00016d00: 7465 2069 7320 6e6f 7420 4e6f 6e65 3a0d  te is not None:.
+00016d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016d20: 2074 7279 3a0d 0a20 2020 2020 2020 2020   try:..         
+00016d30: 2020 2020 2020 2020 2020 2068 6f73 7444             hostD
+00016d40: 6174 612e 6c6f 635b 686f 7374 4461 7461  ata.loc[hostData
+00016d50: 2e69 6e64 6578 5b2d 315d 2c22 4d46 5f44  .index[-1],"MF_D
+00016d60: 6174 6522 5d20 3d20 6c61 7465 7374 5f6d  ate"] = latest_m
+00016d70: 6664 6174 650d 0a20 2020 2020 2020 2020  fdate..         
+00016d80: 2020 2020 2020 2065 7863 6570 7420 284b         except (K
+00016d90: 6579 4572 726f 722c 496e 6465 7845 7272  eyError,IndexErr
+00016da0: 6f72 293a 0d0a 2020 2020 2020 2020 2020  or):..          
+00016db0: 2020 2020 2020 2020 2020 7061 7373 0d0a            pass..
+00016dc0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+00016dd0: 6574 4368 616e 6765 496e 7374 2069 7320  etChangeInst is 
+00016de0: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
+00016df0: 2020 2020 2020 2020 2020 2074 7279 3a0d             try:.
+00016e00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016e10: 2020 2020 2068 6f73 7444 6174 612e 6c6f       hostData.lo
+00016e20: 635b 686f 7374 4461 7461 2e69 6e64 6578  c[hostData.index
+00016e30: 5b2d 315d 2c22 4649 4922 5d20 3d20 6e65  [-1],"FII"] = ne
+00016e40: 7443 6861 6e67 6549 6e73 740d 0a20 2020  tChangeInst..   
+00016e50: 2020 2020 2020 2020 2020 2020 2065 7863               exc
+00016e60: 6570 7420 284b 6579 4572 726f 722c 496e  ept (KeyError,In
+00016e70: 6465 7845 7272 6f72 293a 0d0a 2020 2020  dexError):..    
+00016e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016e90: 7061 7373 0d0a 2020 2020 2020 2020 2020  pass..          
+00016ea0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+00016eb0: 2020 2020 2020 2020 206e 6574 4368 616e           netChan
+00016ec0: 6765 496e 7374 203d 2030 0d0a 2020 2020  geInst = 0..    
+00016ed0: 2020 2020 2020 2020 6966 206c 6174 6573          if lates
+00016ee0: 745f 696e 7374 6461 7465 2069 7320 6e6f  t_instdate is no
+00016ef0: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
+00016f00: 2020 2020 2020 2020 2074 7279 3a0d 0a20           try:.. 
+00016f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016f20: 2020 2068 6f73 7444 6174 612e 6c6f 635b     hostData.loc[
+00016f30: 686f 7374 4461 7461 2e69 6e64 6578 5b2d  hostData.index[-
+00016f40: 315d 2c22 4649 495f 4461 7465 225d 203d  1],"FII_Date"] =
+00016f50: 206c 6174 6573 745f 696e 7374 6461 7465   latest_instdate
+00016f60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016f70: 2020 6578 6365 7074 2028 4b65 7945 7272    except (KeyErr
+00016f80: 6f72 2c49 6e64 6578 4572 726f 7229 3a0d  or,IndexError):.
 00016f90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016fa0: 206c 6174 6573 745f 696e 7374 6461 7465   latest_instdate
-00016fb0: 203d 2050 4b44 6174 6555 7469 6c69 7469   = PKDateUtiliti
-00016fc0: 6573 2e64 6174 6546 726f 6d59 6d64 5374  es.dateFromYmdSt
-00016fd0: 7269 6e67 286c 6174 6573 745f 696e 7374  ring(latest_inst
-00016fe0: 6461 7465 2e73 706c 6974 2822 5422 295b  date.split("T")[
-00016ff0: 305d 290d 0a20 2020 2020 2020 2020 2020  0])..           
-00017000: 2072 6574 7572 6e20 6e65 7443 6861 6e67   return netChang
-00017010: 654d 4620 6966 2028 286c 6174 6573 745f  eMF if ((latest_
-00017020: 6d66 6461 7465 2069 7320 6e6f 7420 4e6f  mfdate is not No
-00017030: 6e65 2920 616e 6420 6c61 7465 7374 5f6d  ne) and latest_m
-00017040: 6664 6174 6520 3e20 286c 6174 6573 745f  fdate > (latest_
-00017050: 696e 7374 6461 7465 2069 6620 6c61 7465  instdate if late
-00017060: 7374 5f69 6e73 7464 6174 6520 6973 206e  st_instdate is n
-00017070: 6f74 204e 6f6e 6520 656c 7365 2028 6c61  ot None else (la
-00017080: 7465 7374 5f6d 6664 6174 6520 2d20 6461  test_mfdate - da
-00017090: 7465 7469 6d65 2e74 696d 6564 656c 7461  tetime.timedelta
-000170a0: 2831 2929 2929 2065 6c73 6520 6e65 7443  (1)))) else netC
-000170b0: 6861 6e67 6549 6e73 740d 0a0d 0a20 2020  hangeInst....   
-000170c0: 2064 6566 2067 6574 4672 6573 684d 4649   def getFreshMFI
-000170d0: 5374 6174 7573 2873 656c 662c 2073 746f  Status(self, sto
-000170e0: 636b 2c65 7863 6861 6e67 654e 616d 653d  ck,exchangeName=
-000170f0: 2249 4e44 4941 2229 3a0d 0a20 2020 2020  "INDIA"):..     
-00017100: 2020 2063 6861 6e67 6553 7461 7475 7344     changeStatusD
-00017110: 6174 614d 4620 3d20 4e6f 6e65 0d0a 2020  ataMF = None..  
-00017120: 2020 2020 2020 6368 616e 6765 5374 6174        changeStat
-00017130: 7573 4461 7461 496e 7374 203d 204e 6f6e  usDataInst = Non
-00017140: 650d 0a20 2020 2020 2020 206e 6574 4368  e..        netCh
-00017150: 616e 6765 4d46 203d 2030 0d0a 2020 2020  angeMF = 0..    
-00017160: 2020 2020 6e65 7443 6861 6e67 6549 6e73      netChangeIns
-00017170: 7420 3d20 300d 0a20 2020 2020 2020 206c  t = 0..        l
-00017180: 6174 6573 745f 6d66 6461 7465 203d 204e  atest_mfdate = N
-00017190: 6f6e 650d 0a20 2020 2020 2020 206c 6174  one..        lat
-000171a0: 6573 745f 696e 7374 6461 7465 203d 204e  est_instdate = N
-000171b0: 6f6e 650d 0a20 2020 2020 2020 2073 6563  one..        sec
-000171c0: 7572 6974 7920 3d20 4e6f 6e65 0d0a 2020  urity = None..  
-000171d0: 2020 2020 2020 7472 793a 0d0a 2020 2020        try:..    
-000171e0: 2020 2020 2020 2020 7769 7468 2053 7570          with Sup
-000171f0: 7072 6573 734f 7574 7075 7428 7375 7070  pressOutput(supp
-00017200: 7265 7373 5f73 7464 6572 723d 5472 7565  ress_stderr=True
-00017210: 2c20 7375 7070 7265 7373 5f73 7464 6f75  , suppress_stdou
-00017220: 743d 5472 7565 293a 0d0a 2020 2020 2020  t=True):..      
-00017230: 2020 2020 2020 2020 2020 7365 6375 7269            securi
-00017240: 7479 203d 2053 746f 636b 2873 746f 636b  ty = Stock(stock
-00017250: 2c65 7863 6861 6e67 653d 6578 6368 616e  ,exchange=exchan
-00017260: 6765 4e61 6d65 290d 0a20 2020 2020 2020  geName)..       
-00017270: 2065 7863 6570 7420 5661 6c75 6545 7272   except ValueErr
-00017280: 6f72 3a0d 0a20 2020 2020 2020 2020 2020  or:..           
-00017290: 2023 2057 6520 6469 6420 6e6f 7420 6669   # We did not fi
-000172a0: 6e64 2074 6865 2073 746f 636b 3f20 4974  nd the stock? It
-000172b0: 2773 206f 6b61 792e 204d 6f76 6520 6f6e  's okay. Move on
-000172c0: 2074 6f20 7468 6520 6e65 7874 206f 6e65   to the next one
-000172d0: 2e0d 0a20 2020 2020 2020 2020 2020 2070  ...            p
-000172e0: 6173 730d 0a20 2020 2020 2020 2069 6620  ass..        if 
-000172f0: 7365 6375 7269 7479 2069 7320 6e6f 7420  security is not 
-00017300: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-00017310: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
-00017320: 2020 2020 2020 2020 2077 6974 6820 5375           with Su
-00017330: 7070 7265 7373 4f75 7470 7574 2873 7570  ppressOutput(sup
-00017340: 7072 6573 735f 7374 6465 7272 3d54 7275  press_stderr=Tru
-00017350: 652c 2073 7570 7072 6573 735f 7374 646f  e, suppress_stdo
-00017360: 7574 3d54 7275 6529 3a0d 0a20 2020 2020  ut=True):..     
-00017370: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00017380: 6861 6e67 6553 7461 7475 7352 6f77 734d  hangeStatusRowsM
-00017390: 4620 3d20 7365 6375 7269 7479 2e6d 7574  F = security.mut
-000173a0: 7561 6c46 756e 644f 776e 6572 7368 6970  ualFundOwnership
-000173b0: 2874 6f70 3d35 290d 0a20 2020 2020 2020  (top=5)..       
-000173c0: 2020 2020 2020 2020 2020 2020 2063 6861               cha
-000173d0: 6e67 6553 7461 7475 7352 6f77 7349 6e73  ngeStatusRowsIns
-000173e0: 7420 3d20 7365 6375 7269 7479 2e69 6e73  t = security.ins
-000173f0: 7469 7475 7469 6f6e 4f77 6e65 7273 6869  titutionOwnershi
-00017400: 7028 746f 703d 3529 0d0a 2020 2020 2020  p(top=5)..      
-00017410: 2020 2020 2020 2020 2020 2020 2020 6368                ch
-00017420: 616e 6765 5374 6174 7573 4461 7461 4d46  angeStatusDataMF
-00017430: 203d 2073 6563 7572 6974 792e 6d75 7475   = security.mutu
-00017440: 616c 4675 6e64 4649 4943 6861 6e67 6544  alFundFIIChangeD
-00017450: 6174 6128 6368 616e 6765 5374 6174 7573  ata(changeStatus
-00017460: 526f 7773 4d46 290d 0a20 2020 2020 2020  RowsMF)..       
-00017470: 2020 2020 2020 2020 2020 2020 2063 6861               cha
-00017480: 6e67 6553 7461 7475 7344 6174 6149 6e73  ngeStatusDataIns
-00017490: 7420 3d20 7365 6375 7269 7479 2e6d 7574  t = security.mut
-000174a0: 7561 6c46 756e 6446 4949 4368 616e 6765  ualFundFIIChange
-000174b0: 4461 7461 2863 6861 6e67 6553 7461 7475  Data(changeStatu
-000174c0: 7352 6f77 7349 6e73 7429 0d0a 2020 2020  sRowsInst)..    
-000174d0: 2020 2020 2020 2020 6578 6365 7074 2045          except E
-000174e0: 7863 6570 7469 6f6e 2061 7320 653a 0d0a  xception as e:..
-000174f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017500: 7365 6c66 2e64 6566 6175 6c74 5f6c 6f67  self.default_log
-00017510: 6765 722e 6465 6275 6728 652c 2065 7863  ger.debug(e, exc
-00017520: 5f69 6e66 6f3d 5472 7565 290d 0a20 2020  _info=True)..   
-00017530: 2020 2020 2020 2020 2020 2020 2023 2054               # T
-00017540: 7970 6545 7272 6f72 206f 7220 436f 6e6e  ypeError or Conn
-00017550: 6563 7469 6f6e 4572 726f 7220 6265 6361  ectionError beca
-00017560: 7573 6520 7765 2063 6f75 6c64 206e 6f74  use we could not
-00017570: 2066 696e 6420 7468 6520 7374 6f63 6b20   find the stock 
-00017580: 6f72 204d 4649 2064 6174 6120 6973 6e27  or MFI data isn'
-00017590: 7420 6176 6169 6c61 626c 653f 0d0a 2020  t available?..  
-000175a0: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-000175b0: 7373 0d0a 2020 2020 2020 2020 2020 2020  ss..            
-000175c0: 6c61 7374 4461 794c 6173 744d 6f6e 7468  lastDayLastMonth
-000175d0: 203d 2050 4b44 6174 6555 7469 6c69 7469   = PKDateUtiliti
-000175e0: 6573 2e6c 6173 745f 6461 795f 6f66 5f70  es.last_day_of_p
-000175f0: 7265 7669 6f75 735f 6d6f 6e74 6828 504b  revious_month(PK
-00017600: 4461 7465 5574 696c 6974 6965 732e 6375  DateUtilities.cu
-00017610: 7272 656e 7444 6174 6554 696d 6528 2929  rrentDateTime())
-00017620: 0d0a 2020 2020 2020 2020 2020 2020 6c61  ..            la
-00017630: 7374 4461 794c 6173 744d 6f6e 7468 203d  stDayLastMonth =
-00017640: 206c 6173 7444 6179 4c61 7374 4d6f 6e74   lastDayLastMont
-00017650: 682e 7374 7266 7469 6d65 2822 2559 2d25  h.strftime("%Y-%
-00017660: 6d2d 2564 5430 303a 3030 3a30 302e 3030  m-%dT00:00:00.00
-00017670: 3022 290d 0a20 2020 2020 2020 2020 2020  0")..           
-00017680: 2069 6620 6368 616e 6765 5374 6174 7573   if changeStatus
-00017690: 4461 7461 4d46 2069 7320 6e6f 7420 4e6f  DataMF is not No
-000176a0: 6e65 2061 6e64 206c 656e 2863 6861 6e67  ne and len(chang
-000176b0: 6553 7461 7475 7344 6174 614d 4629 203e  eStatusDataMF) >
-000176c0: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
-000176d0: 2020 2020 2064 665f 6772 6f75 7065 644d       df_groupedM
-000176e0: 4620 3d20 6368 616e 6765 5374 6174 7573  F = changeStatus
-000176f0: 4461 7461 4d46 2e67 726f 7570 6279 2822  DataMF.groupby("
-00017700: 6461 7465 222c 2073 6f72 743d 4661 6c73  date", sort=Fals
-00017710: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
-00017720: 2020 2020 666f 7220 6d66 6461 7465 2c20      for mfdate, 
-00017730: 6466 5f67 726f 7570 4d46 2069 6e20 6466  df_groupMF in df
-00017740: 5f67 726f 7570 6564 4d46 3a0d 0a20 2020  _groupedMF:..   
-00017750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017760: 206e 6574 4368 616e 6765 4d46 203d 2064   netChangeMF = d
-00017770: 665f 6772 6f75 704d 465b 2263 6861 6e67  f_groupMF["chang
-00017780: 6541 6d6f 756e 7422 5d2e 7375 6d28 290d  eAmount"].sum().
-00017790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000177a0: 2020 2020 206c 6174 6573 745f 6d66 6461       latest_mfda
-000177b0: 7465 203d 206d 6664 6174 650d 0a20 2020  te = mfdate..   
-000177c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000177d0: 2062 7265 616b 0d0a 2020 2020 2020 2020   break..        
-000177e0: 2020 2020 6966 2063 6861 6e67 6553 7461      if changeSta
-000177f0: 7475 7344 6174 6149 6e73 7420 6973 206e  tusDataInst is n
-00017800: 6f74 204e 6f6e 6520 616e 6420 6c65 6e28  ot None and len(
-00017810: 6368 616e 6765 5374 6174 7573 4461 7461  changeStatusData
-00017820: 496e 7374 2920 3e20 303a 0d0a 2020 2020  Inst) > 0:..    
-00017830: 2020 2020 2020 2020 2020 2020 6466 5f67              df_g
-00017840: 726f 7570 6564 496e 7374 203d 2063 6861  roupedInst = cha
-00017850: 6e67 6553 7461 7475 7344 6174 6149 6e73  ngeStatusDataIns
-00017860: 742e 6772 6f75 7062 7928 2264 6174 6522  t.groupby("date"
-00017870: 2c20 736f 7274 3d46 616c 7365 290d 0a20  , sort=False).. 
-00017880: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00017890: 6f72 2069 6e73 7464 6174 652c 2064 665f  or instdate, df_
-000178a0: 6772 6f75 7049 6e73 7420 696e 2064 665f  groupInst in df_
-000178b0: 6772 6f75 7065 6449 6e73 743a 0d0a 2020  groupedInst:..  
-000178c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000178d0: 2020 6966 2028 6c61 7465 7374 5f6d 6664    if (latest_mfd
-000178e0: 6174 6520 6973 206e 6f74 204e 6f6e 6520  ate is not None 
-000178f0: 616e 6420 6c61 7465 7374 5f6d 6664 6174  and latest_mfdat
-00017900: 6520 3d3d 2069 6e73 7464 6174 6529 206f  e == instdate) o
-00017910: 7220 286c 6174 6573 745f 6d66 6461 7465  r (latest_mfdate
-00017920: 2069 7320 4e6f 6e65 2920 6f72 2028 696e   is None) or (in
-00017930: 7374 6461 7465 203d 3d20 6c61 7374 4461  stdate == lastDa
-00017940: 794c 6173 744d 6f6e 7468 293a 0d0a 2020  yLastMonth):..  
-00017950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017960: 2020 2020 2020 6e65 7443 6861 6e67 6549        netChangeI
-00017970: 6e73 7420 3d20 6466 5f67 726f 7570 496e  nst = df_groupIn
-00017980: 7374 5b22 6368 616e 6765 416d 6f75 6e74  st["changeAmount
-00017990: 225d 2e73 756d 2829 0d0a 2020 2020 2020  "].sum()..      
-000179a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000179b0: 2020 6c61 7465 7374 5f69 6e73 7464 6174    latest_instdat
-000179c0: 6520 3d20 696e 7374 6461 7465 0d0a 2020  e = instdate..  
-000179d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000179e0: 2020 6272 6561 6b0d 0a20 2020 2020 2020    break..       
-000179f0: 2072 6574 7572 6e20 6e65 7443 6861 6e67   return netChang
-00017a00: 654d 462c 6e65 7443 6861 6e67 6549 6e73  eMF,netChangeIns
-00017a10: 742c 6c61 7465 7374 5f6d 6664 6174 652c  t,latest_mfdate,
-00017a20: 6c61 7465 7374 5f69 6e73 7464 6174 650d  latest_instdate.
-00017a30: 0a0d 0a0d 0a20 2020 2064 6566 2067 6574  .....    def get
-00017a40: 4e69 6674 7950 7265 6469 6374 696f 6e28  NiftyPrediction(
-00017a50: 7365 6c66 2c20 6466 293a 0d0a 2020 2020  self, df):..    
-00017a60: 2020 2020 696d 706f 7274 2077 6172 6e69      import warni
-00017a70: 6e67 730d 0a0d 0a20 2020 2020 2020 2077  ngs....        w
-00017a80: 6172 6e69 6e67 732e 6669 6c74 6572 7761  arnings.filterwa
-00017a90: 726e 696e 6773 2822 6967 6e6f 7265 2229  rnings("ignore")
-00017aa0: 0d0a 2020 2020 2020 2020 6461 7461 203d  ..        data =
-00017ab0: 2064 662e 636f 7079 2829 0d0a 2020 2020   df.copy()..    
-00017ac0: 2020 2020 6d6f 6465 6c2c 2070 6b6c 203d      model, pkl =
-00017ad0: 2055 7469 6c69 7479 2e74 6f6f 6c73 2e67   Utility.tools.g
-00017ae0: 6574 4e69 6674 794d 6f64 656c 2829 0d0a  etNiftyModel()..
-00017af0: 2020 2020 2020 2020 6966 206d 6f64 656c          if model
-00017b00: 2069 7320 4e6f 6e65 206f 7220 706b 6c20   is None or pkl 
-00017b10: 6973 204e 6f6e 653a 0d0a 2020 2020 2020  is None:..      
-00017b20: 2020 2020 2020 7265 7475 726e 2030 2c20        return 0, 
-00017b30: 2255 6e6b 6e6f 776e 222c 2022 556e 6b6e  "Unknown", "Unkn
-00017b40: 6f77 6e22 0d0a 2020 2020 2020 2020 7769  own"..        wi
-00017b50: 7468 2053 7570 7072 6573 734f 7574 7075  th SuppressOutpu
-00017b60: 7428 7375 7070 7265 7373 5f73 7464 6572  t(suppress_stder
-00017b70: 723d 5472 7565 2c20 7375 7070 7265 7373  r=True, suppress
-00017b80: 5f73 7464 6f75 743d 5472 7565 293a 0d0a  _stdout=True):..
-00017b90: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00017ba0: 203d 2064 6174 615b 706b 6c5b 2263 6f6c   = data[pkl["col
-00017bb0: 756d 6e73 225d 5d0d 0a20 2020 2020 2020  umns"]]..       
-00017bc0: 2020 2020 2023 2323 2076 3220 5072 6570       ### v2 Prep
-00017bd0: 726f 6365 7373 696e 670d 0a20 2020 2020  rocessing..     
-00017be0: 2020 2020 2020 2064 6174 615b 2248 6967         data["Hig
-00017bf0: 6822 5d20 3d20 6461 7461 5b22 4869 6768  h"] = data["High
-00017c00: 225d 2e70 6374 5f63 6861 6e67 6528 2920  "].pct_change() 
-00017c10: 2a20 3130 300d 0a20 2020 2020 2020 2020  * 100..         
-00017c20: 2020 2064 6174 615b 224c 6f77 225d 203d     data["Low"] =
-00017c30: 2064 6174 615b 224c 6f77 225d 2e70 6374   data["Low"].pct
-00017c40: 5f63 6861 6e67 6528 2920 2a20 3130 300d  _change() * 100.
-00017c50: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-00017c60: 615b 224f 7065 6e22 5d20 3d20 6461 7461  a["Open"] = data
-00017c70: 5b22 4f70 656e 225d 2e70 6374 5f63 6861  ["Open"].pct_cha
-00017c80: 6e67 6528 2920 2a20 3130 300d 0a20 2020  nge() * 100..   
-00017c90: 2020 2020 2020 2020 2064 6174 615b 2243           data["C
-00017ca0: 6c6f 7365 225d 203d 2064 6174 615b 2243  lose"] = data["C
-00017cb0: 6c6f 7365 225d 2e70 6374 5f63 6861 6e67  lose"].pct_chang
-00017cc0: 6528 2920 2a20 3130 300d 0a20 2020 2020  e() * 100..     
-00017cd0: 2020 2020 2020 2064 6174 6120 3d20 6461         data = da
-00017ce0: 7461 2e69 6c6f 635b 2d31 5d0d 0a20 2020  ta.iloc[-1]..   
-00017cf0: 2020 2020 2020 2020 2023 2323 0d0a 2020           ###..  
-00017d00: 2020 2020 2020 2020 2020 6461 7461 203d            data =
-00017d10: 2070 6b6c 5b22 7363 616c 6572 225d 2e74   pkl["scaler"].t
-00017d20: 7261 6e73 666f 726d 285b 6461 7461 5d29  ransform([data])
-00017d30: 0d0a 2020 2020 2020 2020 2020 2020 7769  ..            wi
-00017d40: 7468 2053 7570 7072 6573 734f 7574 7075  th SuppressOutpu
-00017d50: 7428 7375 7070 7265 7373 5f73 7464 6f75  t(suppress_stdou
-00017d60: 743d 5472 7565 2c20 7375 7070 7265 7373  t=True, suppress
-00017d70: 5f73 7464 6572 723d 5472 7565 293a 0d0a  _stderr=True):..
-00017d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017d90: 7072 6564 203d 206d 6f64 656c 2e70 7265  pred = model.pre
-00017da0: 6469 6374 2864 6174 6129 5b30 5d0d 0a20  dict(data)[0].. 
-00017db0: 2020 2020 2020 2069 6620 7072 6564 203e         if pred >
-00017dc0: 2030 2e35 3a0d 0a20 2020 2020 2020 2020   0.5:..         
-00017dd0: 2020 206f 7574 5465 7874 203d 2022 4245     outText = "BE
-00017de0: 4152 4953 4822 0d0a 2020 2020 2020 2020  ARISH"..        
-00017df0: 2020 2020 6f75 7420 3d20 280d 0a20 2020      out = (..   
-00017e00: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
-00017e10: 6f72 5465 7874 2e42 4f4c 440d 0a20 2020  orText.BOLD..   
-00017e20: 2020 2020 2020 2020 2020 2020 202b 2063               + c
-00017e30: 6f6c 6f72 5465 7874 2e46 4149 4c0d 0a20  olorText.FAIL.. 
-00017e40: 2020 2020 2020 2020 2020 2020 2020 202b                 +
-00017e50: 206f 7574 5465 7874 0d0a 2020 2020 2020   outText..      
-00017e60: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
-00017e70: 7254 6578 742e 454e 440d 0a20 2020 2020  rText.END..     
-00017e80: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
-00017e90: 6f72 5465 7874 2e42 4f4c 440d 0a20 2020  orText.BOLD..   
-00017ea0: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
-00017eb0: 2020 2020 2020 2020 7375 6720 3d20 2248          sug = "H
-00017ec0: 6f6c 6420 796f 7572 2053 686f 7274 2070  old your Short p
-00017ed0: 6f73 6974 696f 6e21 220d 0a20 2020 2020  osition!"..     
-00017ee0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00017ef0: 2020 2020 2020 6f75 7454 6578 7420 3d20        outText = 
-00017f00: 2242 554c 4c49 5348 220d 0a20 2020 2020  "BULLISH"..     
-00017f10: 2020 2020 2020 206f 7574 203d 2028 0d0a         out = (..
-00017f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017f30: 636f 6c6f 7254 6578 742e 424f 4c44 0d0a  colorText.BOLD..
-00017f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017f50: 2b20 636f 6c6f 7254 6578 742e 4752 4545  + colorText.GREE
-00017f60: 4e0d 0a20 2020 2020 2020 2020 2020 2020  N..             
-00017f70: 2020 202b 206f 7574 5465 7874 0d0a 2020     + outText..  
-00017f80: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-00017f90: 636f 6c6f 7254 6578 742e 454e 440d 0a20  colorText.END.. 
-00017fa0: 2020 2020 2020 2020 2020 2020 2020 202b                 +
-00017fb0: 2063 6f6c 6f72 5465 7874 2e42 4f4c 440d   colorText.BOLD.
-00017fc0: 0a20 2020 2020 2020 2020 2020 2029 0d0a  .            )..
-00017fd0: 2020 2020 2020 2020 2020 2020 7375 6720              sug 
-00017fe0: 3d20 2253 7461 7920 4275 6c6c 6973 6821  = "Stay Bullish!
-00017ff0: 220d 0a20 2020 2020 2020 2069 6620 504b  "..        if PK
-00018000: 4461 7465 5574 696c 6974 6965 732e 6973  DateUtilities.is
-00018010: 436c 6f73 696e 6748 6f75 7228 293a 0d0a  ClosingHour():..
-00018020: 2020 2020 2020 2020 2020 2020 4f75 7470              Outp
-00018030: 7574 436f 6e74 726f 6c73 2829 2e70 7269  utControls().pri
-00018040: 6e74 4f75 7470 7574 280d 0a20 2020 2020  ntOutput(..     
-00018050: 2020 2020 2020 2020 2020 2063 6f6c 6f72             color
-00018060: 5465 7874 2e42 4f4c 440d 0a20 2020 2020  Text.BOLD..     
-00018070: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
-00018080: 6f72 5465 7874 2e57 4152 4e0d 0a20 2020  orText.WARN..   
-00018090: 2020 2020 2020 2020 2020 2020 202b 2022               + "
-000180a0: 4e6f 7465 3a20 5468 6520 4149 2070 7265  Note: The AI pre
-000180b0: 6469 6374 696f 6e20 7368 6f75 6c64 2062  diction should b
-000180c0: 6520 6578 6563 7574 6564 2041 6674 6572  e executed After
-000180d0: 2033 2050 4d20 6f72 204e 6561 7220 746f   3 PM or Near to
-000180e0: 2043 6c6f 7369 6e67 2074 696d 6520 6173   Closing time as
-000180f0: 2074 6865 2050 7265 6469 6374 696f 6e20   the Prediction 
-00018100: 4163 6375 7261 6379 2069 7320 6261 7365  Accuracy is base
-00018110: 6420 6f6e 2074 6865 2043 6c6f 7369 6e67  d on the Closing
-00018120: 2070 7269 6365 2122 0d0a 2020 2020 2020   price!"..      
-00018130: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
-00018140: 7254 6578 742e 454e 440d 0a20 2020 2020  rText.END..     
-00018150: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-00018160: 2020 7072 6564 6963 7469 6f6e 5465 7874    predictionText
-00018170: 203d 2022 4d61 726b 6574 206d 6179 204f   = "Market may O
-00018180: 7065 6e20 7b7d 206e 6578 7420 6461 7921  pen {} next day!
-00018190: 207b 7d22 2e66 6f72 6d61 7428 6f75 742c   {}".format(out,
-000181a0: 2073 7567 290d 0a20 2020 2020 2020 2073   sug)..        s
-000181b0: 7472 656e 6774 6854 6578 7420 3d20 2250  trengthText = "P
-000181c0: 726f 6261 6269 6c69 7479 2f53 7472 656e  robability/Stren
-000181d0: 6774 6820 6f66 2050 7265 6469 6374 696f  gth of Predictio
-000181e0: 6e20 3d20 7b7d 2522 2e66 6f72 6d61 7428  n = {}%".format(
-000181f0: 0d0a 2020 2020 2020 2020 2020 2020 5574  ..            Ut
-00018200: 696c 6974 792e 746f 6f6c 732e 6765 7453  ility.tools.getS
-00018210: 6967 6d6f 6964 436f 6e66 6964 656e 6365  igmoidConfidence
-00018220: 2870 7265 645b 305d 290d 0a20 2020 2020  (pred[0])..     
-00018230: 2020 2029 0d0a 2020 2020 2020 2020 4f75     )..        Ou
-00018240: 7470 7574 436f 6e74 726f 6c73 2829 2e70  tputControls().p
-00018250: 7269 6e74 4f75 7470 7574 280d 0a20 2020  rintOutput(..   
-00018260: 2020 2020 2020 2020 2063 6f6c 6f72 5465           colorTe
-00018270: 7874 2e42 4f4c 440d 0a20 2020 2020 2020  xt.BOLD..       
-00018280: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
-00018290: 2e42 4c55 450d 0a20 2020 2020 2020 2020  .BLUE..         
-000182a0: 2020 202b 2022 5c6e 220d 0a20 2020 2020     + "\n"..     
-000182b0: 2020 2020 2020 202b 2022 5b2b 5d20 4e69         + "[+] Ni
-000182c0: 6674 7920 4149 2050 7265 6469 6374 696f  fty AI Predictio
-000182d0: 6e20 2d3e 2022 0d0a 2020 2020 2020 2020  n -> "..        
-000182e0: 2020 2020 2b20 636f 6c6f 7254 6578 742e      + colorText.
-000182f0: 454e 440d 0a20 2020 2020 2020 2020 2020  END..           
-00018300: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
-00018310: 440d 0a20 2020 2020 2020 2020 2020 202b  D..            +
-00018320: 2070 7265 6469 6374 696f 6e54 6578 740d   predictionText.
-00018330: 0a20 2020 2020 2020 2020 2020 202b 2063  .            + c
-00018340: 6f6c 6f72 5465 7874 2e45 4e44 0d0a 2020  olorText.END..  
-00018350: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-00018360: 204f 7574 7075 7443 6f6e 7472 6f6c 7328   OutputControls(
-00018370: 292e 7072 696e 744f 7574 7075 7428 0d0a  ).printOutput(..
-00018380: 2020 2020 2020 2020 2020 2020 636f 6c6f              colo
-00018390: 7254 6578 742e 424f 4c44 0d0a 2020 2020  rText.BOLD..    
-000183a0: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
-000183b0: 6578 742e 424c 5545 0d0a 2020 2020 2020  ext.BLUE..      
-000183c0: 2020 2020 2020 2b20 225c 6e22 0d0a 2020        + "\n"..  
-000183d0: 2020 2020 2020 2020 2020 2b20 225b 2b5d            + "[+]
-000183e0: 204e 6966 7479 2041 4920 5072 6564 6963   Nifty AI Predic
-000183f0: 7469 6f6e 202d 3e20 220d 0a20 2020 2020  tion -> "..     
-00018400: 2020 2020 2020 202b 2063 6f6c 6f72 5465         + colorTe
-00018410: 7874 2e45 4e44 0d0a 2020 2020 2020 2020  xt.END..        
-00018420: 2020 2020 2b20 7374 7265 6e67 7468 5465      + strengthTe
-00018430: 7874 0d0a 2020 2020 2020 2020 290d 0a0d  xt..        )...
-00018440: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00018450: 7072 6564 2c20 7072 6564 6963 7469 6f6e  pred, prediction
-00018460: 5465 7874 2e72 6570 6c61 6365 286f 7574  Text.replace(out
-00018470: 2c20 6f75 7454 6578 7429 2c20 7374 7265  , outText), stre
-00018480: 6e67 7468 5465 7874 0d0a 0d0a 2020 2020  ngthText....    
-00018490: 6465 6620 6d6f 6e69 746f 7246 6976 6545  def monitorFiveE
-000184a0: 6d61 2873 656c 662c 2066 6574 6368 6572  ma(self, fetcher
-000184b0: 2c20 7265 7375 6c74 5f64 662c 206c 6173  , result_df, las
-000184c0: 745f 7369 676e 616c 2c20 7269 736b 5f72  t_signal, risk_r
-000184d0: 6577 6172 643d 3329 3a0d 0a20 2020 2020  eward=3):..     
-000184e0: 2020 2063 6f6c 5f6e 616d 6573 203d 205b     col_names = [
-000184f0: 2248 6967 6822 2c20 224c 6f77 222c 2022  "High", "Low", "
-00018500: 436c 6f73 6522 2c20 2235 454d 4122 5d0d  Close", "5EMA"].
-00018510: 0a20 2020 2020 2020 2064 6174 615f 6c69  .        data_li
-00018520: 7374 203d 205b 226e 6966 7479 5f62 7579  st = ["nifty_buy
-00018530: 222c 2022 6261 6e6b 6e69 6674 795f 6275  ", "banknifty_bu
-00018540: 7922 2c20 226e 6966 7479 5f73 656c 6c22  y", "nifty_sell"
-00018550: 2c20 2262 616e 6b6e 6966 7479 5f73 656c  , "banknifty_sel
-00018560: 6c22 5d0d 0a0d 0a20 2020 2020 2020 2064  l"]....        d
-00018570: 6174 615f 7475 706c 6520 3d20 6665 7463  ata_tuple = fetc
-00018580: 6865 722e 6665 7463 6846 6976 6545 6d61  her.fetchFiveEma
-00018590: 4461 7461 2829 0d0a 2020 2020 2020 2020  Data()..        
-000185a0: 666f 7220 636e 7420 696e 2072 616e 6765  for cnt in range
-000185b0: 286c 656e 2864 6174 615f 7475 706c 6529  (len(data_tuple)
-000185c0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-000185d0: 6420 3d20 6461 7461 5f74 7570 6c65 5b63  d = data_tuple[c
-000185e0: 6e74 5d0d 0a20 2020 2020 2020 2020 2020  nt]..           
-000185f0: 2064 5b22 3545 4d41 225d 203d 2070 6b74   d["5EMA"] = pkt
-00018600: 616c 6962 2e45 4d41 2864 5b22 436c 6f73  alib.EMA(d["Clos
-00018610: 6522 5d2c 2074 696d 6570 6572 696f 643d  e"], timeperiod=
-00018620: 3529 0d0a 2020 2020 2020 2020 2020 2020  5)..            
-00018630: 6420 3d20 645b 636f 6c5f 6e61 6d65 735d  d = d[col_names]
-00018640: 0d0a 2020 2020 2020 2020 2020 2020 6420  ..            d 
-00018650: 3d20 642e 6472 6f70 6e61 2829 2e72 6f75  = d.dropna().rou
-00018660: 6e64 2832 290d 0a0d 0a20 2020 2020 2020  nd(2)....       
-00018670: 2020 2020 2077 6974 6820 5375 7070 7265       with Suppre
-00018680: 7373 4f75 7470 7574 2873 7570 7072 6573  ssOutput(suppres
-00018690: 735f 7374 6465 7272 3d54 7275 652c 2073  s_stderr=True, s
-000186a0: 7570 7072 6573 735f 7374 646f 7574 3d54  uppress_stdout=T
-000186b0: 7275 6529 3a0d 0a20 2020 2020 2020 2020  rue):..         
-000186c0: 2020 2020 2020 2069 6620 2273 656c 6c22         if "sell"
-000186d0: 2069 6e20 6461 7461 5f6c 6973 745b 636e   in data_list[cn
-000186e0: 745d 3a0d 0a20 2020 2020 2020 2020 2020  t]:..           
-000186f0: 2020 2020 2020 2020 2073 7472 6563 6865           streche
-00018700: 6420 3d20 645b 2864 2e4c 6f77 203e 2064  d = d[(d.Low > d
-00018710: 5b22 3545 4d41 225d 2920 2620 2864 2e4c  ["5EMA"]) & (d.L
-00018720: 6f77 202d 2064 5b22 3545 4d41 225d 203e  ow - d["5EMA"] >
-00018730: 2030 2e35 295d 0d0a 2020 2020 2020 2020   0.5)]..        
-00018740: 2020 2020 2020 2020 2020 2020 7374 7265              stre
-00018750: 6368 6564 5b22 534c 225d 203d 2073 7472  ched["SL"] = str
-00018760: 6563 6865 642e 4869 6768 0d0a 2020 2020  eched.High..    
-00018770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018780: 7661 6c69 6461 7465 203d 2064 5b0d 0a20  validate = d[.. 
-00018790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000187a0: 2020 2020 2020 2028 642e 4c6f 772e 7368         (d.Low.sh
-000187b0: 6966 7428 3129 203e 2064 5b22 3545 4d41  ift(1) > d["5EMA
-000187c0: 225d 2e73 6869 6674 2831 2929 0d0a 2020  "].shift(1))..  
-000187d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000187e0: 2020 2020 2020 2620 2864 2e4c 6f77 2e73        & (d.Low.s
-000187f0: 6869 6674 2831 2920 2d20 645b 2235 454d  hift(1) - d["5EM
-00018800: 4122 5d2e 7368 6966 7428 3129 203e 2030  A"].shift(1) > 0
-00018810: 2e35 290d 0a20 2020 2020 2020 2020 2020  .5)..           
-00018820: 2020 2020 2020 2020 205d 0d0a 2020 2020           ]..    
-00018830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018840: 6f6c 645f 696e 6465 7820 3d20 7661 6c69  old_index = vali
-00018850: 6461 7465 2e69 6e64 6578 0d0a 2020 2020  date.index..    
-00018860: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00018870: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00018880: 2020 2020 2020 206d 6173 6b20 3d20 2864         mask = (d
-00018890: 2e48 6967 6820 3c20 645b 2235 454d 4122  .High < d["5EMA"
-000188a0: 5d29 2026 2028 645b 2235 454d 4122 5d20  ]) & (d["5EMA"] 
-000188b0: 2d20 642e 4869 6768 203e 2030 2e35 2920  - d.High > 0.5) 
-000188c0: 2023 2042 7579 0d0a 2020 2020 2020 2020   # Buy..        
-000188d0: 2020 2020 2020 2020 2020 2020 7374 7265              stre
-000188e0: 6368 6564 203d 2064 5b6d 6173 6b5d 0d0a  ched = d[mask]..
-000188f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018900: 2020 2020 7374 7265 6368 6564 5b22 534c      streched["SL
-00018910: 225d 203d 2073 7472 6563 6865 642e 4c6f  "] = streched.Lo
-00018920: 770d 0a20 2020 2020 2020 2020 2020 2020  w..             
-00018930: 2020 2020 2020 2076 616c 6964 6174 6520         validate 
-00018940: 3d20 642e 6c6f 635b 6d61 736b 2e73 6869  = d.loc[mask.shi
-00018950: 6674 2831 292e 6669 6c6c 6e61 2846 616c  ft(1).fillna(Fal
-00018960: 7365 295d 0d0a 2020 2020 2020 2020 2020  se)]..          
-00018970: 2020 2020 2020 2020 2020 6f6c 645f 696e            old_in
-00018980: 6465 7820 3d20 7661 6c69 6461 7465 2e69  dex = validate.i
-00018990: 6e64 6578 0d0a 2020 2020 2020 2020 2020  ndex..          
-000189a0: 2020 7467 7420 3d20 7064 2e44 6174 6146    tgt = pd.DataF
-000189b0: 7261 6d65 280d 0a20 2020 2020 2020 2020  rame(..         
-000189c0: 2020 2020 2020 2028 0d0a 2020 2020 2020         (..      
-000189d0: 2020 2020 2020 2020 2020 2020 2020 7661                va
-000189e0: 6c69 6461 7465 2e43 6c6f 7365 2e72 6573  lidate.Close.res
-000189f0: 6574 5f69 6e64 6578 2864 726f 703d 5472  et_index(drop=Tr
-00018a00: 7565 290d 0a20 2020 2020 2020 2020 2020  ue)..           
-00018a10: 2020 2020 2020 2020 202d 2028 0d0a 2020           - (..  
+00016fa0: 2020 2020 2070 6173 730d 0a20 2020 2020       pass..     
+00016fb0: 2020 206c 6173 7444 6179 4c61 7374 4d6f     lastDayLastMo
+00016fc0: 6e74 6820 3d20 6c61 7374 4461 794c 6173  nth = lastDayLas
+00016fd0: 744d 6f6e 7468 2e73 7472 6674 696d 6528  tMonth.strftime(
+00016fe0: 2225 592d 256d 2d25 6454 3030 3a30 303a  "%Y-%m-%dT00:00:
+00016ff0: 3030 2e30 3030 2229 0d0a 2020 2020 2020  00.000")..      
+00017000: 2020 6966 206f 6e6c 794d 463a 0d0a 2020    if onlyMF:..  
+00017010: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00017020: 206e 6574 4368 616e 6765 4d46 0d0a 2020   netChangeMF..  
+00017030: 2020 2020 2020 6966 206c 6174 6573 745f        if latest_
+00017040: 696e 7374 6461 7465 203d 3d20 6c61 7465  instdate == late
+00017050: 7374 5f6d 6664 6174 653a 0d0a 2020 2020  st_mfdate:..    
+00017060: 2020 2020 2020 2020 7265 7475 726e 2028          return (
+00017070: 6e65 7443 6861 6e67 654d 4620 2b20 6e65  netChangeMF + ne
+00017080: 7443 6861 6e67 6549 6e73 7429 0d0a 2020  tChangeInst)..  
+00017090: 2020 2020 2020 656c 6966 206c 6174 6573        elif lates
+000170a0: 745f 6d66 6461 7465 203d 3d20 6c61 7374  t_mfdate == last
+000170b0: 4461 794c 6173 744d 6f6e 7468 3a0d 0a20  DayLastMonth:.. 
+000170c0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000170d0: 6e20 6e65 7443 6861 6e67 654d 460d 0a20  n netChangeMF.. 
+000170e0: 2020 2020 2020 2065 6c69 6620 6c61 7465         elif late
+000170f0: 7374 5f69 6e73 7464 6174 6520 3d3d 206c  st_instdate == l
+00017100: 6173 7444 6179 4c61 7374 4d6f 6e74 683a  astDayLastMonth:
+00017110: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00017120: 7475 726e 206e 6574 4368 616e 6765 496e  turn netChangeIn
+00017130: 7374 0d0a 2020 2020 2020 2020 656c 7365  st..        else
+00017140: 3a0d 0a20 2020 2020 2020 2020 2020 2023  :..            #
+00017150: 2066 696e 6420 7468 6520 6c61 7465 7374   find the latest
+00017160: 2064 6174 650d 0a20 2020 2020 2020 2020   date..         
+00017170: 2020 2069 6620 6c61 7465 7374 5f6d 6664     if latest_mfd
+00017180: 6174 6520 6973 206e 6f74 204e 6f6e 653a  ate is not None:
+00017190: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000171a0: 2020 6c61 7465 7374 5f6d 6664 6174 6520    latest_mfdate 
+000171b0: 3d20 504b 4461 7465 5574 696c 6974 6965  = PKDateUtilitie
+000171c0: 732e 6461 7465 4672 6f6d 596d 6453 7472  s.dateFromYmdStr
+000171d0: 696e 6728 6c61 7465 7374 5f6d 6664 6174  ing(latest_mfdat
+000171e0: 652e 7370 6c69 7428 2254 2229 5b30 5d29  e.split("T")[0])
+000171f0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00017200: 206c 6174 6573 745f 696e 7374 6461 7465   latest_instdate
+00017210: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
+00017220: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00017230: 6174 6573 745f 696e 7374 6461 7465 203d  atest_instdate =
+00017240: 2050 4b44 6174 6555 7469 6c69 7469 6573   PKDateUtilities
+00017250: 2e64 6174 6546 726f 6d59 6d64 5374 7269  .dateFromYmdStri
+00017260: 6e67 286c 6174 6573 745f 696e 7374 6461  ng(latest_instda
+00017270: 7465 2e73 706c 6974 2822 5422 295b 305d  te.split("T")[0]
+00017280: 290d 0a20 2020 2020 2020 2020 2020 2072  )..            r
+00017290: 6574 7572 6e20 6e65 7443 6861 6e67 654d  eturn netChangeM
+000172a0: 4620 6966 2028 286c 6174 6573 745f 6d66  F if ((latest_mf
+000172b0: 6461 7465 2069 7320 6e6f 7420 4e6f 6e65  date is not None
+000172c0: 2920 616e 6420 6c61 7465 7374 5f6d 6664  ) and latest_mfd
+000172d0: 6174 6520 3e20 286c 6174 6573 745f 696e  ate > (latest_in
+000172e0: 7374 6461 7465 2069 6620 6c61 7465 7374  stdate if latest
+000172f0: 5f69 6e73 7464 6174 6520 6973 206e 6f74  _instdate is not
+00017300: 204e 6f6e 6520 656c 7365 2028 6c61 7465   None else (late
+00017310: 7374 5f6d 6664 6174 6520 2d20 6461 7465  st_mfdate - date
+00017320: 7469 6d65 2e74 696d 6564 656c 7461 2831  time.timedelta(1
+00017330: 2929 2929 2065 6c73 6520 6e65 7443 6861  )))) else netCha
+00017340: 6e67 6549 6e73 740d 0a0d 0a20 2020 2064  ngeInst....    d
+00017350: 6566 2067 6574 4672 6573 684d 4649 5374  ef getFreshMFISt
+00017360: 6174 7573 2873 656c 662c 2073 746f 636b  atus(self, stock
+00017370: 2c65 7863 6861 6e67 654e 616d 653d 2249  ,exchangeName="I
+00017380: 4e44 4941 2229 3a0d 0a20 2020 2020 2020  NDIA"):..       
+00017390: 2063 6861 6e67 6553 7461 7475 7344 6174   changeStatusDat
+000173a0: 614d 4620 3d20 4e6f 6e65 0d0a 2020 2020  aMF = None..    
+000173b0: 2020 2020 6368 616e 6765 5374 6174 7573      changeStatus
+000173c0: 4461 7461 496e 7374 203d 204e 6f6e 650d  DataInst = None.
+000173d0: 0a20 2020 2020 2020 206e 6574 4368 616e  .        netChan
+000173e0: 6765 4d46 203d 2030 0d0a 2020 2020 2020  geMF = 0..      
+000173f0: 2020 6e65 7443 6861 6e67 6549 6e73 7420    netChangeInst 
+00017400: 3d20 300d 0a20 2020 2020 2020 206c 6174  = 0..        lat
+00017410: 6573 745f 6d66 6461 7465 203d 204e 6f6e  est_mfdate = Non
+00017420: 650d 0a20 2020 2020 2020 206c 6174 6573  e..        lates
+00017430: 745f 696e 7374 6461 7465 203d 204e 6f6e  t_instdate = Non
+00017440: 650d 0a20 2020 2020 2020 2073 6563 7572  e..        secur
+00017450: 6974 7920 3d20 4e6f 6e65 0d0a 2020 2020  ity = None..    
+00017460: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
+00017470: 2020 2020 2020 7769 7468 2053 7570 7072        with Suppr
+00017480: 6573 734f 7574 7075 7428 7375 7070 7265  essOutput(suppre
+00017490: 7373 5f73 7464 6572 723d 5472 7565 2c20  ss_stderr=True, 
+000174a0: 7375 7070 7265 7373 5f73 7464 6f75 743d  suppress_stdout=
+000174b0: 5472 7565 293a 0d0a 2020 2020 2020 2020  True):..        
+000174c0: 2020 2020 2020 2020 7365 6375 7269 7479          security
+000174d0: 203d 2053 746f 636b 2873 746f 636b 2c65   = Stock(stock,e
+000174e0: 7863 6861 6e67 653d 6578 6368 616e 6765  xchange=exchange
+000174f0: 4e61 6d65 290d 0a20 2020 2020 2020 2065  Name)..        e
+00017500: 7863 6570 7420 5661 6c75 6545 7272 6f72  xcept ValueError
+00017510: 3a0d 0a20 2020 2020 2020 2020 2020 2023  :..            #
+00017520: 2057 6520 6469 6420 6e6f 7420 6669 6e64   We did not find
+00017530: 2074 6865 2073 746f 636b 3f20 4974 2773   the stock? It's
+00017540: 206f 6b61 792e 204d 6f76 6520 6f6e 2074   okay. Move on t
+00017550: 6f20 7468 6520 6e65 7874 206f 6e65 2e0d  o the next one..
+00017560: 0a20 2020 2020 2020 2020 2020 2070 6173  .            pas
+00017570: 730d 0a20 2020 2020 2020 2069 6620 7365  s..        if se
+00017580: 6375 7269 7479 2069 7320 6e6f 7420 4e6f  curity is not No
+00017590: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+000175a0: 2074 7279 3a0d 0a20 2020 2020 2020 2020   try:..         
+000175b0: 2020 2020 2020 2077 6974 6820 5375 7070         with Supp
+000175c0: 7265 7373 4f75 7470 7574 2873 7570 7072  ressOutput(suppr
+000175d0: 6573 735f 7374 6465 7272 3d54 7275 652c  ess_stderr=True,
+000175e0: 2073 7570 7072 6573 735f 7374 646f 7574   suppress_stdout
+000175f0: 3d54 7275 6529 3a0d 0a20 2020 2020 2020  =True):..       
+00017600: 2020 2020 2020 2020 2020 2020 2063 6861               cha
+00017610: 6e67 6553 7461 7475 7352 6f77 734d 4620  ngeStatusRowsMF 
+00017620: 3d20 7365 6375 7269 7479 2e6d 7574 7561  = security.mutua
+00017630: 6c46 756e 644f 776e 6572 7368 6970 2874  lFundOwnership(t
+00017640: 6f70 3d35 290d 0a20 2020 2020 2020 2020  op=5)..         
+00017650: 2020 2020 2020 2020 2020 2063 6861 6e67             chang
+00017660: 6553 7461 7475 7352 6f77 7349 6e73 7420  eStatusRowsInst 
+00017670: 3d20 7365 6375 7269 7479 2e69 6e73 7469  = security.insti
+00017680: 7475 7469 6f6e 4f77 6e65 7273 6869 7028  tutionOwnership(
+00017690: 746f 703d 3529 0d0a 2020 2020 2020 2020  top=5)..        
+000176a0: 2020 2020 2020 2020 2020 2020 6368 616e              chan
+000176b0: 6765 5374 6174 7573 4461 7461 4d46 203d  geStatusDataMF =
+000176c0: 2073 6563 7572 6974 792e 6d75 7475 616c   security.mutual
+000176d0: 4675 6e64 4649 4943 6861 6e67 6544 6174  FundFIIChangeDat
+000176e0: 6128 6368 616e 6765 5374 6174 7573 526f  a(changeStatusRo
+000176f0: 7773 4d46 290d 0a20 2020 2020 2020 2020  wsMF)..         
+00017700: 2020 2020 2020 2020 2020 2063 6861 6e67             chang
+00017710: 6553 7461 7475 7344 6174 6149 6e73 7420  eStatusDataInst 
+00017720: 3d20 7365 6375 7269 7479 2e6d 7574 7561  = security.mutua
+00017730: 6c46 756e 6446 4949 4368 616e 6765 4461  lFundFIIChangeDa
+00017740: 7461 2863 6861 6e67 6553 7461 7475 7352  ta(changeStatusR
+00017750: 6f77 7349 6e73 7429 0d0a 2020 2020 2020  owsInst)..      
+00017760: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
+00017770: 6570 7469 6f6e 2061 7320 653a 0d0a 2020  eption as e:..  
+00017780: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00017790: 6c66 2e64 6566 6175 6c74 5f6c 6f67 6765  lf.default_logge
+000177a0: 722e 6465 6275 6728 652c 2065 7863 5f69  r.debug(e, exc_i
+000177b0: 6e66 6f3d 5472 7565 290d 0a20 2020 2020  nfo=True)..     
+000177c0: 2020 2020 2020 2020 2020 2023 2054 7970             # Typ
+000177d0: 6545 7272 6f72 206f 7220 436f 6e6e 6563  eError or Connec
+000177e0: 7469 6f6e 4572 726f 7220 6265 6361 7573  tionError becaus
+000177f0: 6520 7765 2063 6f75 6c64 206e 6f74 2066  e we could not f
+00017800: 696e 6420 7468 6520 7374 6f63 6b20 6f72  ind the stock or
+00017810: 204d 4649 2064 6174 6120 6973 6e27 7420   MFI data isn't 
+00017820: 6176 6169 6c61 626c 653f 0d0a 2020 2020  available?..    
+00017830: 2020 2020 2020 2020 2020 2020 7061 7373              pass
+00017840: 0d0a 2020 2020 2020 2020 2020 2020 6c61  ..            la
+00017850: 7374 4461 794c 6173 744d 6f6e 7468 203d  stDayLastMonth =
+00017860: 2050 4b44 6174 6555 7469 6c69 7469 6573   PKDateUtilities
+00017870: 2e6c 6173 745f 6461 795f 6f66 5f70 7265  .last_day_of_pre
+00017880: 7669 6f75 735f 6d6f 6e74 6828 504b 4461  vious_month(PKDa
+00017890: 7465 5574 696c 6974 6965 732e 6375 7272  teUtilities.curr
+000178a0: 656e 7444 6174 6554 696d 6528 2929 0d0a  entDateTime())..
+000178b0: 2020 2020 2020 2020 2020 2020 6c61 7374              last
+000178c0: 4461 794c 6173 744d 6f6e 7468 203d 206c  DayLastMonth = l
+000178d0: 6173 7444 6179 4c61 7374 4d6f 6e74 682e  astDayLastMonth.
+000178e0: 7374 7266 7469 6d65 2822 2559 2d25 6d2d  strftime("%Y-%m-
+000178f0: 2564 5430 303a 3030 3a30 302e 3030 3022  %dT00:00:00.000"
+00017900: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
+00017910: 6620 6368 616e 6765 5374 6174 7573 4461  f changeStatusDa
+00017920: 7461 4d46 2069 7320 6e6f 7420 4e6f 6e65  taMF is not None
+00017930: 2061 6e64 206c 656e 2863 6861 6e67 6553   and len(changeS
+00017940: 7461 7475 7344 6174 614d 4629 203e 2030  tatusDataMF) > 0
+00017950: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00017960: 2020 2064 665f 6772 6f75 7065 644d 4620     df_groupedMF 
+00017970: 3d20 6368 616e 6765 5374 6174 7573 4461  = changeStatusDa
+00017980: 7461 4d46 2e67 726f 7570 6279 2822 6461  taMF.groupby("da
+00017990: 7465 222c 2073 6f72 743d 4661 6c73 6529  te", sort=False)
+000179a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000179b0: 2020 666f 7220 6d66 6461 7465 2c20 6466    for mfdate, df
+000179c0: 5f67 726f 7570 4d46 2069 6e20 6466 5f67  _groupMF in df_g
+000179d0: 726f 7570 6564 4d46 3a0d 0a20 2020 2020  roupedMF:..     
+000179e0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+000179f0: 6574 4368 616e 6765 4d46 203d 2064 665f  etChangeMF = df_
+00017a00: 6772 6f75 704d 465b 2263 6861 6e67 6541  groupMF["changeA
+00017a10: 6d6f 756e 7422 5d2e 7375 6d28 290d 0a20  mount"].sum().. 
+00017a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017a30: 2020 206c 6174 6573 745f 6d66 6461 7465     latest_mfdate
+00017a40: 203d 206d 6664 6174 650d 0a20 2020 2020   = mfdate..     
+00017a50: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+00017a60: 7265 616b 0d0a 2020 2020 2020 2020 2020  reak..          
+00017a70: 2020 6966 2063 6861 6e67 6553 7461 7475    if changeStatu
+00017a80: 7344 6174 6149 6e73 7420 6973 206e 6f74  sDataInst is not
+00017a90: 204e 6f6e 6520 616e 6420 6c65 6e28 6368   None and len(ch
+00017aa0: 616e 6765 5374 6174 7573 4461 7461 496e  angeStatusDataIn
+00017ab0: 7374 2920 3e20 303a 0d0a 2020 2020 2020  st) > 0:..      
+00017ac0: 2020 2020 2020 2020 2020 6466 5f67 726f            df_gro
+00017ad0: 7570 6564 496e 7374 203d 2063 6861 6e67  upedInst = chang
+00017ae0: 6553 7461 7475 7344 6174 6149 6e73 742e  eStatusDataInst.
+00017af0: 6772 6f75 7062 7928 2264 6174 6522 2c20  groupby("date", 
+00017b00: 736f 7274 3d46 616c 7365 290d 0a20 2020  sort=False)..   
+00017b10: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00017b20: 2069 6e73 7464 6174 652c 2064 665f 6772   instdate, df_gr
+00017b30: 6f75 7049 6e73 7420 696e 2064 665f 6772  oupInst in df_gr
+00017b40: 6f75 7065 6449 6e73 743a 0d0a 2020 2020  oupedInst:..    
+00017b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017b60: 6966 2028 6c61 7465 7374 5f6d 6664 6174  if (latest_mfdat
+00017b70: 6520 6973 206e 6f74 204e 6f6e 6520 616e  e is not None an
+00017b80: 6420 6c61 7465 7374 5f6d 6664 6174 6520  d latest_mfdate 
+00017b90: 3d3d 2069 6e73 7464 6174 6529 206f 7220  == instdate) or 
+00017ba0: 286c 6174 6573 745f 6d66 6461 7465 2069  (latest_mfdate i
+00017bb0: 7320 4e6f 6e65 2920 6f72 2028 696e 7374  s None) or (inst
+00017bc0: 6461 7465 203d 3d20 6c61 7374 4461 794c  date == lastDayL
+00017bd0: 6173 744d 6f6e 7468 293a 0d0a 2020 2020  astMonth):..    
+00017be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017bf0: 2020 2020 6e65 7443 6861 6e67 6549 6e73      netChangeIns
+00017c00: 7420 3d20 6466 5f67 726f 7570 496e 7374  t = df_groupInst
+00017c10: 5b22 6368 616e 6765 416d 6f75 6e74 225d  ["changeAmount"]
+00017c20: 2e73 756d 2829 0d0a 2020 2020 2020 2020  .sum()..        
+00017c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017c40: 6c61 7465 7374 5f69 6e73 7464 6174 6520  latest_instdate 
+00017c50: 3d20 696e 7374 6461 7465 0d0a 2020 2020  = instdate..    
+00017c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017c70: 6272 6561 6b0d 0a20 2020 2020 2020 2072  break..        r
+00017c80: 6574 7572 6e20 6e65 7443 6861 6e67 654d  eturn netChangeM
+00017c90: 462c 6e65 7443 6861 6e67 6549 6e73 742c  F,netChangeInst,
+00017ca0: 6c61 7465 7374 5f6d 6664 6174 652c 6c61  latest_mfdate,la
+00017cb0: 7465 7374 5f69 6e73 7464 6174 650d 0a0d  test_instdate...
+00017cc0: 0a0d 0a20 2020 2064 6566 2067 6574 4e69  ...    def getNi
+00017cd0: 6674 7950 7265 6469 6374 696f 6e28 7365  ftyPrediction(se
+00017ce0: 6c66 2c20 6466 293a 0d0a 2020 2020 2020  lf, df):..      
+00017cf0: 2020 696d 706f 7274 2077 6172 6e69 6e67    import warning
+00017d00: 730d 0a0d 0a20 2020 2020 2020 2077 6172  s....        war
+00017d10: 6e69 6e67 732e 6669 6c74 6572 7761 726e  nings.filterwarn
+00017d20: 696e 6773 2822 6967 6e6f 7265 2229 0d0a  ings("ignore")..
+00017d30: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
+00017d40: 662e 636f 7079 2829 0d0a 2020 2020 2020  f.copy()..      
+00017d50: 2020 6d6f 6465 6c2c 2070 6b6c 203d 2055    model, pkl = U
+00017d60: 7469 6c69 7479 2e74 6f6f 6c73 2e67 6574  tility.tools.get
+00017d70: 4e69 6674 794d 6f64 656c 2829 0d0a 2020  NiftyModel()..  
+00017d80: 2020 2020 2020 6966 206d 6f64 656c 2069        if model i
+00017d90: 7320 4e6f 6e65 206f 7220 706b 6c20 6973  s None or pkl is
+00017da0: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+00017db0: 2020 2020 7265 7475 726e 2030 2c20 2255      return 0, "U
+00017dc0: 6e6b 6e6f 776e 222c 2022 556e 6b6e 6f77  nknown", "Unknow
+00017dd0: 6e22 0d0a 2020 2020 2020 2020 7769 7468  n"..        with
+00017de0: 2053 7570 7072 6573 734f 7574 7075 7428   SuppressOutput(
+00017df0: 7375 7070 7265 7373 5f73 7464 6572 723d  suppress_stderr=
+00017e00: 5472 7565 2c20 7375 7070 7265 7373 5f73  True, suppress_s
+00017e10: 7464 6f75 743d 5472 7565 293a 0d0a 2020  tdout=True):..  
+00017e20: 2020 2020 2020 2020 2020 6461 7461 203d            data =
+00017e30: 2064 6174 615b 706b 6c5b 2263 6f6c 756d   data[pkl["colum
+00017e40: 6e73 225d 5d0d 0a20 2020 2020 2020 2020  ns"]]..         
+00017e50: 2020 2023 2323 2076 3220 5072 6570 726f     ### v2 Prepro
+00017e60: 6365 7373 696e 670d 0a20 2020 2020 2020  cessing..       
+00017e70: 2020 2020 2064 6174 615b 2248 6967 6822       data["High"
+00017e80: 5d20 3d20 6461 7461 5b22 4869 6768 225d  ] = data["High"]
+00017e90: 2e70 6374 5f63 6861 6e67 6528 2920 2a20  .pct_change() * 
+00017ea0: 3130 300d 0a20 2020 2020 2020 2020 2020  100..           
+00017eb0: 2064 6174 615b 224c 6f77 225d 203d 2064   data["Low"] = d
+00017ec0: 6174 615b 224c 6f77 225d 2e70 6374 5f63  ata["Low"].pct_c
+00017ed0: 6861 6e67 6528 2920 2a20 3130 300d 0a20  hange() * 100.. 
+00017ee0: 2020 2020 2020 2020 2020 2064 6174 615b             data[
+00017ef0: 224f 7065 6e22 5d20 3d20 6461 7461 5b22  "Open"] = data["
+00017f00: 4f70 656e 225d 2e70 6374 5f63 6861 6e67  Open"].pct_chang
+00017f10: 6528 2920 2a20 3130 300d 0a20 2020 2020  e() * 100..     
+00017f20: 2020 2020 2020 2064 6174 615b 2243 6c6f         data["Clo
+00017f30: 7365 225d 203d 2064 6174 615b 2243 6c6f  se"] = data["Clo
+00017f40: 7365 225d 2e70 6374 5f63 6861 6e67 6528  se"].pct_change(
+00017f50: 2920 2a20 3130 300d 0a20 2020 2020 2020  ) * 100..       
+00017f60: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
+00017f70: 2e69 6c6f 635b 2d31 5d0d 0a20 2020 2020  .iloc[-1]..     
+00017f80: 2020 2020 2020 2023 2323 0d0a 2020 2020         ###..    
+00017f90: 2020 2020 2020 2020 6461 7461 203d 2070          data = p
+00017fa0: 6b6c 5b22 7363 616c 6572 225d 2e74 7261  kl["scaler"].tra
+00017fb0: 6e73 666f 726d 285b 6461 7461 5d29 0d0a  nsform([data])..
+00017fc0: 2020 2020 2020 2020 2020 2020 7769 7468              with
+00017fd0: 2053 7570 7072 6573 734f 7574 7075 7428   SuppressOutput(
+00017fe0: 7375 7070 7265 7373 5f73 7464 6f75 743d  suppress_stdout=
+00017ff0: 5472 7565 2c20 7375 7070 7265 7373 5f73  True, suppress_s
+00018000: 7464 6572 723d 5472 7565 293a 0d0a 2020  tderr=True):..  
+00018010: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00018020: 6564 203d 206d 6f64 656c 2e70 7265 6469  ed = model.predi
+00018030: 6374 2864 6174 6129 5b30 5d0d 0a20 2020  ct(data)[0]..   
+00018040: 2020 2020 2069 6620 7072 6564 203e 2030       if pred > 0
+00018050: 2e35 3a0d 0a20 2020 2020 2020 2020 2020  .5:..           
+00018060: 206f 7574 5465 7874 203d 2022 4245 4152   outText = "BEAR
+00018070: 4953 4822 0d0a 2020 2020 2020 2020 2020  ISH"..          
+00018080: 2020 6f75 7420 3d20 280d 0a20 2020 2020    out = (..     
+00018090: 2020 2020 2020 2020 2020 2063 6f6c 6f72             color
+000180a0: 5465 7874 2e42 4f4c 440d 0a20 2020 2020  Text.BOLD..     
+000180b0: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
+000180c0: 6f72 5465 7874 2e46 4149 4c0d 0a20 2020  orText.FAIL..   
+000180d0: 2020 2020 2020 2020 2020 2020 202b 206f               + o
+000180e0: 7574 5465 7874 0d0a 2020 2020 2020 2020  utText..        
+000180f0: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
+00018100: 6578 742e 454e 440d 0a20 2020 2020 2020  ext.END..       
+00018110: 2020 2020 2020 2020 202b 2063 6f6c 6f72           + color
+00018120: 5465 7874 2e42 4f4c 440d 0a20 2020 2020  Text.BOLD..     
+00018130: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+00018140: 2020 2020 2020 7375 6720 3d20 2248 6f6c        sug = "Hol
+00018150: 6420 796f 7572 2053 686f 7274 2070 6f73  d your Short pos
+00018160: 6974 696f 6e21 220d 0a20 2020 2020 2020  ition!"..       
+00018170: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+00018180: 2020 2020 6f75 7454 6578 7420 3d20 2242      outText = "B
+00018190: 554c 4c49 5348 220d 0a20 2020 2020 2020  ULLISH"..       
+000181a0: 2020 2020 206f 7574 203d 2028 0d0a 2020       out = (..  
+000181b0: 2020 2020 2020 2020 2020 2020 2020 636f                co
+000181c0: 6c6f 7254 6578 742e 424f 4c44 0d0a 2020  lorText.BOLD..  
+000181d0: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+000181e0: 636f 6c6f 7254 6578 742e 4752 4545 4e0d  colorText.GREEN.
+000181f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018200: 202b 206f 7574 5465 7874 0d0a 2020 2020   + outText..    
+00018210: 2020 2020 2020 2020 2020 2020 2b20 636f              + co
+00018220: 6c6f 7254 6578 742e 454e 440d 0a20 2020  lorText.END..   
+00018230: 2020 2020 2020 2020 2020 2020 202b 2063               + c
+00018240: 6f6c 6f72 5465 7874 2e42 4f4c 440d 0a20  olorText.BOLD.. 
+00018250: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
+00018260: 2020 2020 2020 2020 2020 7375 6720 3d20            sug = 
+00018270: 2253 7461 7920 4275 6c6c 6973 6821 220d  "Stay Bullish!".
+00018280: 0a20 2020 2020 2020 2069 6620 504b 4461  .        if PKDa
+00018290: 7465 5574 696c 6974 6965 732e 6973 436c  teUtilities.isCl
+000182a0: 6f73 696e 6748 6f75 7228 293a 0d0a 2020  osingHour():..  
+000182b0: 2020 2020 2020 2020 2020 4f75 7470 7574            Output
+000182c0: 436f 6e74 726f 6c73 2829 2e70 7269 6e74  Controls().print
+000182d0: 4f75 7470 7574 280d 0a20 2020 2020 2020  Output(..       
+000182e0: 2020 2020 2020 2020 2063 6f6c 6f72 5465           colorTe
+000182f0: 7874 2e42 4f4c 440d 0a20 2020 2020 2020  xt.BOLD..       
+00018300: 2020 2020 2020 2020 202b 2063 6f6c 6f72           + color
+00018310: 5465 7874 2e57 4152 4e0d 0a20 2020 2020  Text.WARN..     
+00018320: 2020 2020 2020 2020 2020 202b 2022 4e6f             + "No
+00018330: 7465 3a20 5468 6520 4149 2070 7265 6469  te: The AI predi
+00018340: 6374 696f 6e20 7368 6f75 6c64 2062 6520  ction should be 
+00018350: 6578 6563 7574 6564 2041 6674 6572 2033  executed After 3
+00018360: 2050 4d20 6f72 204e 6561 7220 746f 2043   PM or Near to C
+00018370: 6c6f 7369 6e67 2074 696d 6520 6173 2074  losing time as t
+00018380: 6865 2050 7265 6469 6374 696f 6e20 4163  he Prediction Ac
+00018390: 6375 7261 6379 2069 7320 6261 7365 6420  curacy is based 
+000183a0: 6f6e 2074 6865 2043 6c6f 7369 6e67 2070  on the Closing p
+000183b0: 7269 6365 2122 0d0a 2020 2020 2020 2020  rice!"..        
+000183c0: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
+000183d0: 6578 742e 454e 440d 0a20 2020 2020 2020  ext.END..       
+000183e0: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+000183f0: 7072 6564 6963 7469 6f6e 5465 7874 203d  predictionText =
+00018400: 2022 4d61 726b 6574 206d 6179 204f 7065   "Market may Ope
+00018410: 6e20 7b7d 206e 6578 7420 6461 7921 207b  n {} next day! {
+00018420: 7d22 2e66 6f72 6d61 7428 6f75 742c 2073  }".format(out, s
+00018430: 7567 290d 0a20 2020 2020 2020 2073 7472  ug)..        str
+00018440: 656e 6774 6854 6578 7420 3d20 2250 726f  engthText = "Pro
+00018450: 6261 6269 6c69 7479 2f53 7472 656e 6774  bability/Strengt
+00018460: 6820 6f66 2050 7265 6469 6374 696f 6e20  h of Prediction 
+00018470: 3d20 7b7d 2522 2e66 6f72 6d61 7428 0d0a  = {}%".format(..
+00018480: 2020 2020 2020 2020 2020 2020 5574 696c              Util
+00018490: 6974 792e 746f 6f6c 732e 6765 7453 6967  ity.tools.getSig
+000184a0: 6d6f 6964 436f 6e66 6964 656e 6365 2870  moidConfidence(p
+000184b0: 7265 645b 305d 290d 0a20 2020 2020 2020  red[0])..       
+000184c0: 2029 0d0a 2020 2020 2020 2020 4f75 7470   )..        Outp
+000184d0: 7574 436f 6e74 726f 6c73 2829 2e70 7269  utControls().pri
+000184e0: 6e74 4f75 7470 7574 280d 0a20 2020 2020  ntOutput(..     
+000184f0: 2020 2020 2020 2063 6f6c 6f72 5465 7874         colorText
+00018500: 2e42 4f4c 440d 0a20 2020 2020 2020 2020  .BOLD..         
+00018510: 2020 202b 2063 6f6c 6f72 5465 7874 2e42     + colorText.B
+00018520: 4c55 450d 0a20 2020 2020 2020 2020 2020  LUE..           
+00018530: 202b 2022 5c6e 220d 0a20 2020 2020 2020   + "\n"..       
+00018540: 2020 2020 202b 2022 5b2b 5d20 4e69 6674       + "[+] Nift
+00018550: 7920 4149 2050 7265 6469 6374 696f 6e20  y AI Prediction 
+00018560: 2d3e 2022 0d0a 2020 2020 2020 2020 2020  -> "..          
+00018570: 2020 2b20 636f 6c6f 7254 6578 742e 454e    + colorText.EN
+00018580: 440d 0a20 2020 2020 2020 2020 2020 202b  D..            +
+00018590: 2063 6f6c 6f72 5465 7874 2e42 4f4c 440d   colorText.BOLD.
+000185a0: 0a20 2020 2020 2020 2020 2020 202b 2070  .            + p
+000185b0: 7265 6469 6374 696f 6e54 6578 740d 0a20  redictionText.. 
+000185c0: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
+000185d0: 6f72 5465 7874 2e45 4e44 0d0a 2020 2020  orText.END..    
+000185e0: 2020 2020 290d 0a20 2020 2020 2020 204f      )..        O
+000185f0: 7574 7075 7443 6f6e 7472 6f6c 7328 292e  utputControls().
+00018600: 7072 696e 744f 7574 7075 7428 0d0a 2020  printOutput(..  
+00018610: 2020 2020 2020 2020 2020 636f 6c6f 7254            colorT
+00018620: 6578 742e 424f 4c44 0d0a 2020 2020 2020  ext.BOLD..      
+00018630: 2020 2020 2020 2b20 636f 6c6f 7254 6578        + colorTex
+00018640: 742e 424c 5545 0d0a 2020 2020 2020 2020  t.BLUE..        
+00018650: 2020 2020 2b20 225c 6e22 0d0a 2020 2020      + "\n"..    
+00018660: 2020 2020 2020 2020 2b20 225b 2b5d 204e          + "[+] N
+00018670: 6966 7479 2041 4920 5072 6564 6963 7469  ifty AI Predicti
+00018680: 6f6e 202d 3e20 220d 0a20 2020 2020 2020  on -> "..       
+00018690: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
+000186a0: 2e45 4e44 0d0a 2020 2020 2020 2020 2020  .END..          
+000186b0: 2020 2b20 7374 7265 6e67 7468 5465 7874    + strengthText
+000186c0: 0d0a 2020 2020 2020 2020 290d 0a0d 0a20  ..        ).... 
+000186d0: 2020 2020 2020 2072 6574 7572 6e20 7072         return pr
+000186e0: 6564 2c20 7072 6564 6963 7469 6f6e 5465  ed, predictionTe
+000186f0: 7874 2e72 6570 6c61 6365 286f 7574 2c20  xt.replace(out, 
+00018700: 6f75 7454 6578 7429 2c20 7374 7265 6e67  outText), streng
+00018710: 7468 5465 7874 0d0a 0d0a 2020 2020 6465  thText....    de
+00018720: 6620 6d6f 6e69 746f 7246 6976 6545 6d61  f monitorFiveEma
+00018730: 2873 656c 662c 2066 6574 6368 6572 2c20  (self, fetcher, 
+00018740: 7265 7375 6c74 5f64 662c 206c 6173 745f  result_df, last_
+00018750: 7369 676e 616c 2c20 7269 736b 5f72 6577  signal, risk_rew
+00018760: 6172 643d 3329 3a0d 0a20 2020 2020 2020  ard=3):..       
+00018770: 2063 6f6c 5f6e 616d 6573 203d 205b 2248   col_names = ["H
+00018780: 6967 6822 2c20 224c 6f77 222c 2022 436c  igh", "Low", "Cl
+00018790: 6f73 6522 2c20 2235 454d 4122 5d0d 0a20  ose", "5EMA"].. 
+000187a0: 2020 2020 2020 2064 6174 615f 6c69 7374         data_list
+000187b0: 203d 205b 226e 6966 7479 5f62 7579 222c   = ["nifty_buy",
+000187c0: 2022 6261 6e6b 6e69 6674 795f 6275 7922   "banknifty_buy"
+000187d0: 2c20 226e 6966 7479 5f73 656c 6c22 2c20  , "nifty_sell", 
+000187e0: 2262 616e 6b6e 6966 7479 5f73 656c 6c22  "banknifty_sell"
+000187f0: 5d0d 0a0d 0a20 2020 2020 2020 2064 6174  ]....        dat
+00018800: 615f 7475 706c 6520 3d20 6665 7463 6865  a_tuple = fetche
+00018810: 722e 6665 7463 6846 6976 6545 6d61 4461  r.fetchFiveEmaDa
+00018820: 7461 2829 0d0a 2020 2020 2020 2020 666f  ta()..        fo
+00018830: 7220 636e 7420 696e 2072 616e 6765 286c  r cnt in range(l
+00018840: 656e 2864 6174 615f 7475 706c 6529 293a  en(data_tuple)):
+00018850: 0d0a 2020 2020 2020 2020 2020 2020 6420  ..            d 
+00018860: 3d20 6461 7461 5f74 7570 6c65 5b63 6e74  = data_tuple[cnt
+00018870: 5d0d 0a20 2020 2020 2020 2020 2020 2064  ]..            d
+00018880: 5b22 3545 4d41 225d 203d 2070 6b74 616c  ["5EMA"] = pktal
+00018890: 6962 2e45 4d41 2864 5b22 436c 6f73 6522  ib.EMA(d["Close"
+000188a0: 5d2c 2074 696d 6570 6572 696f 643d 3529  ], timeperiod=5)
+000188b0: 0d0a 2020 2020 2020 2020 2020 2020 6420  ..            d 
+000188c0: 3d20 645b 636f 6c5f 6e61 6d65 735d 0d0a  = d[col_names]..
+000188d0: 2020 2020 2020 2020 2020 2020 6420 3d20              d = 
+000188e0: 642e 6472 6f70 6e61 2829 2e72 6f75 6e64  d.dropna().round
+000188f0: 2832 290d 0a0d 0a20 2020 2020 2020 2020  (2)....         
+00018900: 2020 2077 6974 6820 5375 7070 7265 7373     with Suppress
+00018910: 4f75 7470 7574 2873 7570 7072 6573 735f  Output(suppress_
+00018920: 7374 6465 7272 3d54 7275 652c 2073 7570  stderr=True, sup
+00018930: 7072 6573 735f 7374 646f 7574 3d54 7275  press_stdout=Tru
+00018940: 6529 3a0d 0a20 2020 2020 2020 2020 2020  e):..           
+00018950: 2020 2020 2069 6620 2273 656c 6c22 2069       if "sell" i
+00018960: 6e20 6461 7461 5f6c 6973 745b 636e 745d  n data_list[cnt]
+00018970: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00018980: 2020 2020 2020 2073 7472 6563 6865 6420         streched 
+00018990: 3d20 645b 2864 2e4c 6f77 203e 2064 5b22  = d[(d.Low > d["
+000189a0: 3545 4d41 225d 2920 2620 2864 2e4c 6f77  5EMA"]) & (d.Low
+000189b0: 202d 2064 5b22 3545 4d41 225d 203e 2030   - d["5EMA"] > 0
+000189c0: 2e35 295d 0d0a 2020 2020 2020 2020 2020  .5)]..          
+000189d0: 2020 2020 2020 2020 2020 7374 7265 6368            strech
+000189e0: 6564 5b22 534c 225d 203d 2073 7472 6563  ed["SL"] = strec
+000189f0: 6865 642e 4869 6768 0d0a 2020 2020 2020  hed.High..      
+00018a00: 2020 2020 2020 2020 2020 2020 2020 7661                va
+00018a10: 6c69 6461 7465 203d 2064 5b0d 0a20 2020  lidate = d[..   
 00018a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018a30: 2020 2020 2020 280d 0a20 2020 2020 2020        (..       
-00018a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018a50: 2020 2020 2073 7472 6563 6865 642e 534c       streched.SL
-00018a60: 2e72 6573 6574 5f69 6e64 6578 2864 726f  .reset_index(dro
-00018a70: 703d 5472 7565 290d 0a20 2020 2020 2020  p=True)..       
-00018a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018a90: 2020 2020 202d 2076 616c 6964 6174 652e       - validate.
-00018aa0: 436c 6f73 652e 7265 7365 745f 696e 6465  Close.reset_inde
-00018ab0: 7828 6472 6f70 3d54 7275 6529 0d0a 2020  x(drop=True)..  
-00018ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ad0: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-00018ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018af0: 202a 2072 6973 6b5f 7265 7761 7264 0d0a   * risk_reward..
-00018b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018b10: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
-00018b20: 2020 2020 2020 2029 2c0d 0a20 2020 2020         ),..     
-00018b30: 2020 2020 2020 2020 2020 2063 6f6c 756d             colum
-00018b40: 6e73 3d5b 2254 6172 6765 7422 5d2c 0d0a  ns=["Target"],..
-00018b50: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
-00018b60: 2020 2020 2020 2020 2020 2076 616c 6964             valid
-00018b70: 6174 6520 3d20 7064 2e63 6f6e 6361 7428  ate = pd.concat(
-00018b80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018b90: 2020 5b0d 0a20 2020 2020 2020 2020 2020    [..           
-00018ba0: 2020 2020 2020 2020 2076 616c 6964 6174           validat
-00018bb0: 652e 7265 7365 745f 696e 6465 7828 6472  e.reset_index(dr
-00018bc0: 6f70 3d54 7275 6529 2c0d 0a20 2020 2020  op=True),..     
-00018bd0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00018be0: 7472 6563 6865 645b 2253 4c22 5d2e 7265  treched["SL"].re
-00018bf0: 7365 745f 696e 6465 7828 6472 6f70 3d54  set_index(drop=T
-00018c00: 7275 6529 2c0d 0a20 2020 2020 2020 2020  rue),..         
-00018c10: 2020 2020 2020 2020 2020 2074 6774 2c0d             tgt,.
-00018c20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018c30: 205d 2c0d 0a20 2020 2020 2020 2020 2020   ],..           
-00018c40: 2020 2020 2061 7869 733d 312c 0d0a 2020       axis=1,..  
-00018c50: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
-00018c60: 2020 2020 2020 2020 2076 616c 6964 6174           validat
-00018c70: 6520 3d20 7661 6c69 6461 7465 2e74 6169  e = validate.tai
-00018c80: 6c28 6c65 6e28 6f6c 645f 696e 6465 7829  l(len(old_index)
-00018c90: 290d 0a20 2020 2020 2020 2020 2020 2076  )..            v
-00018ca0: 616c 6964 6174 6520 3d20 7661 6c69 6461  alidate = valida
-00018cb0: 7465 2e73 6574 5f69 6e64 6578 286f 6c64  te.set_index(old
-00018cc0: 5f69 6e64 6578 290d 0a20 2020 2020 2020  _index)..       
-00018cd0: 2020 2020 2069 6620 2273 656c 6c22 2069       if "sell" i
-00018ce0: 6e20 6461 7461 5f6c 6973 745b 636e 745d  n data_list[cnt]
-00018cf0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00018d00: 2020 2066 696e 616c 203d 2076 616c 6964     final = valid
-00018d10: 6174 655b 7661 6c69 6461 7465 2e43 6c6f  ate[validate.Clo
-00018d20: 7365 203c 2076 616c 6964 6174 655b 2235  se < validate["5
-00018d30: 454d 4122 5d5d 2e74 6169 6c28 3129 0d0a  EMA"]].tail(1)..
-00018d40: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00018d50: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00018d60: 2020 2066 696e 616c 203d 2076 616c 6964     final = valid
-00018d70: 6174 655b 7661 6c69 6461 7465 2e43 6c6f  ate[validate.Clo
-00018d80: 7365 203e 2076 616c 6964 6174 655b 2235  se > validate["5
-00018d90: 454d 4122 5d5d 2e74 6169 6c28 3129 0d0a  EMA"]].tail(1)..
-00018da0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00018db0: 2064 6174 615f 6c69 7374 5b63 6e74 5d20   data_list[cnt] 
-00018dc0: 6e6f 7420 696e 206c 6173 745f 7369 676e  not in last_sign
-00018dd0: 616c 3a0d 0a20 2020 2020 2020 2020 2020  al:..           
-00018de0: 2020 2020 206c 6173 745f 7369 676e 616c       last_signal
-00018df0: 5b64 6174 615f 6c69 7374 5b63 6e74 5d5d  [data_list[cnt]]
-00018e00: 203d 2066 696e 616c 0d0a 2020 2020 2020   = final..      
-00018e10: 2020 2020 2020 656c 6966 2064 6174 615f        elif data_
-00018e20: 6c69 7374 5b63 6e74 5d20 696e 206c 6173  list[cnt] in las
-00018e30: 745f 7369 676e 616c 3a0d 0a20 2020 2020  t_signal:..     
-00018e40: 2020 2020 2020 2020 2020 2074 7279 3a0d             try:.
-00018e50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018e60: 2020 2020 2063 6f6e 6469 7469 6f6e 203d       condition =
-00018e70: 206c 6173 745f 7369 676e 616c 5b64 6174   last_signal[dat
-00018e80: 615f 6c69 7374 5b63 6e74 5d5d 5b30 5d5b  a_list[cnt]][0][
-00018e90: 2253 4c22 5d5b 305d 0d0a 2020 2020 2020  "SL"][0]..      
-00018ea0: 2020 2020 2020 2020 2020 6578 6365 7074            except
-00018eb0: 204b 6579 4572 726f 7220 6173 2065 3a20   KeyError as e: 
-00018ec0: 2320 7072 6167 6d61 3a20 6e6f 2063 6f76  # pragma: no cov
-00018ed0: 6572 0d0a 2020 2020 2020 2020 2020 2020  er..            
-00018ee0: 2020 2020 2020 2020 7365 6c66 2e64 6566          self.def
-00018ef0: 6175 6c74 5f6c 6f67 6765 722e 6465 6275  ault_logger.debu
-00018f00: 6728 652c 2065 7863 5f69 6e66 6f3d 5472  g(e, exc_info=Tr
-00018f10: 7565 290d 0a20 2020 2020 2020 2020 2020  ue)..           
-00018f20: 2020 2020 2020 2020 2063 6f6e 6469 7469           conditi
-00018f30: 6f6e 203d 206c 6173 745f 7369 676e 616c  on = last_signal
-00018f40: 5b64 6174 615f 6c69 7374 5b63 6e74 5d5d  [data_list[cnt]]
-00018f50: 5b22 534c 225d 5b30 5d0d 0a20 2020 2020  ["SL"][0]..     
-00018f60: 2020 2020 2020 2020 2020 2023 2069 6620             # if 
-00018f70: 6c61 7374 5f73 6967 6e61 6c5b 6461 7461  last_signal[data
-00018f80: 5f6c 6973 745b 636e 745d 5d20 6973 206e  _list[cnt]] is n
-00018f90: 6f74 2066 696e 616c 3a20 2020 2020 2020  ot final:       
-00018fa0: 2020 2023 2044 6562 7567 202d 2053 686f     # Debug - Sho
-00018fb0: 7773 2061 6c6c 2063 6f6e 6469 7469 6f6e  ws all condition
-00018fc0: 730d 0a20 2020 2020 2020 2020 2020 2020  s..             
-00018fd0: 2020 2069 6620 6c65 6e28 6669 6e61 6c5b     if len(final[
-00018fe0: 2253 4c22 5d29 203e 2030 2061 6e64 2063  "SL"]) > 0 and c
-00018ff0: 6f6e 6469 7469 6f6e 2021 3d20 6669 6e61  ondition != fina
-00019000: 6c5b 2253 4c22 5d2e 696c 6f63 5b30 5d3a  l["SL"].iloc[0]:
-00019010: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00019020: 2020 2020 2020 2320 446f 2073 6f6d 6574        # Do somet
-00019030: 6869 6e67 2077 6974 6820 7265 7375 6c74  hing with result
-00019040: 730d 0a20 2020 2020 2020 2020 2020 2020  s..             
-00019050: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
-00019060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019070: 2020 2020 2072 6573 756c 745f 6466 203d       result_df =
-00019080: 2070 642e 636f 6e63 6174 280d 0a20 2020   pd.concat(..   
-00019090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000190a0: 2020 2020 2020 2020 205b 0d0a 2020 2020           [..    
-000190b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000190c0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-000190d0: 6c74 5f64 662c 0d0a 2020 2020 2020 2020  lt_df,..        
+00018a30: 2020 2020 2028 642e 4c6f 772e 7368 6966       (d.Low.shif
+00018a40: 7428 3129 203e 2064 5b22 3545 4d41 225d  t(1) > d["5EMA"]
+00018a50: 2e73 6869 6674 2831 2929 0d0a 2020 2020  .shift(1))..    
+00018a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018a70: 2020 2020 2620 2864 2e4c 6f77 2e73 6869      & (d.Low.shi
+00018a80: 6674 2831 2920 2d20 645b 2235 454d 4122  ft(1) - d["5EMA"
+00018a90: 5d2e 7368 6966 7428 3129 203e 2030 2e35  ].shift(1) > 0.5
+00018aa0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00018ab0: 2020 2020 2020 205d 0d0a 2020 2020 2020         ]..      
+00018ac0: 2020 2020 2020 2020 2020 2020 2020 6f6c                ol
+00018ad0: 645f 696e 6465 7820 3d20 7661 6c69 6461  d_index = valida
+00018ae0: 7465 2e69 6e64 6578 0d0a 2020 2020 2020  te.index..      
+00018af0: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
+00018b00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018b10: 2020 2020 206d 6173 6b20 3d20 2864 2e48       mask = (d.H
+00018b20: 6967 6820 3c20 645b 2235 454d 4122 5d29  igh < d["5EMA"])
+00018b30: 2026 2028 645b 2235 454d 4122 5d20 2d20   & (d["5EMA"] - 
+00018b40: 642e 4869 6768 203e 2030 2e35 2920 2023  d.High > 0.5)  #
+00018b50: 2042 7579 0d0a 2020 2020 2020 2020 2020   Buy..          
+00018b60: 2020 2020 2020 2020 2020 7374 7265 6368            strech
+00018b70: 6564 203d 2064 5b6d 6173 6b5d 0d0a 2020  ed = d[mask]..  
+00018b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018b90: 2020 7374 7265 6368 6564 5b22 534c 225d    streched["SL"]
+00018ba0: 203d 2073 7472 6563 6865 642e 4c6f 770d   = streched.Low.
+00018bb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018bc0: 2020 2020 2076 616c 6964 6174 6520 3d20       validate = 
+00018bd0: 642e 6c6f 635b 6d61 736b 2e73 6869 6674  d.loc[mask.shift
+00018be0: 2831 292e 6669 6c6c 6e61 2846 616c 7365  (1).fillna(False
+00018bf0: 295d 0d0a 2020 2020 2020 2020 2020 2020  )]..            
+00018c00: 2020 2020 2020 2020 6f6c 645f 696e 6465          old_inde
+00018c10: 7820 3d20 7661 6c69 6461 7465 2e69 6e64  x = validate.ind
+00018c20: 6578 0d0a 2020 2020 2020 2020 2020 2020  ex..            
+00018c30: 7467 7420 3d20 7064 2e44 6174 6146 7261  tgt = pd.DataFra
+00018c40: 6d65 280d 0a20 2020 2020 2020 2020 2020  me(..           
+00018c50: 2020 2020 2028 0d0a 2020 2020 2020 2020       (..        
+00018c60: 2020 2020 2020 2020 2020 2020 7661 6c69              vali
+00018c70: 6461 7465 2e43 6c6f 7365 2e72 6573 6574  date.Close.reset
+00018c80: 5f69 6e64 6578 2864 726f 703d 5472 7565  _index(drop=True
+00018c90: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00018ca0: 2020 2020 2020 202d 2028 0d0a 2020 2020         - (..    
+00018cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018cc0: 2020 2020 280d 0a20 2020 2020 2020 2020      (..         
+00018cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018ce0: 2020 2073 7472 6563 6865 642e 534c 2e72     streched.SL.r
+00018cf0: 6573 6574 5f69 6e64 6578 2864 726f 703d  eset_index(drop=
+00018d00: 5472 7565 290d 0a20 2020 2020 2020 2020  True)..         
+00018d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018d20: 2020 202d 2076 616c 6964 6174 652e 436c     - validate.Cl
+00018d30: 6f73 652e 7265 7365 745f 696e 6465 7828  ose.reset_index(
+00018d40: 6472 6f70 3d54 7275 6529 0d0a 2020 2020  drop=True)..    
+00018d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018d60: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
+00018d70: 2020 2020 2020 2020 2020 2020 2020 202a                 *
+00018d80: 2072 6973 6b5f 7265 7761 7264 0d0a 2020   risk_reward..  
+00018d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018da0: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
+00018db0: 2020 2020 2029 2c0d 0a20 2020 2020 2020       ),..       
+00018dc0: 2020 2020 2020 2020 2063 6f6c 756d 6e73           columns
+00018dd0: 3d5b 2254 6172 6765 7422 5d2c 0d0a 2020  =["Target"],..  
+00018de0: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
+00018df0: 2020 2020 2020 2020 2076 616c 6964 6174           validat
+00018e00: 6520 3d20 7064 2e63 6f6e 6361 7428 0d0a  e = pd.concat(..
+00018e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018e20: 5b0d 0a20 2020 2020 2020 2020 2020 2020  [..             
+00018e30: 2020 2020 2020 2076 616c 6964 6174 652e         validate.
+00018e40: 7265 7365 745f 696e 6465 7828 6472 6f70  reset_index(drop
+00018e50: 3d54 7275 6529 2c0d 0a20 2020 2020 2020  =True),..       
+00018e60: 2020 2020 2020 2020 2020 2020 2073 7472               str
+00018e70: 6563 6865 645b 2253 4c22 5d2e 7265 7365  eched["SL"].rese
+00018e80: 745f 696e 6465 7828 6472 6f70 3d54 7275  t_index(drop=Tru
+00018e90: 6529 2c0d 0a20 2020 2020 2020 2020 2020  e),..           
+00018ea0: 2020 2020 2020 2020 2074 6774 2c0d 0a20           tgt,.. 
+00018eb0: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
+00018ec0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00018ed0: 2020 2061 7869 733d 312c 0d0a 2020 2020     axis=1,..    
+00018ee0: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
+00018ef0: 2020 2020 2020 2076 616c 6964 6174 6520         validate 
+00018f00: 3d20 7661 6c69 6461 7465 2e74 6169 6c28  = validate.tail(
+00018f10: 6c65 6e28 6f6c 645f 696e 6465 7829 290d  len(old_index)).
+00018f20: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
+00018f30: 6964 6174 6520 3d20 7661 6c69 6461 7465  idate = validate
+00018f40: 2e73 6574 5f69 6e64 6578 286f 6c64 5f69  .set_index(old_i
+00018f50: 6e64 6578 290d 0a20 2020 2020 2020 2020  ndex)..         
+00018f60: 2020 2069 6620 2273 656c 6c22 2069 6e20     if "sell" in 
+00018f70: 6461 7461 5f6c 6973 745b 636e 745d 3a0d  data_list[cnt]:.
+00018f80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018f90: 2066 696e 616c 203d 2076 616c 6964 6174   final = validat
+00018fa0: 655b 7661 6c69 6461 7465 2e43 6c6f 7365  e[validate.Close
+00018fb0: 203c 2076 616c 6964 6174 655b 2235 454d   < validate["5EM
+00018fc0: 4122 5d5d 2e74 6169 6c28 3129 0d0a 2020  A"]].tail(1)..  
+00018fd0: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
+00018fe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018ff0: 2066 696e 616c 203d 2076 616c 6964 6174   final = validat
+00019000: 655b 7661 6c69 6461 7465 2e43 6c6f 7365  e[validate.Close
+00019010: 203e 2076 616c 6964 6174 655b 2235 454d   > validate["5EM
+00019020: 4122 5d5d 2e74 6169 6c28 3129 0d0a 0d0a  A"]].tail(1)....
+00019030: 2020 2020 2020 2020 2020 2020 6966 2064              if d
+00019040: 6174 615f 6c69 7374 5b63 6e74 5d20 6e6f  ata_list[cnt] no
+00019050: 7420 696e 206c 6173 745f 7369 676e 616c  t in last_signal
+00019060: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00019070: 2020 206c 6173 745f 7369 676e 616c 5b64     last_signal[d
+00019080: 6174 615f 6c69 7374 5b63 6e74 5d5d 203d  ata_list[cnt]] =
+00019090: 2066 696e 616c 0d0a 2020 2020 2020 2020   final..        
+000190a0: 2020 2020 656c 6966 2064 6174 615f 6c69      elif data_li
+000190b0: 7374 5b63 6e74 5d20 696e 206c 6173 745f  st[cnt] in last_
+000190c0: 7369 676e 616c 3a0d 0a20 2020 2020 2020  signal:..       
+000190d0: 2020 2020 2020 2020 2074 7279 3a0d 0a20           try:.. 
 000190e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000190f0: 2020 2020 2020 2020 7064 2e44 6174 6146          pd.DataF
-00019100: 7261 6d65 280d 0a20 2020 2020 2020 2020  rame(..         
-00019110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019120: 2020 2020 2020 2020 2020 205b 0d0a 2020             [..  
-00019130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019150: 2020 2020 2020 5b0d 0a20 2020 2020 2020        [..       
-00019160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019180: 2020 2020 2063 6f6c 6f72 5465 7874 2e42       colorText.B
-00019190: 4c55 450d 0a20 2020 2020 2020 2020 2020  LUE..           
-000191a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000191b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000191c0: 202b 2073 7472 2866 696e 616c 2e69 6e64   + str(final.ind
-000191d0: 6578 5b30 5d29 0d0a 2020 2020 2020 2020  ex[0])..        
-000191e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000191f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019200: 2020 2020 2b20 636f 6c6f 7254 6578 742e      + colorText.
-00019210: 454e 442c 0d0a 2020 2020 2020 2020 2020  END,..          
-00019220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019240: 2020 636f 6c6f 7254 6578 742e 424f 4c44    colorText.BOLD
-00019250: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00019260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019270: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-00019280: 636f 6c6f 7254 6578 742e 5741 524e 0d0a  colorText.WARN..
-00019290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000190f0: 2020 2063 6f6e 6469 7469 6f6e 203d 206c     condition = l
+00019100: 6173 745f 7369 676e 616c 5b64 6174 615f  ast_signal[data_
+00019110: 6c69 7374 5b63 6e74 5d5d 5b30 5d5b 2253  list[cnt]][0]["S
+00019120: 4c22 5d5b 305d 0d0a 2020 2020 2020 2020  L"][0]..        
+00019130: 2020 2020 2020 2020 6578 6365 7074 204b          except K
+00019140: 6579 4572 726f 7220 6173 2065 3a20 2320  eyError as e: # 
+00019150: 7072 6167 6d61 3a20 6e6f 2063 6f76 6572  pragma: no cover
+00019160: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019170: 2020 2020 2020 7365 6c66 2e64 6566 6175        self.defau
+00019180: 6c74 5f6c 6f67 6765 722e 6465 6275 6728  lt_logger.debug(
+00019190: 652c 2065 7863 5f69 6e66 6f3d 5472 7565  e, exc_info=True
+000191a0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000191b0: 2020 2020 2020 2063 6f6e 6469 7469 6f6e         condition
+000191c0: 203d 206c 6173 745f 7369 676e 616c 5b64   = last_signal[d
+000191d0: 6174 615f 6c69 7374 5b63 6e74 5d5d 5b22  ata_list[cnt]]["
+000191e0: 534c 225d 5b30 5d0d 0a20 2020 2020 2020  SL"][0]..       
+000191f0: 2020 2020 2020 2020 2023 2069 6620 6c61           # if la
+00019200: 7374 5f73 6967 6e61 6c5b 6461 7461 5f6c  st_signal[data_l
+00019210: 6973 745b 636e 745d 5d20 6973 206e 6f74  ist[cnt]] is not
+00019220: 2066 696e 616c 3a20 2020 2020 2020 2020   final:         
+00019230: 2023 2044 6562 7567 202d 2053 686f 7773   # Debug - Shows
+00019240: 2061 6c6c 2063 6f6e 6469 7469 6f6e 730d   all conditions.
+00019250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019260: 2069 6620 6c65 6e28 6669 6e61 6c5b 2253   if len(final["S
+00019270: 4c22 5d29 203e 2030 2061 6e64 2063 6f6e  L"]) > 0 and con
+00019280: 6469 7469 6f6e 2021 3d20 6669 6e61 6c5b  dition != final[
+00019290: 2253 4c22 5d2e 696c 6f63 5b30 5d3a 0d0a  "SL"].iloc[0]:..
 000192a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000192b0: 2020 2020 2020 2020 2020 2020 2b20 6461              + da
-000192c0: 7461 5f6c 6973 745b 636e 745d 2e73 706c  ta_list[cnt].spl
-000192d0: 6974 2822 5f22 295b 305d 2e75 7070 6572  it("_")[0].upper
-000192e0: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
+000192b0: 2020 2020 2320 446f 2073 6f6d 6574 6869      # Do somethi
+000192c0: 6e67 2077 6974 6820 7265 7375 6c74 730d  ng with results.
+000192d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000192e0: 2020 2020 2074 7279 3a0d 0a20 2020 2020       try:..     
 000192f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019310: 2b20 636f 6c6f 7254 6578 742e 454e 442c  + colorText.END,
-00019320: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00019330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019340: 2020 2020 2020 2020 2020 2020 2020 280d                (.
-00019350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019300: 2020 2072 6573 756c 745f 6466 203d 2070     result_df = p
+00019310: 642e 636f 6e63 6174 280d 0a20 2020 2020  d.concat(..     
+00019320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019330: 2020 2020 2020 205b 0d0a 2020 2020 2020         [..      
+00019340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019350: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00019360: 5f64 662c 0d0a 2020 2020 2020 2020 2020  _df,..          
 00019370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019380: 2063 6f6c 6f72 5465 7874 2e42 4f4c 440d   colorText.BOLD.
-00019390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019380: 2020 2020 2020 7064 2e44 6174 6146 7261        pd.DataFra
+00019390: 6d65 280d 0a20 2020 2020 2020 2020 2020  me(..           
 000193a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000193b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000193c0: 202b 2063 6f6c 6f72 5465 7874 2e46 4149   + colorText.FAI
-000193d0: 4c0d 0a20 2020 2020 2020 2020 2020 2020  L..             
-000193e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000193b0: 2020 2020 2020 2020 205b 0d0a 2020 2020           [..    
+000193c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000193d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000193e0: 2020 2020 5b0d 0a20 2020 2020 2020 2020      [..         
 000193f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019400: 2020 202b 2064 6174 615f 6c69 7374 5b63     + data_list[c
-00019410: 6e74 5d2e 7370 6c69 7428 225f 2229 5b31  nt].split("_")[1
-00019420: 5d2e 7570 7065 7228 290d 0a20 2020 2020  ].upper()..     
+00019400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019410: 2020 2063 6f6c 6f72 5465 7874 2e42 4c55     colorText.BLU
+00019420: 450d 0a20 2020 2020 2020 2020 2020 2020  E..             
 00019430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019450: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
-00019460: 6f72 5465 7874 2e45 4e44 0d0a 2020 2020  orText.END..    
+00019440: 2020 2020 2020 2020 2020 2020 2020 202b                 +
+00019450: 2073 7472 2866 696e 616c 2e69 6e64 6578   str(final.index
+00019460: 5b30 5d29 0d0a 2020 2020 2020 2020 2020  [0])..          
 00019470: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00019480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019490: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
-000194a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019490: 2020 2b20 636f 6c6f 7254 6578 742e 454e    + colorText.EN
+000194a0: 442c 0d0a 2020 2020 2020 2020 2020 2020  D,..            
 000194b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000194c0: 2020 2020 2020 2069 6620 2273 656c 6c22         if "sell"
-000194d0: 2069 6e20 6461 7461 5f6c 6973 745b 636e   in data_list[cn
-000194e0: 745d 0d0a 2020 2020 2020 2020 2020 2020  t]..            
+000194c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000194d0: 636f 6c6f 7254 6578 742e 424f 4c44 0d0a  colorText.BOLD..
+000194e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000194f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019510: 656c 7365 2028 0d0a 2020 2020 2020 2020  else (..        
+00019500: 2020 2020 2020 2020 2020 2020 2b20 636f              + co
+00019510: 6c6f 7254 6578 742e 5741 524e 0d0a 2020  lorText.WARN..  
 00019520: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00019530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019540: 2020 2020 2020 2020 636f 6c6f 7254 6578          colorTex
-00019550: 742e 424f 4c44 0d0a 2020 2020 2020 2020  t.BOLD..        
-00019560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019580: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
-00019590: 6578 742e 4752 4545 4e0d 0a20 2020 2020  ext.GREEN..     
-000195a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019540: 2020 2020 2020 2020 2020 2b20 6461 7461            + data
+00019550: 5f6c 6973 745b 636e 745d 2e73 706c 6974  _list[cnt].split
+00019560: 2822 5f22 295b 305d 2e75 7070 6572 2829  ("_")[0].upper()
+00019570: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019590: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+000195a0: 636f 6c6f 7254 6578 742e 454e 442c 0d0a  colorText.END,..
 000195b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000195c0: 2020 2020 2020 2020 2020 202b 2064 6174             + dat
-000195d0: 615f 6c69 7374 5b63 6e74 5d2e 7370 6c69  a_list[cnt].spli
-000195e0: 7428 225f 2229 5b31 5d2e 7570 7065 7228  t("_")[1].upper(
-000195f0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00019600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019620: 2020 202b 2063 6f6c 6f72 5465 7874 2e45     + colorText.E
-00019630: 4e44 0d0a 2020 2020 2020 2020 2020 2020  ND..            
-00019640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019660: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+000195c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000195d0: 2020 2020 2020 2020 2020 2020 280d 0a20              (.. 
+000195e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000195f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019600: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00019610: 6f6c 6f72 5465 7874 2e42 4f4c 440d 0a20  olorText.BOLD.. 
+00019620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019640: 2020 2020 2020 2020 2020 2020 2020 202b                 +
+00019650: 2063 6f6c 6f72 5465 7874 2e46 4149 4c0d   colorText.FAIL.
+00019660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00019670: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00019680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019690: 636f 6c6f 7254 6578 742e 4641 494c 0d0a  colorText.FAIL..
-000196a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000196b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000196c0: 2020 2020 2020 2020 2020 2020 2b20 7374              + st
-000196d0: 7228 6669 6e61 6c2e 534c 5b30 5d29 0d0a  r(final.SL[0])..
-000196e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000196f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019700: 2020 2020 2020 2020 2020 2020 2b20 636f              + co
-00019710: 6c6f 7254 6578 742e 454e 442c 0d0a 2020  lorText.END,..  
-00019720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019690: 202b 2064 6174 615f 6c69 7374 5b63 6e74   + data_list[cnt
+000196a0: 5d2e 7370 6c69 7428 225f 2229 5b31 5d2e  ].split("_")[1].
+000196b0: 7570 7065 7228 290d 0a20 2020 2020 2020  upper()..       
+000196c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000196d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000196e0: 2020 2020 2020 2020 202b 2063 6f6c 6f72           + color
+000196f0: 5465 7874 2e45 4e44 0d0a 2020 2020 2020  Text.END..      
+00019700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019720: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
 00019730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019740: 2020 2020 2020 2020 2020 636f 6c6f 7254            colorT
-00019750: 6578 742e 4752 4545 4e0d 0a20 2020 2020  ext.GREEN..     
-00019760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019780: 2020 2020 2020 202b 2073 7472 2866 696e         + str(fin
-00019790: 616c 2e54 6172 6765 745b 305d 290d 0a20  al.Target[0]).. 
-000197a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019750: 2020 2020 2069 6620 2273 656c 6c22 2069       if "sell" i
+00019760: 6e20 6461 7461 5f6c 6973 745b 636e 745d  n data_list[cnt]
+00019770: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019790: 2020 2020 2020 2020 2020 2020 2020 656c                el
+000197a0: 7365 2028 0d0a 2020 2020 2020 2020 2020  se (..          
 000197b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000197c0: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
-000197d0: 6f72 5465 7874 2e45 4e44 2c0d 0a20 2020  orText.END,..   
-000197e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000197c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000197d0: 2020 2020 2020 636f 6c6f 7254 6578 742e        colorText.
+000197e0: 424f 4c44 0d0a 2020 2020 2020 2020 2020  BOLD..          
 000197f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019800: 2020 2020 2020 2020 2066 2231 3a7b 7269           f"1:{ri
-00019810: 736b 5f72 6577 6172 647d 222c 0d0a 2020  sk_reward}",..  
-00019820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019810: 2020 2020 2020 2b20 636f 6c6f 7254 6578        + colorTex
+00019820: 742e 4752 4545 4e0d 0a20 2020 2020 2020  t.GREEN..       
 00019830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019840: 2020 2020 2020 5d0d 0a20 2020 2020 2020        ]..       
-00019850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019860: 2020 2020 2020 2020 2020 2020 205d 2c0d               ],.
-00019870: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019890: 2020 2020 2063 6f6c 756d 6e73 3d72 6573       columns=res
-000198a0: 756c 745f 6466 2e63 6f6c 756d 6e73 2c0d  ult_df.columns,.
-000198b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000198c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000198d0: 2029 2c0d 0a20 2020 2020 2020 2020 2020   ),..           
-000198e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000198f0: 205d 2c0d 0a20 2020 2020 2020 2020 2020   ],..           
+00019840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019850: 2020 2020 2020 2020 202b 2064 6174 615f           + data_
+00019860: 6c69 7374 5b63 6e74 5d2e 7370 6c69 7428  list[cnt].split(
+00019870: 225f 2229 5b31 5d2e 7570 7065 7228 290d  "_")[1].upper().
+00019880: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000198a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000198b0: 202b 2063 6f6c 6f72 5465 7874 2e45 4e44   + colorText.END
+000198c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000198d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000198e0: 2020 2020 2020 2020 2020 2020 2020 292c                ),
+000198f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00019900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019910: 2061 7869 733d 302c 0d0a 2020 2020 2020   axis=0,..      
-00019920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019930: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
-00019940: 2020 2020 2020 2020 2020 2020 2072 6573               res
-00019950: 756c 745f 6466 2e72 6573 6574 5f69 6e64  ult_df.reset_ind
-00019960: 6578 2864 726f 703d 5472 7565 2c20 696e  ex(drop=True, in
-00019970: 706c 6163 653d 5472 7565 290d 0a20 2020  place=True)..   
+00019910: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00019920: 6c6f 7254 6578 742e 4641 494c 0d0a 2020  lorText.FAIL..  
+00019930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019950: 2020 2020 2020 2020 2020 2b20 7374 7228            + str(
+00019960: 6669 6e61 6c2e 534c 5b30 5d29 0d0a 2020  final.SL[0])..  
+00019970: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00019980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019990: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
-000199a0: 6e20 6173 2065 3a20 2023 2070 7261 676d  n as e:  # pragm
-000199b0: 613a 206e 6f20 636f 7665 720d 0a20 2020  a: no cover..   
+00019990: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
+000199a0: 7254 6578 742e 454e 442c 0d0a 2020 2020  rText.END,..    
+000199b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000199c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000199d0: 2020 2020 2073 656c 662e 6465 6661 756c       self.defaul
-000199e0: 745f 6c6f 6767 6572 2e64 6562 7567 2865  t_logger.debug(e
-000199f0: 2c20 6578 635f 696e 666f 3d54 7275 6529  , exc_info=True)
-00019a00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00019a10: 2020 2020 2020 2020 2020 7061 7373 0d0a            pass..
-00019a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019a30: 2020 2020 2320 5468 656e 2075 7064 6174      # Then updat
-00019a40: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
-00019a50: 2020 2020 2020 206c 6173 745f 7369 676e         last_sign
-00019a60: 616c 5b64 6174 615f 6c69 7374 5b63 6e74  al[data_list[cnt
-00019a70: 5d5d 203d 205b 6669 6e61 6c5d 0d0a 2020  ]] = [final]..  
-00019a80: 2020 2020 2020 6966 2072 6573 756c 745f        if result_
-00019a90: 6466 2069 7320 6e6f 7420 4e6f 6e65 3a0d  df is not None:.
-00019aa0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00019ab0: 756c 745f 6466 2e64 726f 705f 6475 706c  ult_df.drop_dupl
-00019ac0: 6963 6174 6573 286b 6565 703d 226c 6173  icates(keep="las
-00019ad0: 7422 2c20 696e 706c 6163 653d 5472 7565  t", inplace=True
-00019ae0: 290d 0a20 2020 2020 2020 2020 2020 2072  )..            r
-00019af0: 6573 756c 745f 6466 2e73 6f72 745f 7661  esult_df.sort_va
-00019b00: 6c75 6573 2862 793d 2254 696d 6522 2c20  lues(by="Time", 
-00019b10: 696e 706c 6163 653d 5472 7565 290d 0a20  inplace=True).. 
-00019b20: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-00019b30: 7375 6c74 5f64 665b 3a3a 2d31 5d0d 0a0d  sult_df[::-1]...
-00019b40: 0a20 2020 2023 2050 7265 7072 6f63 6573  .    # Preproces
-00019b50: 7320 7468 6520 6163 7175 6972 6564 2064  s the acquired d
-00019b60: 6174 610d 0a20 2020 2064 6566 2070 7265  ata..    def pre
-00019b70: 7072 6f63 6573 7344 6174 6128 7365 6c66  processData(self
-00019b80: 2c20 6466 2c20 6461 7973 546f 4c6f 6f6b  , df, daysToLook
-00019b90: 6261 636b 3d4e 6f6e 6529 3a0d 0a20 2020  back=None):..   
-00019ba0: 2020 2020 2061 7373 6572 7420 6973 696e       assert isin
-00019bb0: 7374 616e 6365 2864 662c 2070 642e 4461  stance(df, pd.Da
-00019bc0: 7461 4672 616d 6529 0d0a 2020 2020 2020  taFrame)..      
-00019bd0: 2020 6461 7461 203d 2064 662e 636f 7079    data = df.copy
-00019be0: 2829 0d0a 2020 2020 2020 2020 7472 793a  ()..        try:
-00019bf0: 0d0a 2020 2020 2020 2020 2020 2020 6461  ..            da
-00019c00: 7461 203d 2064 6174 612e 7265 706c 6163  ta = data.replac
-00019c10: 6528 6e70 2e69 6e66 2c20 6e70 2e6e 616e  e(np.inf, np.nan
-00019c20: 292e 7265 706c 6163 6528 2d6e 702e 696e  ).replace(-np.in
-00019c30: 662c 206e 702e 6e61 6e29 2e64 726f 706e  f, np.nan).dropn
-00019c40: 6128 686f 773d 2261 6c6c 2229 0d0a 2020  a(how="all")..  
-00019c50: 2020 2020 2020 2020 2020 2320 7365 6c66            # self
-00019c60: 2e64 6566 6175 6c74 5f6c 6f67 6765 722e  .default_logger.
-00019c70: 696e 666f 2866 2250 7265 7072 6f63 6573  info(f"Preproces
-00019c80: 7369 6e67 2064 6174 613a 5c6e 7b64 6174  sing data:\n{dat
-00019c90: 612e 6865 6164 2831 297d 5c6e 2229 0d0a  a.head(1)}\n")..
-00019ca0: 2020 2020 2020 2020 2020 2020 6966 2064              if d
-00019cb0: 6179 7354 6f4c 6f6f 6b62 6163 6b20 6973  aysToLookback is
-00019cc0: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-00019cd0: 2020 2020 2020 2020 6461 7973 546f 4c6f          daysToLo
-00019ce0: 6f6b 6261 636b 203d 2073 656c 662e 636f  okback = self.co
-00019cf0: 6e66 6967 4d61 6e61 6765 722e 6461 7973  nfigManager.days
-00019d00: 546f 4c6f 6f6b 6261 636b 0d0a 2020 2020  ToLookback..    
-00019d10: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00019d20: 636f 6e66 6967 4d61 6e61 6765 722e 7573  configManager.us
-00019d30: 6545 4d41 3a0d 0a20 2020 2020 2020 2020  eEMA:..         
-00019d40: 2020 2020 2020 2073 6d61 203d 2070 6b74         sma = pkt
-00019d50: 616c 6962 2e45 4d41 2864 6174 615b 2243  alib.EMA(data["C
-00019d60: 6c6f 7365 225d 2c20 7469 6d65 7065 7269  lose"], timeperi
-00019d70: 6f64 3d35 3029 0d0a 2020 2020 2020 2020  od=50)..        
-00019d80: 2020 2020 2020 2020 6c6d 6120 3d20 706b          lma = pk
-00019d90: 7461 6c69 622e 454d 4128 6461 7461 5b22  talib.EMA(data["
-00019da0: 436c 6f73 6522 5d2c 2074 696d 6570 6572  Close"], timeper
-00019db0: 696f 643d 3230 3029 0d0a 2020 2020 2020  iod=200)..      
-00019dc0: 2020 2020 2020 2020 2020 7373 6d61 203d            ssma =
-00019dd0: 2070 6b74 616c 6962 2e45 4d41 2864 6174   pktalib.EMA(dat
-00019de0: 615b 2243 6c6f 7365 225d 2c20 7469 6d65  a["Close"], time
-00019df0: 7065 7269 6f64 3d39 290d 0a20 2020 2020  period=9)..     
-00019e00: 2020 2020 2020 2020 2020 2064 6174 612e             data.
-00019e10: 696e 7365 7274 286c 656e 2864 6174 612e  insert(len(data.
-00019e20: 636f 6c75 6d6e 7329 2c20 2253 4d41 222c  columns), "SMA",
-00019e30: 2073 6d61 290d 0a20 2020 2020 2020 2020   sma)..         
-00019e40: 2020 2020 2020 2064 6174 612e 696e 7365         data.inse
-00019e50: 7274 286c 656e 2864 6174 612e 636f 6c75  rt(len(data.colu
-00019e60: 6d6e 7329 2c20 224c 4d41 222c 206c 6d61  mns), "LMA", lma
-00019e70: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00019e80: 2020 2064 6174 612e 696e 7365 7274 286c     data.insert(l
-00019e90: 656e 2864 6174 612e 636f 6c75 6d6e 7329  en(data.columns)
-00019ea0: 2c20 2253 534d 4122 2c20 7373 6d61 290d  , "SSMA", ssma).
-00019eb0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-00019ec0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00019ed0: 2020 2020 736d 6120 3d20 706b 7461 6c69      sma = pktali
-00019ee0: 622e 534d 4128 6461 7461 5b22 436c 6f73  b.SMA(data["Clos
-00019ef0: 6522 5d2c 2074 696d 6570 6572 696f 643d  e"], timeperiod=
-00019f00: 3530 290d 0a20 2020 2020 2020 2020 2020  50)..           
-00019f10: 2020 2020 206c 6d61 203d 2070 6b74 616c       lma = pktal
-00019f20: 6962 2e53 4d41 2864 6174 615b 2243 6c6f  ib.SMA(data["Clo
-00019f30: 7365 225d 2c20 7469 6d65 7065 7269 6f64  se"], timeperiod
-00019f40: 3d32 3030 290d 0a20 2020 2020 2020 2020  =200)..         
-00019f50: 2020 2020 2020 2073 736d 6120 3d20 706b         ssma = pk
-00019f60: 7461 6c69 622e 534d 4128 6461 7461 5b22  talib.SMA(data["
-00019f70: 436c 6f73 6522 5d2c 2074 696d 6570 6572  Close"], timeper
-00019f80: 696f 643d 3929 0d0a 2020 2020 2020 2020  iod=9)..        
-00019f90: 2020 2020 2020 2020 6461 7461 2e69 6e73          data.ins
-00019fa0: 6572 7428 6c65 6e28 6461 7461 2e63 6f6c  ert(len(data.col
-00019fb0: 756d 6e73 292c 2022 534d 4122 2c20 736d  umns), "SMA", sm
-00019fc0: 6129 0d0a 2020 2020 2020 2020 2020 2020  a)..            
-00019fd0: 2020 2020 6461 7461 2e69 6e73 6572 7428      data.insert(
-00019fe0: 6c65 6e28 6461 7461 2e63 6f6c 756d 6e73  len(data.columns
-00019ff0: 292c 2022 4c4d 4122 2c20 6c6d 6129 0d0a  ), "LMA", lma)..
-0001a000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a010: 6461 7461 2e69 6e73 6572 7428 6c65 6e28  data.insert(len(
-0001a020: 6461 7461 2e63 6f6c 756d 6e73 292c 2022  data.columns), "
-0001a030: 5353 4d41 222c 2073 736d 6129 0d0a 2020  SSMA", ssma)..  
-0001a040: 2020 2020 2020 2020 2020 766f 6c20 3d20            vol = 
-0001a050: 706b 7461 6c69 622e 534d 4128 6461 7461  pktalib.SMA(data
-0001a060: 5b22 566f 6c75 6d65 225d 2c20 7469 6d65  ["Volume"], time
-0001a070: 7065 7269 6f64 3d32 3029 0d0a 2020 2020  period=20)..    
-0001a080: 2020 2020 2020 2020 7273 6920 3d20 706b          rsi = pk
-0001a090: 7461 6c69 622e 5253 4928 6461 7461 5b22  talib.RSI(data["
-0001a0a0: 436c 6f73 6522 5d2c 2074 696d 6570 6572  Close"], timeper
-0001a0b0: 696f 643d 3134 290d 0a20 2020 2020 2020  iod=14)..       
-0001a0c0: 2020 2020 2064 6174 612e 696e 7365 7274       data.insert
-0001a0d0: 286c 656e 2864 6174 612e 636f 6c75 6d6e  (len(data.column
-0001a0e0: 7329 2c20 2256 6f6c 4d41 222c 2076 6f6c  s), "VolMA", vol
-0001a0f0: 290d 0a20 2020 2020 2020 2020 2020 2064  )..            d
-0001a100: 6174 612e 696e 7365 7274 286c 656e 2864  ata.insert(len(d
-0001a110: 6174 612e 636f 6c75 6d6e 7329 2c20 2252  ata.columns), "R
-0001a120: 5349 222c 2072 7369 290d 0a20 2020 2020  SI", rsi)..     
-0001a130: 2020 2020 2020 2063 6369 203d 2070 6b74         cci = pkt
-0001a140: 616c 6962 2e43 4349 2864 6174 615b 2248  alib.CCI(data["H
-0001a150: 6967 6822 5d2c 2064 6174 615b 224c 6f77  igh"], data["Low
-0001a160: 225d 2c20 6461 7461 5b22 436c 6f73 6522  "], data["Close"
-0001a170: 5d2c 2074 696d 6570 6572 696f 643d 3134  ], timeperiod=14
-0001a180: 290d 0a20 2020 2020 2020 2020 2020 2064  )..            d
-0001a190: 6174 612e 696e 7365 7274 286c 656e 2864  ata.insert(len(d
-0001a1a0: 6174 612e 636f 6c75 6d6e 7329 2c20 2243  ata.columns), "C
-0001a1b0: 4349 222c 2063 6369 290d 0a20 2020 2020  CI", cci)..     
-0001a1c0: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
-0001a1d0: 2020 2020 2020 2020 2020 2020 2066 6173               fas
-0001a1e0: 746b 2c20 6661 7374 6420 3d20 706b 7461  tk, fastd = pkta
-0001a1f0: 6c69 622e 5354 4f43 4852 5349 280d 0a20  lib.STOCHRSI(.. 
-0001a200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a210: 2020 2064 6174 615b 2243 6c6f 7365 225d     data["Close"]
-0001a220: 2c20 7469 6d65 7065 7269 6f64 3d31 342c  , timeperiod=14,
-0001a230: 2066 6173 746b 5f70 6572 696f 643d 352c   fastk_period=5,
-0001a240: 2066 6173 7464 5f70 6572 696f 643d 332c   fastd_period=3,
-0001a250: 2066 6173 7464 5f6d 6174 7970 653d 300d   fastd_matype=0.
-0001a260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a270: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
-0001a280: 2020 2020 6461 7461 2e69 6e73 6572 7428      data.insert(
-0001a290: 6c65 6e28 6461 7461 2e63 6f6c 756d 6e73  len(data.columns
-0001a2a0: 292c 2022 4641 5354 4b22 2c20 6661 7374  ), "FASTK", fast
-0001a2b0: 6b29 0d0a 2020 2020 2020 2020 2020 2020  k)..            
-0001a2c0: 2020 2020 6461 7461 2e69 6e73 6572 7428      data.insert(
-0001a2d0: 6c65 6e28 6461 7461 2e63 6f6c 756d 6e73  len(data.columns
-0001a2e0: 292c 2022 4641 5354 4422 2c20 6661 7374  ), "FASTD", fast
-0001a2f0: 6429 0d0a 2020 2020 2020 2020 2020 2020  d)..            
-0001a300: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
-0001a310: 2061 7320 653a 0d0a 2020 2020 2020 2020   as e:..        
-0001a320: 2020 2020 2020 2020 7365 6c66 2e64 6566          self.def
-0001a330: 6175 6c74 5f6c 6f67 6765 722e 6465 6275  ault_logger.debu
-0001a340: 6728 652c 2065 7863 5f69 6e66 6f3d 5472  g(e, exc_info=Tr
-0001a350: 7565 290d 0a20 2020 2020 2020 2020 2020  ue)..           
-0001a360: 2020 2020 2070 6173 730d 0a20 2020 2020       pass..     
-0001a370: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
-0001a380: 696f 6e20 6173 2065 3a0d 0a20 2020 2020  ion as e:..     
-0001a390: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001a3a0: 6465 6661 756c 745f 6c6f 6767 6572 2e64  default_logger.d
-0001a3b0: 6562 7567 2865 2c20 6578 635f 696e 666f  ebug(e, exc_info
-0001a3c0: 3d54 7275 6529 0d0a 2020 2020 2020 2020  =True)..        
-0001a3d0: 2020 2020 2020 2020 7061 7373 0d0a 2020          pass..  
-0001a3e0: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
-0001a3f0: 615b 3a3a 2d31 5d20 2023 2052 6576 6572  a[::-1]  # Rever
-0001a400: 7365 2074 6865 2064 6174 6166 7261 6d65  se the dataframe
-0001a410: 0d0a 2020 2020 2020 2020 2320 6461 7461  ..        # data
-0001a420: 203d 2064 6174 612e 6669 6c6c 6e61 2830   = data.fillna(0
-0001a430: 290d 0a20 2020 2020 2020 2023 2064 6174  )..        # dat
-0001a440: 6120 3d20 6461 7461 2e72 6570 6c61 6365  a = data.replace
-0001a450: 285b 6e70 2e69 6e66 2c20 2d6e 702e 696e  ([np.inf, -np.in
-0001a460: 665d 2c20 3029 0d0a 2020 2020 2020 2020  f], 0)..        
-0001a470: 6675 6c6c 4461 7461 203d 2064 6174 610d  fullData = data.
-0001a480: 0a20 2020 2020 2020 2074 7269 6d6d 6564  .        trimmed
-0001a490: 4461 7461 203d 2064 6174 612e 6865 6164  Data = data.head
-0001a4a0: 2864 6179 7354 6f4c 6f6f 6b62 6163 6b29  (daysToLookback)
-0001a4b0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-0001a4c0: 2028 6675 6c6c 4461 7461 2c20 7472 696d   (fullData, trim
-0001a4d0: 6d65 6444 6174 6129 0d0a 0d0a 2020 2020  medData)....    
-0001a4e0: 2320 5661 6c69 6461 7465 2069 6620 7468  # Validate if th
-0001a4f0: 6520 7374 6f63 6b20 6973 2062 756c 6c69  e stock is bulli
-0001a500: 7368 2069 6e20 7468 6520 7368 6f72 7420  sh in the short 
-0001a510: 7465 726d 0d0a 2020 2020 6465 6620 7661  term..    def va
-0001a520: 6c69 6461 7465 3135 4d69 6e75 7465 5072  lidate15MinutePr
-0001a530: 6963 6556 6f6c 756d 6542 7265 616b 6f75  iceVolumeBreakou
-0001a540: 7428 7365 6c66 2c20 6466 293a 0d0a 2020  t(self, df):..  
-0001a550: 2020 2020 2020 6966 2064 6620 6973 204e        if df is N
-0001a560: 6f6e 6520 6f72 206c 656e 2864 6629 203d  one or len(df) =
-0001a570: 3d20 303a 0d0a 2020 2020 2020 2020 2020  = 0:..          
-0001a580: 2020 7265 7475 726e 2046 616c 7365 0d0a    return False..
-0001a590: 2020 2020 2020 2020 2320 6874 7470 733a          # https:
-0001a5a0: 2f2f 6368 6172 7469 6e6b 2e63 6f6d 2f73  //chartink.com/s
-0001a5b0: 6372 6565 6e65 722f 3135 2d6d 696e 2d70  creener/15-min-p
-0001a5c0: 7269 6365 2d76 6f6c 756d 652d 6272 6561  rice-volume-brea
-0001a5d0: 6b6f 7574 0d0a 2020 2020 2020 2020 6461  kout..        da
-0001a5e0: 7461 203d 2064 662e 636f 7079 2829 0d0a  ta = df.copy()..
-0001a5f0: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
-0001a600: 6174 612e 6669 6c6c 6e61 2830 290d 0a20  ata.fillna(0).. 
-0001a610: 2020 2020 2020 2064 6174 6120 3d20 6461         data = da
-0001a620: 7461 2e72 6570 6c61 6365 285b 6e70 2e69  ta.replace([np.i
-0001a630: 6e66 2c20 2d6e 702e 696e 665d 2c20 3029  nf, -np.inf], 0)
-0001a640: 0d0a 2020 2020 2020 2020 6461 7461 203d  ..        data =
-0001a650: 2064 6174 615b 3a3a 2d31 5d20 2023 2052   data[::-1]  # R
-0001a660: 6576 6572 7365 2074 6865 2064 6174 6166  everse the dataf
-0001a670: 7261 6d65 2073 6f20 7468 6174 2069 7473  rame so that its
-0001a680: 2074 6865 206f 6c64 6573 7420 6461 7465   the oldest date
-0001a690: 2066 6972 7374 0d0a 2020 2020 2020 2020   first..        
-0001a6a0: 6461 7461 5b22 534d 4132 3022 5d20 3d20  data["SMA20"] = 
-0001a6b0: 706b 7461 6c69 622e 534d 4128 6461 7461  pktalib.SMA(data
-0001a6c0: 5b22 436c 6f73 6522 5d2c 2032 3029 0d0a  ["Close"], 20)..
-0001a6d0: 2020 2020 2020 2020 6461 7461 5b22 534d          data["SM
-0001a6e0: 4132 3056 225d 203d 2070 6b74 616c 6962  A20V"] = pktalib
-0001a6f0: 2e53 4d41 2864 6174 615b 2256 6f6c 756d  .SMA(data["Volum
-0001a700: 6522 5d2c 2032 3029 0d0a 2020 2020 2020  e"], 20)..      
-0001a710: 2020 6461 7461 203d 2064 6174 615b 0d0a    data = data[..
-0001a720: 2020 2020 2020 2020 2020 2020 3a3a 2d31              ::-1
-0001a730: 0d0a 2020 2020 2020 2020 5d20 2023 2052  ..        ]  # R
-0001a740: 6576 6572 7365 2074 6865 2064 6174 6166  everse the dataf
-0001a750: 7261 6d65 2073 6f20 7468 6174 2069 7427  rame so that it'
-0001a760: 7320 7468 6520 6d6f 7374 2072 6563 656e  s the most recen
-0001a770: 7420 6461 7465 2066 6972 7374 0d0a 2020  t date first..  
-0001a780: 2020 2020 2020 7265 6365 6e74 203d 2064        recent = d
-0001a790: 6174 612e 6865 6164 2833 290d 0a20 2020  ata.head(3)..   
-0001a7a0: 2020 2020 2069 6620 6c65 6e28 7265 6365       if len(rece
-0001a7b0: 6e74 2920 3c20 333a 0d0a 2020 2020 2020  nt) < 3:..      
-0001a7c0: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-0001a7d0: 7365 0d0a 2020 2020 2020 2020 636f 6e64  se..        cond
-0001a7e0: 3120 3d20 7265 6365 6e74 5b22 436c 6f73  1 = recent["Clos
-0001a7f0: 6522 5d2e 696c 6f63 5b30 5d20 3e20 7265  e"].iloc[0] > re
-0001a800: 6365 6e74 5b22 436c 6f73 6522 5d2e 696c  cent["Close"].il
-0001a810: 6f63 5b31 5d0d 0a20 2020 2020 2020 2063  oc[1]..        c
-0001a820: 6f6e 6432 203d 2063 6f6e 6431 2061 6e64  ond2 = cond1 and
-0001a830: 2028 7265 6365 6e74 5b22 436c 6f73 6522   (recent["Close"
-0001a840: 5d2e 696c 6f63 5b30 5d20 3e20 7265 6365  ].iloc[0] > rece
-0001a850: 6e74 5b22 534d 4132 3022 5d2e 696c 6f63  nt["SMA20"].iloc
-0001a860: 5b30 5d29 0d0a 2020 2020 2020 2020 636f  [0])..        co
-0001a870: 6e64 3320 3d20 636f 6e64 3220 616e 6420  nd3 = cond2 and 
-0001a880: 2872 6563 656e 745b 2243 6c6f 7365 225d  (recent["Close"]
-0001a890: 2e69 6c6f 635b 315d 203e 2072 6563 656e  .iloc[1] > recen
-0001a8a0: 745b 2248 6967 6822 5d2e 696c 6f63 5b32  t["High"].iloc[2
-0001a8b0: 5d29 0d0a 2020 2020 2020 2020 636f 6e64  ])..        cond
-0001a8c0: 3420 3d20 636f 6e64 3320 616e 6420 2872  4 = cond3 and (r
-0001a8d0: 6563 656e 745b 2256 6f6c 756d 6522 5d2e  ecent["Volume"].
-0001a8e0: 696c 6f63 5b30 5d20 3e20 7265 6365 6e74  iloc[0] > recent
-0001a8f0: 5b22 534d 4132 3056 225d 2e69 6c6f 635b  ["SMA20V"].iloc[
-0001a900: 305d 290d 0a20 2020 2020 2020 2063 6f6e  0])..        con
-0001a910: 6435 203d 2063 6f6e 6434 2061 6e64 2028  d5 = cond4 and (
-0001a920: 7265 6365 6e74 5b22 566f 6c75 6d65 225d  recent["Volume"]
-0001a930: 2e69 6c6f 635b 315d 203e 2072 6563 656e  .iloc[1] > recen
-0001a940: 745b 2253 4d41 3230 5622 5d2e 696c 6f63  t["SMA20V"].iloc
-0001a950: 5b30 5d29 0d0a 2020 2020 2020 2020 7265  [0])..        re
-0001a960: 7475 726e 2063 6f6e 6435 0d0a 0d0a 2020  turn cond5....  
-0001a970: 2020 6465 6620 7661 6c69 6461 7465 4275    def validateBu
-0001a980: 6c6c 6973 6846 6f72 546f 6d6f 7272 6f77  llishForTomorrow
-0001a990: 2873 656c 662c 2064 6629 3a0d 0a20 2020  (self, df):..   
-0001a9a0: 2020 2020 2069 6620 6466 2069 7320 4e6f       if df is No
-0001a9b0: 6e65 206f 7220 6c65 6e28 6466 2920 3d3d  ne or len(df) ==
-0001a9c0: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
-0001a9d0: 2072 6574 7572 6e20 4661 6c73 650d 0a20   return False.. 
-0001a9e0: 2020 2020 2020 2064 6174 6120 3d20 6466         data = df
-0001a9f0: 2e63 6f70 7928 290d 0a20 2020 2020 2020  .copy()..       
-0001aa00: 2023 2068 7474 7073 3a2f 2f63 6861 7274   # https://chart
-0001aa10: 696e 6b2e 636f 6d2f 7363 7265 656e 6572  ink.com/screener
-0001aa20: 2f62 756c 6c69 7368 2d66 6f72 2d74 6f6d  /bullish-for-tom
-0001aa30: 6f72 726f 770d 0a20 2020 2020 2020 2064  orrow..        d
-0001aa40: 6174 6120 3d20 6461 7461 2e66 696c 6c6e  ata = data.filln
-0001aa50: 6128 3029 0d0a 2020 2020 2020 2020 6461  a(0)..        da
-0001aa60: 7461 203d 2064 6174 612e 7265 706c 6163  ta = data.replac
-0001aa70: 6528 5b6e 702e 696e 662c 202d 6e70 2e69  e([np.inf, -np.i
-0001aa80: 6e66 5d2c 2030 290d 0a20 2020 2020 2020  nf], 0)..       
-0001aa90: 2064 6174 6120 3d20 6461 7461 5b3a 3a2d   data = data[::-
-0001aaa0: 315d 2020 2320 5265 7665 7273 6520 7468  1]  # Reverse th
-0001aab0: 6520 6461 7461 6672 616d 6520 736f 2074  e dataframe so t
-0001aac0: 6861 7420 6974 7320 7468 6520 6f6c 6465  hat its the olde
-0001aad0: 7374 2064 6174 6520 6669 7273 740d 0a20  st date first.. 
-0001aae0: 2020 2020 2020 206d 6163 644c 696e 6520         macdLine 
-0001aaf0: 3d20 706b 7461 6c69 622e 4d41 4344 2864  = pktalib.MACD(d
-0001ab00: 6174 615b 2243 6c6f 7365 225d 2c20 3132  ata["Close"], 12
-0001ab10: 2c20 3236 2c20 3929 5b30 5d2e 7461 696c  , 26, 9)[0].tail
-0001ab20: 2833 290d 0a20 2020 2020 2020 206d 6163  (3)..        mac
-0001ab30: 6453 6967 6e61 6c20 3d20 706b 7461 6c69  dSignal = pktali
-0001ab40: 622e 4d41 4344 2864 6174 615b 2243 6c6f  b.MACD(data["Clo
-0001ab50: 7365 225d 2c20 3132 2c20 3236 2c20 3929  se"], 12, 26, 9)
-0001ab60: 5b31 5d2e 7461 696c 2833 290d 0a20 2020  [1].tail(3)..   
-0001ab70: 2020 2020 206d 6163 6448 6973 7420 3d20       macdHist = 
-0001ab80: 706b 7461 6c69 622e 4d41 4344 2864 6174  pktalib.MACD(dat
-0001ab90: 615b 2243 6c6f 7365 225d 2c20 3132 2c20  a["Close"], 12, 
-0001aba0: 3236 2c20 3929 5b32 5d2e 7461 696c 2833  26, 9)[2].tail(3
-0001abb0: 290d 0a0d 0a20 2020 2020 2020 2072 6574  )....        ret
-0001abc0: 7572 6e20 280d 0a20 2020 2020 2020 2020  urn (..         
-0001abd0: 2020 2028 6d61 6364 4869 7374 2e69 6c6f     (macdHist.ilo
-0001abe0: 635b 3a31 5d2e 696c 6f63 5b30 5d20 3c20  c[:1].iloc[0] < 
-0001abf0: 6d61 6364 4869 7374 2e69 6c6f 635b 3a32  macdHist.iloc[:2
-0001ac00: 5d2e 696c 6f63 5b31 5d29 0d0a 2020 2020  ].iloc[1])..    
-0001ac10: 2020 2020 2020 2020 616e 6420 286d 6163          and (mac
-0001ac20: 6448 6973 742e 696c 6f63 5b3a 335d 2e69  dHist.iloc[:3].i
-0001ac30: 6c6f 635b 325d 203e 206d 6163 6448 6973  loc[2] > macdHis
-0001ac40: 742e 696c 6f63 5b3a 325d 2e69 6c6f 635b  t.iloc[:2].iloc[
-0001ac50: 315d 290d 0a20 2020 2020 2020 2020 2020  1])..           
-0001ac60: 2061 6e64 2028 0d0a 2020 2020 2020 2020   and (..        
-0001ac70: 2020 2020 2020 2020 286d 6163 644c 696e          (macdLin
-0001ac80: 652e 696c 6f63 5b3a 335d 2e69 6c6f 635b  e.iloc[:3].iloc[
-0001ac90: 325d 202d 206d 6163 6453 6967 6e61 6c2e  2] - macdSignal.
-0001aca0: 696c 6f63 5b3a 335d 2e69 6c6f 635b 325d  iloc[:3].iloc[2]
-0001acb0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0001acc0: 2020 202d 2028 6d61 6364 4c69 6e65 2e69     - (macdLine.i
-0001acd0: 6c6f 635b 3a32 5d2e 696c 6f63 5b31 5d20  loc[:2].iloc[1] 
-0001ace0: 2d20 6d61 6364 5369 676e 616c 2e69 6c6f  - macdSignal.ilo
-0001acf0: 635b 3a32 5d2e 696c 6f63 5b31 5d29 0d0a  c[:2].iloc[1])..
-0001ad00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ad10: 3e3d 2030 2e34 0d0a 2020 2020 2020 2020  >= 0.4..        
-0001ad20: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
-0001ad30: 2020 2061 6e64 2028 0d0a 2020 2020 2020     and (..      
-0001ad40: 2020 2020 2020 2020 2020 286d 6163 644c            (macdL
-0001ad50: 696e 652e 696c 6f63 5b3a 325d 2e69 6c6f  ine.iloc[:2].ilo
-0001ad60: 635b 315d 202d 206d 6163 6453 6967 6e61  c[1] - macdSigna
-0001ad70: 6c2e 696c 6f63 5b3a 325d 2e69 6c6f 635b  l.iloc[:2].iloc[
-0001ad80: 315d 290d 0a20 2020 2020 2020 2020 2020  1])..           
-0001ad90: 2020 2020 202d 2028 6d61 6364 4c69 6e65       - (macdLine
-0001ada0: 2e69 6c6f 635b 3a31 5d2e 696c 6f63 5b30  .iloc[:1].iloc[0
-0001adb0: 5d20 2d20 6d61 6364 5369 676e 616c 2e69  ] - macdSignal.i
-0001adc0: 6c6f 635b 3a31 5d2e 696c 6f63 5b30 5d29  loc[:1].iloc[0])
-0001add0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001ade0: 2020 3c3d 2030 2e32 0d0a 2020 2020 2020    <= 0.2..      
-0001adf0: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-0001ae00: 2020 2020 2061 6e64 2028 6d61 6364 4c69       and (macdLi
-0001ae10: 6e65 2e69 6c6f 635b 3a33 5d2e 696c 6f63  ne.iloc[:3].iloc
-0001ae20: 5b32 5d20 3e20 6d61 6364 5369 676e 616c  [2] > macdSignal
-0001ae30: 2e69 6c6f 635b 3a33 5d2e 696c 6f63 5b32  .iloc[:3].iloc[2
-0001ae40: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-0001ae50: 616e 6420 280d 0a20 2020 2020 2020 2020  and (..         
-0001ae60: 2020 2020 2020 2028 6d61 6364 4c69 6e65         (macdLine
-0001ae70: 2e69 6c6f 635b 3a33 5d2e 696c 6f63 5b32  .iloc[:3].iloc[2
-0001ae80: 5d20 2d20 6d61 6364 5369 676e 616c 2e69  ] - macdSignal.i
-0001ae90: 6c6f 635b 3a33 5d2e 696c 6f63 5b32 5d29  loc[:3].iloc[2])
-0001aea0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001aeb0: 2020 2d20 286d 6163 644c 696e 652e 696c    - (macdLine.il
-0001aec0: 6f63 5b3a 325d 2e69 6c6f 635b 315d 202d  oc[:2].iloc[1] -
-0001aed0: 206d 6163 6453 6967 6e61 6c2e 696c 6f63   macdSignal.iloc
-0001aee0: 5b3a 325d 2e69 6c6f 635b 315d 290d 0a20  [:2].iloc[1]).. 
-0001aef0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0001af00: 2031 0d0a 2020 2020 2020 2020 2020 2020   1..            
-0001af10: 290d 0a20 2020 2020 2020 2029 0d0a 0d0a  )..        )....
-0001af20: 2020 2020 2340 6d65 6173 7572 655f 7469      #@measure_ti
-0001af30: 6d65 0d0a 2020 2020 2320 7661 6c69 6461  me..    # valida
-0001af40: 7465 2069 6620 4343 4920 6973 2077 6974  te if CCI is wit
-0001af50: 6869 6e20 6769 7665 6e20 7261 6e67 650d  hin given range.
-0001af60: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
-0001af70: 6543 4349 2873 656c 662c 2064 662c 2073  eCCI(self, df, s
-0001af80: 6372 6565 6e44 6963 742c 2073 6176 6544  creenDict, saveD
-0001af90: 6963 742c 206d 696e 4343 492c 206d 6178  ict, minCCI, max
-0001afa0: 4343 4929 3a0d 0a20 2020 2020 2020 2069  CCI):..        i
-0001afb0: 6620 6466 2069 7320 4e6f 6e65 206f 7220  f df is None or 
-0001afc0: 6c65 6e28 6466 2920 3d3d 2030 3a0d 0a20  len(df) == 0:.. 
-0001afd0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0001afe0: 6e20 4661 6c73 650d 0a20 2020 2020 2020  n False..       
-0001aff0: 2064 6174 6120 3d20 6466 2e63 6f70 7928   data = df.copy(
-0001b000: 290d 0a20 2020 2020 2020 2064 6174 6120  )..        data 
-0001b010: 3d20 6461 7461 2e66 696c 6c6e 6128 3029  = data.fillna(0)
-0001b020: 0d0a 2020 2020 2020 2020 6461 7461 203d  ..        data =
-0001b030: 2064 6174 612e 7265 706c 6163 6528 5b6e   data.replace([n
-0001b040: 702e 696e 662c 202d 6e70 2e69 6e66 5d2c  p.inf, -np.inf],
-0001b050: 2030 290d 0a20 2020 2020 2020 2063 6369   0)..        cci
-0001b060: 203d 2069 6e74 2864 6174 612e 6865 6164   = int(data.head
-0001b070: 2831 295b 2243 4349 225d 2e69 6c6f 635b  (1)["CCI"].iloc[
-0001b080: 305d 290d 0a20 2020 2020 2020 2073 6176  0])..        sav
-0001b090: 6544 6963 745b 2243 4349 225d 203d 2063  eDict["CCI"] = c
-0001b0a0: 6369 0d0a 2020 2020 2020 2020 6966 2028  ci..        if (
-0001b0b0: 6363 6920 3e3d 206d 696e 4343 4920 616e  cci >= minCCI an
-0001b0c0: 6420 6363 6920 3c3d 206d 6178 4343 4929  d cci <= maxCCI)
-0001b0d0: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
-0001b0e0: 6620 2822 5570 2220 696e 2073 6176 6544  f ("Up" in saveD
-0001b0f0: 6963 745b 2254 7265 6e64 225d 293a 0d0a  ict["Trend"]):..
-0001b100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b110: 7363 7265 656e 4469 6374 5b22 4343 4922  screenDict["CCI"
-0001b120: 5d20 3d20 280d 0a20 2020 2020 2020 2020  ] = (..         
-0001b130: 2020 2020 2020 2020 2020 2028 636f 6c6f             (colo
-0001b140: 7254 6578 742e 424f 4c44 2069 6620 2822  rText.BOLD if ("
-0001b150: 5374 726f 6e67 2220 696e 2073 6176 6544  Strong" in saveD
-0001b160: 6963 745b 2254 7265 6e64 225d 2920 656c  ict["Trend"]) el
-0001b170: 7365 2022 2229 202b 2063 6f6c 6f72 5465  se "") + colorTe
-0001b180: 7874 2e47 5245 454e 202b 2073 7472 2863  xt.GREEN + str(c
-0001b190: 6369 2920 2b20 636f 6c6f 7254 6578 742e  ci) + colorText.
-0001b1a0: 454e 440d 0a20 2020 2020 2020 2020 2020  END..           
-0001b1b0: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
-0001b1c0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-0001b1d0: 2020 2020 2020 2020 2020 2073 6372 6565             scree
-0001b1e0: 6e44 6963 745b 2243 4349 225d 203d 2028  nDict["CCI"] = (
-0001b1f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001b200: 2020 2020 2020 2863 6f6c 6f72 5465 7874        (colorText
-0001b210: 2e42 4f4c 4420 6966 2028 2253 7472 6f6e  .BOLD if ("Stron
-0001b220: 6722 2069 6e20 7361 7665 4469 6374 5b22  g" in saveDict["
-0001b230: 5472 656e 6422 5d29 2065 6c73 6520 2222  Trend"]) else ""
-0001b240: 2920 2b20 636f 6c6f 7254 6578 742e 4641  ) + colorText.FA
-0001b250: 494c 202b 2073 7472 2863 6369 2920 2b20  IL + str(cci) + 
-0001b260: 636f 6c6f 7254 6578 742e 454e 440d 0a20  colorText.END.. 
-0001b270: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0001b280: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-0001b290: 7475 726e 2054 7275 650d 0a20 2020 2020  turn True..     
-0001b2a0: 2020 2073 6372 6565 6e44 6963 745b 2243     screenDict["C
-0001b2b0: 4349 225d 203d 2063 6f6c 6f72 5465 7874  CI"] = colorText
-0001b2c0: 2e42 4f4c 4420 2b20 636f 6c6f 7254 6578  .BOLD + colorTex
-0001b2d0: 742e 4641 494c 202b 2073 7472 2863 6369  t.FAIL + str(cci
-0001b2e0: 2920 2b20 636f 6c6f 7254 6578 742e 454e  ) + colorText.EN
-0001b2f0: 440d 0a20 2020 2020 2020 2072 6574 7572  D..        retur
-0001b300: 6e20 4661 6c73 650d 0a0d 0a20 2020 2023  n False....    #
-0001b310: 2046 696e 6420 436f 6e66 6c75 6365 6e63   Find Conflucenc
-0001b320: 650d 0a20 2020 2064 6566 2076 616c 6964  e..    def valid
-0001b330: 6174 6543 6f6e 666c 7565 6e63 6528 7365  ateConfluence(se
-0001b340: 6c66 2c20 7374 6f63 6b2c 2064 662c 2073  lf, stock, df, s
-0001b350: 6372 6565 6e44 6963 742c 2073 6176 6544  creenDict, saveD
-0001b360: 6963 742c 2070 6572 6365 6e74 6167 653d  ict, percentage=
-0001b370: 302e 312c 636f 6e66 4669 6c74 6572 3d33  0.1,confFilter=3
-0001b380: 293a 0d0a 2020 2020 2020 2020 6966 2064  ):..        if d
-0001b390: 6620 6973 204e 6f6e 6520 6f72 206c 656e  f is None or len
-0001b3a0: 2864 6629 203d 3d20 303a 0d0a 2020 2020  (df) == 0:..    
-0001b3b0: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-0001b3c0: 616c 7365 0d0a 2020 2020 2020 2020 6461  alse..        da
-0001b3d0: 7461 203d 2064 662e 636f 7079 2829 0d0a  ta = df.copy()..
-0001b3e0: 2020 2020 2020 2020 7265 6365 6e74 203d          recent =
-0001b3f0: 2064 6174 612e 6865 6164 2832 290d 0a20   data.head(2).. 
-0001b400: 2020 2020 2020 2069 6620 6c65 6e28 7265         if len(re
-0001b410: 6365 6e74 2920 3c20 323a 0d0a 2020 2020  cent) < 2:..    
-0001b420: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-0001b430: 616c 7365 0d0a 2020 2020 2020 2020 6973  alse..        is
-0001b440: 3530 444d 4155 7054 7265 6e64 203d 2028  50DMAUpTrend = (
-0001b450: 7265 6365 6e74 5b22 534d 4122 5d2e 696c  recent["SMA"].il
-0001b460: 6f63 5b30 5d20 3e20 7265 6365 6e74 5b22  oc[0] > recent["
-0001b470: 534d 4122 5d2e 696c 6f63 5b31 5d29 0d0a  SMA"].iloc[1])..
-0001b480: 2020 2020 2020 2020 6973 3530 444d 4144          is50DMAD
-0001b490: 6f77 6e54 7265 6e64 203d 2028 7265 6365  ownTrend = (rece
-0001b4a0: 6e74 5b22 534d 4122 5d2e 696c 6f63 5b30  nt["SMA"].iloc[0
-0001b4b0: 5d20 3c20 7265 6365 6e74 5b22 534d 4122  ] < recent["SMA"
-0001b4c0: 5d2e 696c 6f63 5b31 5d29 0d0a 2020 2020  ].iloc[1])..    
-0001b4d0: 2020 2020 6973 476f 6c64 656e 4372 6f73      isGoldenCros
-0001b4e0: 734f 7665 7220 3d20 2872 6563 656e 745b  sOver = (recent[
-0001b4f0: 2253 4d41 225d 2e69 6c6f 635b 305d 203e  "SMA"].iloc[0] >
-0001b500: 3d20 7265 6365 6e74 5b22 4c4d 4122 5d2e  = recent["LMA"].
-0001b510: 696c 6f63 5b30 5d29 2061 6e64 205c 0d0a  iloc[0]) and \..
-0001b520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b530: 2020 2020 2020 2020 2020 2020 2872 6563              (rec
-0001b540: 656e 745b 2253 4d41 225d 2e69 6c6f 635b  ent["SMA"].iloc[
-0001b550: 315d 203c 3d20 7265 6365 6e74 5b22 4c4d  1] <= recent["LM
-0001b560: 4122 5d2e 696c 6f63 5b31 5d29 0d0a 2020  A"].iloc[1])..  
-0001b570: 2020 2020 2020 6973 4465 6164 4372 6f73        isDeadCros
-0001b580: 734f 7665 7220 3d20 2872 6563 656e 745b  sOver = (recent[
-0001b590: 2253 4d41 225d 2e69 6c6f 635b 305d 203c  "SMA"].iloc[0] <
-0001b5a0: 3d20 7265 6365 6e74 5b22 4c4d 4122 5d2e  = recent["LMA"].
-0001b5b0: 696c 6f63 5b30 5d29 2061 6e64 205c 0d0a  iloc[0]) and \..
-0001b5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b5d0: 2020 2020 2020 2020 2020 2020 2872 6563              (rec
-0001b5e0: 656e 745b 2253 4d41 225d 2e69 6c6f 635b  ent["SMA"].iloc[
-0001b5f0: 315d 203e 3d20 7265 6365 6e74 5b22 4c4d  1] >= recent["LM
-0001b600: 4122 5d2e 696c 6f63 5b31 5d29 0d0a 2020  A"].iloc[1])..  
-0001b610: 2020 2020 2020 6973 3530 444d 4120 3d20        is50DMA = 
-0001b620: 2872 6563 656e 745b 2253 4d41 225d 2e69  (recent["SMA"].i
-0001b630: 6c6f 635b 305d 203c 3d20 7265 6365 6e74  loc[0] <= recent
-0001b640: 5b22 436c 6f73 6522 5d2e 696c 6f63 5b30  ["Close"].iloc[0
-0001b650: 5d29 0d0a 2020 2020 2020 2020 6973 3230  ])..        is20
-0001b660: 3044 4d41 203d 2028 7265 6365 6e74 5b22  0DMA = (recent["
-0001b670: 4c4d 4122 5d2e 696c 6f63 5b30 5d20 3c3d  LMA"].iloc[0] <=
-0001b680: 2072 6563 656e 745b 2243 6c6f 7365 225d   recent["Close"]
-0001b690: 2e69 6c6f 635b 305d 290d 0a20 2020 2020  .iloc[0])..     
-0001b6a0: 2020 2064 6966 6665 7265 6e63 6520 3d20     difference = 
-0001b6b0: 726f 756e 6428 2872 6563 656e 745b 2253  round((recent["S
-0001b6c0: 4d41 225d 2e69 6c6f 635b 305d 202d 2072  MA"].iloc[0] - r
-0001b6d0: 6563 656e 745b 224c 4d41 225d 2e69 6c6f  ecent["LMA"].ilo
-0001b6e0: 635b 305d 290d 0a20 2020 2020 2020 2020  c[0])..         
-0001b6f0: 2020 2020 2020 202f 2072 6563 656e 745b         / recent[
-0001b700: 2243 6c6f 7365 225d 2e69 6c6f 635b 305d  "Close"].iloc[0]
-0001b710: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001b720: 2020 2a20 3130 302c 0d0a 2020 2020 2020    * 100,..      
-0001b730: 2020 2020 2020 2020 2020 322c 0d0a 2020            2,..  
-0001b740: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
-0001b750: 2020 2020 2073 6176 6544 6963 745b 2243       saveDict["C
-0001b760: 6f6e 6644 4d41 4469 6666 6572 656e 6365  onfDMADifference
-0001b770: 225d 203d 2064 6966 6665 7265 6e63 650d  "] = difference.
-0001b780: 0a20 2020 2020 2020 2073 6372 6565 6e44  .        screenD
-0001b790: 6963 745b 2243 6f6e 6644 4d41 4469 6666  ict["ConfDMADiff
-0001b7a0: 6572 656e 6365 225d 203d 2064 6966 6665  erence"] = diffe
-0001b7b0: 7265 6e63 650d 0a20 2020 2020 2020 2073  rence..        s
-0001b7c0: 6176 6564 203d 2073 656c 662e 6669 6e64  aved = self.find
-0001b7d0: 4375 7272 656e 7453 6176 6564 5661 6c75  CurrentSavedValu
-0001b7e0: 6528 7363 7265 656e 4469 6374 2c73 6176  e(screenDict,sav
-0001b7f0: 6544 6963 742c 224d 412d 5369 676e 616c  eDict,"MA-Signal
-0001b800: 2229 0d0a 2020 2020 2020 2020 2320 6469  ")..        # di
-0001b810: 6666 6572 656e 6365 203d 2061 6273 2864  fference = abs(d
-0001b820: 6966 6665 7265 6e63 6529 0d0a 2020 2020  ifference)..    
-0001b830: 2020 2020 636f 6e66 5465 7874 203d 2066      confText = f
-0001b840: 227b 2747 6f6c 6465 6e43 726f 7373 6f76  "{'GoldenCrossov
-0001b850: 6572 2720 6966 2069 7347 6f6c 6465 6e43  er' if isGoldenC
-0001b860: 726f 7373 4f76 6572 2065 6c73 6520 2827  rossOver else ('
-0001b870: 4465 6164 4372 6f73 736f 7665 7227 2069  DeadCrossover' i
-0001b880: 6620 6973 4465 6164 4372 6f73 734f 7665  f isDeadCrossOve
-0001b890: 7220 656c 7365 2028 2743 6f6e 662e 5570  r else ('Conf.Up
-0001b8a0: 2720 6966 2069 7335 3044 4d41 5570 5472  ' if is50DMAUpTr
-0001b8b0: 656e 6420 656c 7365 2028 2743 6f6e 662e  end else ('Conf.
-0001b8c0: 446f 776e 2720 6966 2069 7335 3044 4d41  Down' if is50DMA
-0001b8d0: 446f 776e 5472 656e 6420 656c 7365 2028  DownTrend else (
-0001b8e0: 2735 3044 4d41 2720 6966 2069 7335 3044  '50DMA' if is50D
-0001b8f0: 4d41 2065 6c73 6520 2827 3230 3044 4d41  MA else ('200DMA
-0001b900: 2720 6966 2069 7332 3030 444d 4120 656c  ' if is200DMA el
-0001b910: 7365 2027 556e 6b6e 6f77 6e27 2929 2929  se 'Unknown'))))
-0001b920: 297d 220d 0a20 2020 2020 2020 2069 6620  )}"..        if 
-0001b930: 6162 7328 7265 6365 6e74 5b22 534d 4122  abs(recent["SMA"
-0001b940: 5d2e 696c 6f63 5b30 5d20 2d20 7265 6365  ].iloc[0] - rece
-0001b950: 6e74 5b22 4c4d 4122 5d2e 696c 6f63 5b30  nt["LMA"].iloc[0
-0001b960: 5d29 203c 3d20 280d 0a20 2020 2020 2020  ]) <= (..       
-0001b970: 2020 2020 2072 6563 656e 745b 2253 4d41       recent["SMA
-0001b980: 225d 2e69 6c6f 635b 305d 202a 2070 6572  "].iloc[0] * per
-0001b990: 6365 6e74 6167 650d 0a20 2020 2020 2020  centage..       
-0001b9a0: 2029 3a0d 0a20 2020 2020 2020 2020 2020   ):..           
-0001b9b0: 2069 6620 7265 6365 6e74 5b22 534d 4122   if recent["SMA"
-0001b9c0: 5d2e 696c 6f63 5b30 5d20 3e3d 2072 6563  ].iloc[0] >= rec
-0001b9d0: 656e 745b 224c 4d41 225d 2e69 6c6f 635b  ent["LMA"].iloc[
-0001b9e0: 305d 3a0d 0a20 2020 2020 2020 2020 2020  0]:..           
-0001b9f0: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
-0001ba00: 224d 412d 5369 676e 616c 225d 203d 2028  "MA-Signal"] = (
-0001ba10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001ba20: 2020 2020 2020 7361 7665 645b 305d 200d        saved[0] .
-0001ba30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001ba40: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
-0001ba50: 2e42 4f4c 440d 0a20 2020 2020 2020 2020  .BOLD..         
-0001ba60: 2020 2020 2020 2020 2020 202b 2028 636f             + (co
-0001ba70: 6c6f 7254 6578 742e 4752 4545 4e20 6966  lorText.GREEN if
-0001ba80: 2069 7335 3044 4d41 5570 5472 656e 6420   is50DMAUpTrend 
-0001ba90: 656c 7365 2028 636f 6c6f 7254 6578 742e  else (colorText.
-0001baa0: 4641 494c 2069 6620 6973 3530 444d 4144  FAIL if is50DMAD
-0001bab0: 6f77 6e54 7265 6e64 2065 6c73 6520 636f  ownTrend else co
-0001bac0: 6c6f 7254 6578 742e 5741 524e 2929 0d0a  lorText.WARN))..
-0001bad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bae0: 2020 2020 2b20 6622 7b63 6f6e 6654 6578      + f"{confTex
-0001baf0: 747d 2028 7b64 6966 6665 7265 6e63 657d  t} ({difference}
-0001bb00: 2529 220d 0a20 2020 2020 2020 2020 2020  %)"..           
-0001bb10: 2020 2020 2020 2020 202b 2063 6f6c 6f72           + color
-0001bb20: 5465 7874 2e45 4e44 0d0a 2020 2020 2020  Text.END..      
-0001bb30: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
-0001bb40: 2020 2020 2020 2020 2020 2020 2073 6176               sav
-0001bb50: 6544 6963 745b 224d 412d 5369 676e 616c  eDict["MA-Signal
-0001bb60: 225d 203d 2073 6176 6564 5b31 5d20 2b20  "] = saved[1] + 
-0001bb70: 6622 7b63 6f6e 6654 6578 747d 2028 7b64  f"{confText} ({d
-0001bb80: 6966 6665 7265 6e63 657d 2529 220d 0a20  ifference}%)".. 
-0001bb90: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0001bba0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001bbb0: 2020 7363 7265 656e 4469 6374 5b22 4d41    screenDict["MA
-0001bbc0: 2d53 6967 6e61 6c22 5d20 3d20 280d 0a20  -Signal"] = (.. 
-0001bbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bbe0: 2020 2073 6176 6564 5b30 5d20 0d0a 2020     saved[0] ..  
-0001bbf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bc00: 2020 2b20 636f 6c6f 7254 6578 742e 424f    + colorText.BO
-0001bc10: 4c44 0d0a 2020 2020 2020 2020 2020 2020  LD..            
-0001bc20: 2020 2020 2020 2020 2b20 2863 6f6c 6f72          + (color
-0001bc30: 5465 7874 2e47 5245 454e 2069 6620 6973  Text.GREEN if is
-0001bc40: 3530 444d 4155 7054 7265 6e64 2065 6c73  50DMAUpTrend els
-0001bc50: 6520 2863 6f6c 6f72 5465 7874 2e46 4149  e (colorText.FAI
-0001bc60: 4c20 6966 2069 7335 3044 4d41 446f 776e  L if is50DMADown
-0001bc70: 5472 656e 6420 656c 7365 2063 6f6c 6f72  Trend else color
-0001bc80: 5465 7874 2e57 4152 4e29 290d 0a20 2020  Text.WARN))..   
-0001bc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bca0: 202b 2066 227b 636f 6e66 5465 7874 7d20   + f"{confText} 
-0001bcb0: 287b 6469 6666 6572 656e 6365 7d25 2922  ({difference}%)"
-0001bcc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001bcd0: 2020 2020 2020 2b20 636f 6c6f 7254 6578        + colorTex
-0001bce0: 742e 454e 440d 0a20 2020 2020 2020 2020  t.END..         
-0001bcf0: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-0001bd00: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
-0001bd10: 6374 5b22 4d41 2d53 6967 6e61 6c22 5d20  ct["MA-Signal"] 
-0001bd20: 3d20 7361 7665 645b 315d 202b 2066 227b  = saved[1] + f"{
-0001bd30: 636f 6e66 5465 7874 7d20 287b 6469 6666  confText} ({diff
-0001bd40: 6572 656e 6365 7d25 2922 0d0a 2020 2020  erence}%)"..    
-0001bd50: 2020 2020 2020 2020 7265 7475 726e 2063          return c
-0001bd60: 6f6e 6646 696c 7465 7220 3d3d 2033 206f  onfFilter == 3 o
-0001bd70: 7220 5c0d 0a20 2020 2020 2020 2020 2020  r \..           
-0001bd80: 2020 2020 2028 636f 6e66 4669 6c74 6572       (confFilter
-0001bd90: 203d 3d20 3120 616e 6420 2869 7335 3044   == 1 and (is50D
-0001bda0: 4d41 5570 5472 656e 6420 6f72 2028 6973  MAUpTrend or (is
-0001bdb0: 476f 6c64 656e 4372 6f73 734f 7665 7220  GoldenCrossOver 
-0001bdc0: 6f72 2027 5570 2720 696e 2063 6f6e 6654  or 'Up' in confT
-0001bdd0: 6578 7429 2929 206f 7220 5c0d 0a20 2020  ext))) or \..   
-0001bde0: 2020 2020 2020 2020 2020 2020 2028 636f               (co
-0001bdf0: 6e66 4669 6c74 6572 203d 3d20 3220 616e  nfFilter == 2 an
-0001be00: 6420 2869 7335 3044 4d41 446f 776e 5472  d (is50DMADownTr
-0001be10: 656e 6420 6f72 2069 7344 6561 6443 726f  end or isDeadCro
-0001be20: 7373 4f76 6572 206f 7220 2744 6f77 6e27  ssOver or 'Down'
-0001be30: 2069 6e20 636f 6e66 5465 7874 2929 0d0a   in confText))..
-0001be40: 2020 2020 2020 2020 2320 4d61 7962 6520          # Maybe 
-0001be50: 7468 6520 6469 6666 6572 656e 6365 2069  the difference i
-0001be60: 7320 6e6f 7420 7769 7468 696e 2074 6865  s not within the
-0001be70: 2072 616e 6765 2c20 6275 7420 7765 2764   range, but we'd
-0001be80: 2073 7469 6c6c 206c 696b 6520 746f 206b   still like to k
-0001be90: 6565 7020 7468 6520 7374 6f63 6b20 696e  eep the stock in
-0001bea0: 0d0a 2020 2020 2020 2020 2320 7468 6520  ..        # the 
-0001beb0: 6c69 7374 2069 6620 6974 2773 2061 2067  list if it's a g
-0001bec0: 6f6c 6465 6e20 6372 6f73 736f 7665 7220  olden crossover 
-0001bed0: 6f72 2064 6561 6420 6372 6f73 736f 7665  or dead crossove
-0001bee0: 720d 0a20 2020 2020 2020 2069 6620 6973  r..        if is
-0001bef0: 476f 6c64 656e 4372 6f73 734f 7665 7220  GoldenCrossOver 
-0001bf00: 6f72 2069 7344 6561 6443 726f 7373 4f76  or isDeadCrossOv
-0001bf10: 6572 3a0d 0a20 2020 2020 2020 2020 2020  er:..           
-0001bf20: 2073 6372 6565 6e44 6963 745b 224d 412d   screenDict["MA-
-0001bf30: 5369 676e 616c 225d 203d 2028 0d0a 2020  Signal"] = (..  
-0001bf40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bf50: 2020 7361 7665 645b 305d 200d 0a20 2020    saved[0] ..   
-0001bf60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bf70: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
-0001bf80: 440d 0a20 2020 2020 2020 2020 2020 2020  D..             
-0001bf90: 2020 2020 2020 202b 2028 636f 6c6f 7254         + (colorT
-0001bfa0: 6578 742e 4752 4545 4e20 6966 2069 7335  ext.GREEN if is5
-0001bfb0: 3044 4d41 5570 5472 656e 6420 656c 7365  0DMAUpTrend else
-0001bfc0: 2028 636f 6c6f 7254 6578 742e 4641 494c   (colorText.FAIL
-0001bfd0: 2069 6620 6973 3530 444d 4144 6f77 6e54   if is50DMADownT
-0001bfe0: 7265 6e64 2065 6c73 6520 636f 6c6f 7254  rend else colorT
-0001bff0: 6578 742e 5741 524e 2929 0d0a 2020 2020  ext.WARN))..    
-0001c000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c010: 2b20 6622 7b63 6f6e 6654 6578 747d 2028  + f"{confText} (
-0001c020: 7b64 6966 6665 7265 6e63 657d 2529 220d  {difference}%)".
-0001c030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001c040: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
-0001c050: 2e45 4e44 0d0a 2020 2020 2020 2020 2020  .END..          
-0001c060: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-0001c070: 2020 2020 2073 6176 6544 6963 745b 224d       saveDict["M
-0001c080: 412d 5369 676e 616c 225d 203d 2073 6176  A-Signal"] = sav
-0001c090: 6564 5b31 5d20 2b20 6622 7b63 6f6e 6654  ed[1] + f"{confT
-0001c0a0: 6578 747d 2028 7b64 6966 6665 7265 6e63  ext} ({differenc
-0001c0b0: 657d 2529 220d 0a20 2020 2020 2020 2020  e}%)"..         
-0001c0c0: 2020 2072 6574 7572 6e20 636f 6e66 4669     return confFi
-0001c0d0: 6c74 6572 203d 3d20 3320 6f72 205c 0d0a  lter == 3 or \..
-0001c0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c0f0: 2863 6f6e 6646 696c 7465 7220 3d3d 2031  (confFilter == 1
-0001c100: 2061 6e64 2069 7347 6f6c 6465 6e43 726f   and isGoldenCro
-0001c110: 7373 4f76 6572 2920 6f72 205c 0d0a 2020  ssOver) or \..  
-0001c120: 2020 2020 2020 2020 2020 2020 2020 2863                (c
-0001c130: 6f6e 6646 696c 7465 7220 3d3d 2032 2061  onfFilter == 2 a
-0001c140: 6e64 2069 7344 6561 6443 726f 7373 4f76  nd isDeadCrossOv
-0001c150: 6572 290d 0a20 2020 2020 2020 2072 6574  er)..        ret
-0001c160: 7572 6e20 4661 6c73 650d 0a0d 0a20 2020  urn False....   
-0001c170: 2023 406d 6561 7375 7265 5f74 696d 650d   #@measure_time.
-0001c180: 0a20 2020 2023 2056 616c 6964 6174 6520  .    # Validate 
-0001c190: 6966 2073 6861 7265 2070 7269 6365 7320  if share prices 
-0001c1a0: 6172 6520 636f 6e73 6f6c 6964 6174 696e  are consolidatin
-0001c1b0: 670d 0a20 2020 2064 6566 2076 616c 6964  g..    def valid
-0001c1c0: 6174 6543 6f6e 736f 6c69 6461 7469 6f6e  ateConsolidation
-0001c1d0: 2873 656c 662c 2064 662c 2073 6372 6565  (self, df, scree
-0001c1e0: 6e44 6963 742c 2073 6176 6544 6963 742c  nDict, saveDict,
-0001c1f0: 2070 6572 6365 6e74 6167 653d 3130 293a   percentage=10):
-0001c200: 0d0a 2020 2020 2020 2020 6966 2064 6620  ..        if df 
-0001c210: 6973 204e 6f6e 6520 6f72 206c 656e 2864  is None or len(d
-0001c220: 6629 203d 3d20 303a 0d0a 2020 2020 2020  f) == 0:..      
-0001c230: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-0001c240: 7365 0d0a 2020 2020 2020 2020 6461 7461  se..        data
-0001c250: 203d 2064 662e 636f 7079 2829 0d0a 2020   = df.copy()..  
-0001c260: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
-0001c270: 612e 6669 6c6c 6e61 2830 290d 0a20 2020  a.fillna(0)..   
-0001c280: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
-0001c290: 2e72 6570 6c61 6365 285b 6e70 2e69 6e66  .replace([np.inf
-0001c2a0: 2c20 2d6e 702e 696e 665d 2c20 3029 0d0a  , -np.inf], 0)..
-0001c2b0: 2020 2020 2020 2020 6863 203d 2064 6174          hc = dat
-0001c2c0: 612e 6465 7363 7269 6265 2829 5b22 436c  a.describe()["Cl
-0001c2d0: 6f73 6522 5d5b 226d 6178 225d 0d0a 2020  ose"]["max"]..  
-0001c2e0: 2020 2020 2020 6c63 203d 2064 6174 612e        lc = data.
-0001c2f0: 6465 7363 7269 6265 2829 5b22 436c 6f73  describe()["Clos
-0001c300: 6522 5d5b 226d 696e 225d 0d0a 2020 2020  e"]["min"]..    
-0001c310: 2020 2020 6966 2028 6863 202d 206c 6329      if (hc - lc)
-0001c320: 203c 3d20 2868 6320 2a20 7065 7263 656e   <= (hc * percen
-0001c330: 7461 6765 202f 2031 3030 2920 616e 6420  tage / 100) and 
-0001c340: 2868 6320 2d20 6c63 2021 3d20 3029 3a0d  (hc - lc != 0):.
-0001c350: 0a20 2020 2020 2020 2020 2020 2073 6372  .            scr
-0001c360: 6565 6e44 6963 745b 2243 6f6e 736f 6c2e  eenDict["Consol.
-0001c370: 225d 203d 2028 0d0a 2020 2020 2020 2020  "] = (..        
-0001c380: 2020 2020 2020 2020 636f 6c6f 7254 6578          colorTex
-0001c390: 742e 424f 4c44 0d0a 2020 2020 2020 2020  t.BOLD..        
-0001c3a0: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
-0001c3b0: 6578 742e 4752 4545 4e0d 0a20 2020 2020  ext.GREEN..     
-0001c3c0: 2020 2020 2020 2020 2020 202b 2022 5261             + "Ra
-0001c3d0: 6e67 653a 220d 0a20 2020 2020 2020 2020  nge:"..         
-0001c3e0: 2020 2020 2020 202b 2073 7472 2872 6f75         + str(rou
-0001c3f0: 6e64 2828 6162 7328 2868 6320 2d20 6c63  nd((abs((hc - lc
-0001c400: 2920 2f20 6863 2920 2a20 3130 3029 2c20  ) / hc) * 100), 
-0001c410: 3129 290d 0a20 2020 2020 2020 2020 2020  1))..           
-0001c420: 2020 2020 202b 2022 2522 0d0a 2020 2020       + "%"..    
-0001c430: 2020 2020 2020 2020 2020 2020 2b20 636f              + co
-0001c440: 6c6f 7254 6578 742e 454e 440d 0a20 2020  lorText.END..   
-0001c450: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
-0001c460: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-0001c470: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
-0001c480: 745b 2243 6f6e 736f 6c2e 225d 203d 2028  t["Consol."] = (
-0001c490: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001c4a0: 2020 636f 6c6f 7254 6578 742e 424f 4c44    colorText.BOLD
-0001c4b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001c4c0: 2020 2b20 636f 6c6f 7254 6578 742e 4641    + colorText.FA
-0001c4d0: 494c 0d0a 2020 2020 2020 2020 2020 2020  IL..            
-0001c4e0: 2020 2020 2b20 2252 616e 6765 3a22 0d0a      + "Range:"..
-0001c4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c500: 2b20 7374 7228 726f 756e 6428 2861 6273  + str(round((abs
-0001c510: 2828 6863 202d 206c 6329 202f 2068 6329  ((hc - lc) / hc)
-0001c520: 202a 2031 3030 292c 2031 2929 0d0a 2020   * 100), 1))..  
-0001c530: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-0001c540: 2225 220d 0a20 2020 2020 2020 2020 2020  "%"..           
-0001c550: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
-0001c560: 2e45 4e44 0d0a 2020 2020 2020 2020 2020  .END..          
-0001c570: 2020 290d 0a20 2020 2020 2020 2073 6176    )..        sav
-0001c580: 6544 6963 745b 2243 6f6e 736f 6c2e 225d  eDict["Consol."]
-0001c590: 203d 2066 2752 616e 6765 3a7b 7374 7228   = f'Range:{str(
-0001c5a0: 726f 756e 6428 2861 6273 2828 6863 2d6c  round((abs((hc-l
-0001c5b0: 6329 2f68 6329 2a31 3030 292c 3129 292b  c)/hc)*100),1))+
-0001c5c0: 2225 227d 270d 0a20 2020 2020 2020 2072  "%"}'..        r
-0001c5d0: 6574 7572 6e20 726f 756e 6428 2861 6273  eturn round((abs
-0001c5e0: 2828 6863 202d 206c 6329 202f 2068 6329  ((hc - lc) / hc)
-0001c5f0: 202a 2031 3030 292c 2031 290d 0a0d 0a20   * 100), 1).... 
-0001c600: 2020 2023 2076 616c 6964 6174 6520 6966     # validate if
-0001c610: 2074 6865 2073 746f 636b 2068 6173 2062   the stock has b
-0001c620: 6565 6e20 6861 7669 6e67 2068 6967 6865  een having highe
-0001c630: 7220 6869 6768 732c 2068 6967 6865 7220  r highs, higher 
-0001c640: 6c6f 7773 0d0a 2020 2020 2320 616e 6420  lows..    # and 
-0001c650: 6869 6768 6572 2063 6c6f 7365 2077 6974  higher close wit
-0001c660: 6820 6c61 7465 7374 2063 6c6f 7365 203e  h latest close >
-0001c670: 2073 7570 6572 7472 656e 6420 616e 6420   supertrend and 
-0001c680: 382d 454d 412e 0d0a 2020 2020 6465 6620  8-EMA...    def 
-0001c690: 7661 6c69 6461 7465 4869 6768 6572 4869  validateHigherHi
-0001c6a0: 6768 7348 6967 6865 724c 6f77 7348 6967  ghsHigherLowsHig
-0001c6b0: 6865 7243 6c6f 7365 2873 656c 662c 2064  herClose(self, d
-0001c6c0: 6629 3a0d 0a20 2020 2020 2020 2069 6620  f):..        if 
-0001c6d0: 6466 2069 7320 4e6f 6e65 206f 7220 6c65  df is None or le
-0001c6e0: 6e28 6466 2920 3d3d 2030 3a0d 0a20 2020  n(df) == 0:..   
-0001c6f0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0001c700: 4661 6c73 650d 0a20 2020 2020 2020 2064  False..        d
-0001c710: 6174 6120 3d20 6466 2e63 6f70 7928 290d  ata = df.copy().
-0001c720: 0a20 2020 2020 2020 2064 6179 3020 3d20  .        day0 = 
-0001c730: 6461 7461 0d0a 2020 2020 2020 2020 6461  data..        da
-0001c740: 7931 203d 2064 6174 615b 313a 5d0d 0a20  y1 = data[1:].. 
-0001c750: 2020 2020 2020 2064 6179 3220 3d20 6461         day2 = da
-0001c760: 7461 5b32 3a5d 0d0a 2020 2020 2020 2020  ta[2:]..        
-0001c770: 6461 7933 203d 2064 6174 615b 333a 5d0d  day3 = data[3:].
-0001c780: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
-0001c790: 6461 7931 2920 3c20 3120 6f72 206c 656e  day1) < 1 or len
-0001c7a0: 2864 6179 3229 203c 2031 206f 7220 6c65  (day2) < 1 or le
-0001c7b0: 6e28 6461 7933 2920 3c20 313a 0d0a 2020  n(day3) < 1:..  
-0001c7c0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0001c7d0: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
-0001c7e0: 6869 6768 6572 4869 6768 7320 3d20 280d  higherHighs = (.
-0001c7f0: 0a20 2020 2020 2020 2020 2020 2028 6461  .            (da
-0001c800: 7930 5b22 4869 6768 225d 2e69 6c6f 635b  y0["High"].iloc[
-0001c810: 305d 203e 2064 6179 315b 2248 6967 6822  0] > day1["High"
-0001c820: 5d2e 696c 6f63 5b30 5d29 0d0a 2020 2020  ].iloc[0])..    
-0001c830: 2020 2020 2020 2020 616e 6420 2864 6179          and (day
-0001c840: 315b 2248 6967 6822 5d2e 696c 6f63 5b30  1["High"].iloc[0
-0001c850: 5d20 3e20 6461 7932 5b22 4869 6768 225d  ] > day2["High"]
-0001c860: 2e69 6c6f 635b 305d 290d 0a20 2020 2020  .iloc[0])..     
-0001c870: 2020 2020 2020 2061 6e64 2028 6461 7932         and (day2
-0001c880: 5b22 4869 6768 225d 2e69 6c6f 635b 305d  ["High"].iloc[0]
-0001c890: 203e 2064 6179 335b 2248 6967 6822 5d2e   > day3["High"].
-0001c8a0: 696c 6f63 5b30 5d29 0d0a 2020 2020 2020  iloc[0])..      
-0001c8b0: 2020 290d 0a20 2020 2020 2020 2068 6967    )..        hig
-0001c8c0: 6865 724c 6f77 7320 3d20 280d 0a20 2020  herLows = (..   
-0001c8d0: 2020 2020 2020 2020 2028 6461 7930 5b22           (day0["
-0001c8e0: 4c6f 7722 5d2e 696c 6f63 5b30 5d20 3e20  Low"].iloc[0] > 
-0001c8f0: 6461 7931 5b22 4c6f 7722 5d2e 696c 6f63  day1["Low"].iloc
-0001c900: 5b30 5d29 0d0a 2020 2020 2020 2020 2020  [0])..          
-0001c910: 2020 616e 6420 2864 6179 315b 224c 6f77    and (day1["Low
-0001c920: 225d 2e69 6c6f 635b 305d 203e 2064 6179  "].iloc[0] > day
-0001c930: 325b 224c 6f77 225d 2e69 6c6f 635b 305d  2["Low"].iloc[0]
-0001c940: 290d 0a20 2020 2020 2020 2020 2020 2061  )..            a
-0001c950: 6e64 2028 6461 7932 5b22 4c6f 7722 5d2e  nd (day2["Low"].
-0001c960: 696c 6f63 5b30 5d20 3e20 6461 7933 5b22  iloc[0] > day3["
-0001c970: 4c6f 7722 5d2e 696c 6f63 5b30 5d29 0d0a  Low"].iloc[0])..
-0001c980: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
-0001c990: 2020 2068 6967 6865 7243 6c6f 7365 203d     higherClose =
-0001c9a0: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
-0001c9b0: 2864 6179 305b 2243 6c6f 7365 225d 2e69  (day0["Close"].i
-0001c9c0: 6c6f 635b 305d 203e 2064 6179 315b 2243  loc[0] > day1["C
-0001c9d0: 6c6f 7365 225d 2e69 6c6f 635b 305d 290d  lose"].iloc[0]).
-0001c9e0: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
-0001c9f0: 2028 6461 7931 5b22 436c 6f73 6522 5d2e   (day1["Close"].
-0001ca00: 696c 6f63 5b30 5d20 3e20 6461 7932 5b22  iloc[0] > day2["
-0001ca10: 436c 6f73 6522 5d2e 696c 6f63 5b30 5d29  Close"].iloc[0])
-0001ca20: 0d0a 2020 2020 2020 2020 2020 2020 616e  ..            an
-0001ca30: 6420 2864 6179 325b 2243 6c6f 7365 225d  d (day2["Close"]
-0001ca40: 2e69 6c6f 635b 305d 203e 2064 6179 335b  .iloc[0] > day3[
-0001ca50: 2243 6c6f 7365 225d 2e69 6c6f 635b 305d  "Close"].iloc[0]
-0001ca60: 290d 0a20 2020 2020 2020 2029 0d0a 2020  )..        )..  
-0001ca70: 2020 2020 2020 2320 6869 6768 6572 5253        # higherRS
-0001ca80: 4920 3d20 2864 6179 305b 2252 5349 225d  I = (day0["RSI"]
-0001ca90: 2e69 6c6f 635b 305d 203e 2064 6179 315b  .iloc[0] > day1[
-0001caa0: 2252 5349 225d 2e69 6c6f 635b 305d 2920  "RSI"].iloc[0]) 
-0001cab0: 616e 6420 5c0d 0a20 2020 2020 2020 2023  and \..        #
-0001cac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cad0: 2028 6461 7931 5b22 5253 4922 5d2e 696c   (day1["RSI"].il
-0001cae0: 6f63 5b30 5d20 3e20 6461 7932 5b22 5253  oc[0] > day2["RS
-0001caf0: 4922 5d2e 696c 6f63 5b30 5d29 2061 6e64  I"].iloc[0]) and
-0001cb00: 205c 0d0a 2020 2020 2020 2020 2320 2020   \..        #   
-0001cb10: 2020 2020 2020 2020 2020 2020 2020 2864                (d
-0001cb20: 6179 325b 2252 5349 225d 2e69 6c6f 635b  ay2["RSI"].iloc[
-0001cb30: 305d 203e 2064 6179 335b 2252 5349 225d  0] > day3["RSI"]
-0001cb40: 2e69 6c6f 635b 305d 2920 616e 6420 5c0d  .iloc[0]) and \.
-0001cb50: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
-0001cb60: 2020 2020 2020 2020 2020 2064 6179 335b             day3[
-0001cb70: 2252 5349 225d 2e69 6c6f 635b 305d 203e  "RSI"].iloc[0] >
-0001cb80: 3d20 3530 2061 6e64 2064 6179 305b 2252  = 50 and day0["R
-0001cb90: 5349 225d 2e69 6c6f 635b 305d 203e 3d20  SI"].iloc[0] >= 
-0001cba0: 3635 0d0a 2020 2020 2020 2020 7265 7665  65..        reve
-0001cbb0: 7273 6564 4461 7461 203d 2064 6174 615b  rsedData = data[
-0001cbc0: 3a3a 2d31 5d2e 636f 7079 2829 0d0a 2020  ::-1].copy()..  
-0001cbd0: 2020 2020 2020 7265 7665 7273 6564 4461        reversedDa
-0001cbe0: 7461 5b22 5355 5045 5254 225d 203d 2070  ta["SUPERT"] = p
-0001cbf0: 6b74 616c 6962 2e73 7570 6572 7472 656e  ktalib.supertren
-0001cc00: 6428 7265 7665 7273 6564 4461 7461 2c20  d(reversedData, 
-0001cc10: 372c 2033 295b 2253 5550 4552 545f 375f  7, 3)["SUPERT_7_
-0001cc20: 332e 3022 5d0d 0a20 2020 2020 2020 2072  3.0"]..        r
-0001cc30: 6576 6572 7365 6444 6174 615b 2245 4d41  eversedData["EMA
-0001cc40: 3822 5d20 3d20 706b 7461 6c69 622e 454d  8"] = pktalib.EM
-0001cc50: 4128 7265 7665 7273 6564 4461 7461 5b22  A(reversedData["
-0001cc60: 436c 6f73 6522 5d2c 2074 696d 6570 6572  Close"], timeper
-0001cc70: 696f 643d 3929 0d0a 2020 2020 2020 2020  iod=9)..        
-0001cc80: 6869 6768 6572 436c 6f73 6520 3d20 280d  higherClose = (.
-0001cc90: 0a20 2020 2020 2020 2020 2020 2068 6967  .            hig
-0001cca0: 6865 7243 6c6f 7365 0d0a 2020 2020 2020  herClose..      
-0001ccb0: 2020 2020 2020 616e 6420 6461 7930 5b22        and day0["
-0001ccc0: 436c 6f73 6522 5d2e 696c 6f63 5b30 5d20  Close"].iloc[0] 
-0001ccd0: 3e20 7265 7665 7273 6564 4461 7461 2e74  > reversedData.t
-0001cce0: 6169 6c28 3129 5b22 5355 5045 5254 225d  ail(1)["SUPERT"]
-0001ccf0: 2e69 6c6f 635b 305d 0d0a 2020 2020 2020  .iloc[0]..      
-0001cd00: 2020 2020 2020 616e 6420 6461 7930 5b22        and day0["
-0001cd10: 436c 6f73 6522 5d2e 696c 6f63 5b30 5d20  Close"].iloc[0] 
-0001cd20: 3e20 7265 7665 7273 6564 4461 7461 2e74  > reversedData.t
-0001cd30: 6169 6c28 3129 5b22 454d 4138 225d 2e69  ail(1)["EMA8"].i
-0001cd40: 6c6f 635b 305d 0d0a 2020 2020 2020 2020  loc[0]..        
-0001cd50: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-0001cd60: 6e20 6869 6768 6572 4869 6768 7320 616e  n higherHighs an
-0001cd70: 6420 6869 6768 6572 4c6f 7773 2061 6e64  d higherLows and
-0001cd80: 2068 6967 6865 7243 6c6f 7365 0d0a 0d0a   higherClose....
-0001cd90: 2020 2020 2340 6d65 6173 7572 655f 7469      #@measure_ti
-0001cda0: 6d65 0d0a 2020 2020 2320 5661 6c69 6461  me..    # Valida
-0001cdb0: 7465 2027 496e 7369 6465 2042 6172 2720  te 'Inside Bar' 
-0001cdc0: 7374 7275 6374 7572 6520 666f 7220 7265  structure for re
-0001cdd0: 6365 6e74 2064 6179 730d 0a20 2020 2064  cent days..    d
-0001cde0: 6566 2076 616c 6964 6174 6549 6e73 6964  ef validateInsid
-0001cdf0: 6542 6172 280d 0a20 2020 2020 2020 2073  eBar(..        s
-0001ce00: 656c 662c 2064 662c 2073 6372 6565 6e44  elf, df, screenD
-0001ce10: 6963 742c 2073 6176 6544 6963 742c 2063  ict, saveDict, c
-0001ce20: 6861 7274 5061 7474 6572 6e3d 312c 2064  hartPattern=1, d
-0001ce30: 6179 7354 6f4c 6f6f 6b62 6163 6b3d 350d  aysToLookback=5.
-0001ce40: 0a20 2020 2029 3a0d 0a20 2020 2020 2020  .    ):..       
-0001ce50: 2069 6620 6466 2069 7320 4e6f 6e65 206f   if df is None o
-0001ce60: 7220 6c65 6e28 6466 2920 3d3d 2030 3a0d  r len(df) == 0:.
-0001ce70: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0001ce80: 7572 6e20 4661 6c73 650d 0a20 2020 2020  urn False..     
-0001ce90: 2020 2064 6174 6120 3d20 6466 2e63 6f70     data = df.cop
-0001cea0: 7928 290d 0a20 2020 2020 2020 206f 7267  y()..        org
-0001ceb0: 4461 7461 203d 2064 6174 610d 0a20 2020  Data = data..   
-0001cec0: 2020 2020 2073 6176 6564 203d 2073 656c       saved = sel
-0001ced0: 662e 6669 6e64 4375 7272 656e 7453 6176  f.findCurrentSav
-0001cee0: 6564 5661 6c75 6528 7363 7265 656e 4469  edValue(screenDi
-0001cef0: 6374 2c20 7361 7665 4469 6374 2c20 2250  ct, saveDict, "P
-0001cf00: 6174 7465 726e 2229 0d0a 2020 2020 2020  attern")..      
-0001cf10: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
-0001cf20: 2869 6e74 2864 6179 7354 6f4c 6f6f 6b62  (int(daysToLookb
-0001cf30: 6163 6b29 2c20 696e 7428 726f 756e 6428  ack), int(round(
-0001cf40: 6461 7973 546f 4c6f 6f6b 6261 636b 202a  daysToLookback *
-0001cf50: 2030 2e35 2929 202d 2031 2c20 2d31 293a   0.5)) - 1, -1):
-0001cf60: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-0001cf70: 2069 203d 3d20 323a 0d0a 2020 2020 2020   i == 2:..      
-0001cf80: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0001cf90: 2030 2020 2320 4578 6974 2069 6620 6f6e   0  # Exit if on
-0001cfa0: 6c79 206c 6173 7420 3220 6361 6e64 6c65  ly last 2 candle
-0001cfb0: 7320 6172 6520 6c65 6674 0d0a 2020 2020  s are left..    
-0001cfc0: 2020 2020 2020 2020 6966 2063 6861 7274          if chart
-0001cfd0: 5061 7474 6572 6e20 3d3d 2031 3a0d 0a20  Pattern == 1:.. 
-0001cfe0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0001cff0: 6620 2255 7022 2069 6e20 7361 7665 4469  f "Up" in saveDi
-0001d000: 6374 5b22 5472 656e 6422 5d20 616e 6420  ct["Trend"] and 
-0001d010: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
-0001d020: 2020 2020 2020 2022 4275 6c6c 2220 696e         "Bull" in
-0001d030: 2073 6176 6544 6963 745b 224d 412d 5369   saveDict["MA-Si
-0001d040: 676e 616c 225d 0d0a 2020 2020 2020 2020  gnal"]..        
-0001d050: 2020 2020 2020 2020 2020 2020 6f72 2022              or "
-0001d060: 5375 7070 6f72 7422 2069 6e20 7361 7665  Support" in save
-0001d070: 4469 6374 5b22 4d41 2d53 6967 6e61 6c22  Dict["MA-Signal"
-0001d080: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-0001d090: 2020 2029 3a0d 0a20 2020 2020 2020 2020     ):..         
-0001d0a0: 2020 2020 2020 2020 2020 2064 6174 6120             data 
-0001d0b0: 3d20 6f72 6744 6174 612e 6865 6164 2869  = orgData.head(i
-0001d0c0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0001d0d0: 2020 2020 2020 2072 6566 4361 6e64 6c65         refCandle
-0001d0e0: 203d 2064 6174 612e 7461 696c 2831 290d   = data.tail(1).
-0001d0f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001d100: 2020 2020 2069 6620 280d 0a20 2020 2020       if (..     
-0001d110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d120: 2020 2028 6c65 6e28 6461 7461 2e48 6967     (len(data.Hig
-0001d130: 685b 6461 7461 2e48 6967 6820 3e20 7265  h[data.High > re
-0001d140: 6643 616e 646c 652e 4869 6768 2e69 7465  fCandle.High.ite
-0001d150: 6d28 295d 2920 3d3d 2030 290d 0a20 2020  m()]) == 0)..   
-0001d160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d170: 2020 2020 2061 6e64 2028 6c65 6e28 6461       and (len(da
-0001d180: 7461 2e4c 6f77 5b64 6174 612e 4c6f 7720  ta.Low[data.Low 
-0001d190: 3c20 7265 6643 616e 646c 652e 4c6f 772e  < refCandle.Low.
-0001d1a0: 6974 656d 2829 5d29 203d 3d20 3029 0d0a  item()]) == 0)..
-0001d1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d1c0: 2020 2020 2020 2020 616e 6420 286c 656e          and (len
-0001d1d0: 2864 6174 612e 4f70 656e 5b64 6174 612e  (data.Open[data.
-0001d1e0: 4f70 656e 203e 2072 6566 4361 6e64 6c65  Open > refCandle
-0001d1f0: 2e48 6967 682e 6974 656d 2829 5d29 203d  .High.item()]) =
-0001d200: 3d20 3029 0d0a 2020 2020 2020 2020 2020  = 0)..          
-0001d210: 2020 2020 2020 2020 2020 2020 2020 616e                an
-0001d220: 6420 286c 656e 2864 6174 612e 436c 6f73  d (len(data.Clos
-0001d230: 655b 6461 7461 2e43 6c6f 7365 203c 2072  e[data.Close < r
-0001d240: 6566 4361 6e64 6c65 2e4c 6f77 2e69 7465  efCandle.Low.ite
-0001d250: 6d28 295d 2920 3d3d 2030 290d 0a20 2020  m()]) == 0)..   
-0001d260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d270: 2029 3a0d 0a20 2020 2020 2020 2020 2020   ):..           
-0001d280: 2020 2020 2020 2020 2020 2020 2073 6372               scr
-0001d290: 6565 6e44 6963 745b 2250 6174 7465 726e  eenDict["Pattern
-0001d2a0: 225d 203d 2028 0d0a 2020 2020 2020 2020  "] = (..        
-0001d2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d2c0: 2020 2020 7361 7665 645b 305d 0d0a 2020      saved[0]..  
-0001d2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d2e0: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
-0001d2f0: 7254 6578 742e 424f 4c44 0d0a 2020 2020  rText.BOLD..    
-0001d300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d310: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
-0001d320: 6578 742e 5741 524e 0d0a 2020 2020 2020  ext.WARN..      
-0001d330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d340: 2020 2020 2020 2b20 2822 496e 7369 6465        + ("Inside
-0001d350: 2042 6172 2028 2564 2922 2025 2069 290d   Bar (%d)" % i).
-0001d360: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001d370: 2020 2020 2020 2020 2020 2020 202b 2063               + c
-0001d380: 6f6c 6f72 5465 7874 2e45 4e44 0d0a 2020  olorText.END..  
-0001d390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d3a0: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-0001d3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d3c0: 2073 6176 6544 6963 745b 2250 6174 7465   saveDict["Patte
-0001d3d0: 726e 225d 203d 2073 6176 6564 5b31 5d20  rn"] = saved[1] 
-0001d3e0: 2b20 2249 6e73 6964 6520 4261 7220 2825  + "Inside Bar (%
-0001d3f0: 6429 2220 2520 690d 0a20 2020 2020 2020  d)" % i..       
-0001d400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d410: 2072 6574 7572 6e20 690d 0a20 2020 2020   return i..     
-0001d420: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0001d430: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001d440: 2020 2020 2020 7265 7475 726e 2030 0d0a        return 0..
-0001d450: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0001d460: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0001d470: 2020 2069 6620 2244 6f77 6e22 2069 6e20     if "Down" in 
-0001d480: 7361 7665 4469 6374 5b22 5472 656e 6422  saveDict["Trend"
-0001d490: 5d20 616e 6420 280d 0a20 2020 2020 2020  ] and (..       
-0001d4a0: 2020 2020 2020 2020 2020 2020 2022 4265               "Be
-0001d4b0: 6172 2220 696e 2073 6176 6544 6963 745b  ar" in saveDict[
-0001d4c0: 224d 412d 5369 676e 616c 225d 206f 7220  "MA-Signal"] or 
-0001d4d0: 2252 6573 6973 7422 2069 6e20 7361 7665  "Resist" in save
-0001d4e0: 4469 6374 5b22 4d41 2d53 6967 6e61 6c22  Dict["MA-Signal"
-0001d4f0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-0001d500: 2020 2029 3a0d 0a20 2020 2020 2020 2020     ):..         
-0001d510: 2020 2020 2020 2020 2020 2064 6174 6120             data 
-0001d520: 3d20 6f72 6744 6174 612e 6865 6164 2869  = orgData.head(i
-0001d530: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0001d540: 2020 2020 2020 2072 6566 4361 6e64 6c65         refCandle
-0001d550: 203d 2064 6174 612e 7461 696c 2831 290d   = data.tail(1).
-0001d560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001d570: 2020 2020 2069 6620 280d 0a20 2020 2020       if (..     
-0001d580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d590: 2020 2028 6c65 6e28 6461 7461 2e48 6967     (len(data.Hig
-0001d5a0: 685b 6461 7461 2e48 6967 6820 3e20 7265  h[data.High > re
-0001d5b0: 6643 616e 646c 652e 4869 6768 2e69 7465  fCandle.High.ite
-0001d5c0: 6d28 295d 2920 3d3d 2030 290d 0a20 2020  m()]) == 0)..   
-0001d5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d5e0: 2020 2020 2061 6e64 2028 6c65 6e28 6461       and (len(da
-0001d5f0: 7461 2e4c 6f77 5b64 6174 612e 4c6f 7720  ta.Low[data.Low 
-0001d600: 3c20 7265 6643 616e 646c 652e 4c6f 772e  < refCandle.Low.
-0001d610: 6974 656d 2829 5d29 203d 3d20 3029 0d0a  item()]) == 0)..
+000199d0: 2020 2020 2020 2020 636f 6c6f 7254 6578          colorTex
+000199e0: 742e 4752 4545 4e0d 0a20 2020 2020 2020  t.GREEN..       
+000199f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019a10: 2020 2020 202b 2073 7472 2866 696e 616c       + str(final
+00019a20: 2e54 6172 6765 745b 305d 290d 0a20 2020  .Target[0])..   
+00019a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019a50: 2020 2020 2020 2020 202b 2063 6f6c 6f72           + color
+00019a60: 5465 7874 2e45 4e44 2c0d 0a20 2020 2020  Text.END,..     
+00019a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019a90: 2020 2020 2020 2066 2231 3a7b 7269 736b         f"1:{risk
+00019aa0: 5f72 6577 6172 647d 222c 0d0a 2020 2020  _reward}",..    
+00019ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019ad0: 2020 2020 5d0d 0a20 2020 2020 2020 2020      ]..         
+00019ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019af0: 2020 2020 2020 2020 2020 205d 2c0d 0a20             ],.. 
+00019b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019b20: 2020 2063 6f6c 756d 6e73 3d72 6573 756c     columns=resul
+00019b30: 745f 6466 2e63 6f6c 756d 6e73 2c0d 0a20  t_df.columns,.. 
+00019b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019b50: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00019b60: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00019b70: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
+00019b80: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00019b90: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00019ba0: 7869 733d 302c 0d0a 2020 2020 2020 2020  xis=0,..        
+00019bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019bc0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00019bd0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00019be0: 745f 6466 2e72 6573 6574 5f69 6e64 6578  t_df.reset_index
+00019bf0: 2864 726f 703d 5472 7565 2c20 696e 706c  (drop=True, inpl
+00019c00: 6163 653d 5472 7565 290d 0a20 2020 2020  ace=True)..     
+00019c10: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00019c20: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
+00019c30: 6173 2065 3a20 2023 2070 7261 676d 613a  as e:  # pragma:
+00019c40: 206e 6f20 636f 7665 720d 0a20 2020 2020   no cover..     
+00019c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019c60: 2020 2073 656c 662e 6465 6661 756c 745f     self.default_
+00019c70: 6c6f 6767 6572 2e64 6562 7567 2865 2c20  logger.debug(e, 
+00019c80: 6578 635f 696e 666f 3d54 7275 6529 0d0a  exc_info=True)..
+00019c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019ca0: 2020 2020 2020 2020 7061 7373 0d0a 2020          pass..  
+00019cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019cc0: 2020 2320 5468 656e 2075 7064 6174 650d    # Then update.
+00019cd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019ce0: 2020 2020 206c 6173 745f 7369 676e 616c       last_signal
+00019cf0: 5b64 6174 615f 6c69 7374 5b63 6e74 5d5d  [data_list[cnt]]
+00019d00: 203d 205b 6669 6e61 6c5d 0d0a 2020 2020   = [final]..    
+00019d10: 2020 2020 6966 2072 6573 756c 745f 6466      if result_df
+00019d20: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
+00019d30: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00019d40: 745f 6466 2e64 726f 705f 6475 706c 6963  t_df.drop_duplic
+00019d50: 6174 6573 286b 6565 703d 226c 6173 7422  ates(keep="last"
+00019d60: 2c20 696e 706c 6163 653d 5472 7565 290d  , inplace=True).
+00019d70: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00019d80: 756c 745f 6466 2e73 6f72 745f 7661 6c75  ult_df.sort_valu
+00019d90: 6573 2862 793d 2254 696d 6522 2c20 696e  es(by="Time", in
+00019da0: 706c 6163 653d 5472 7565 290d 0a20 2020  place=True)..   
+00019db0: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
+00019dc0: 6c74 5f64 665b 3a3a 2d31 5d0d 0a0d 0a20  lt_df[::-1].... 
+00019dd0: 2020 2023 2050 7265 7072 6f63 6573 7320     # Preprocess 
+00019de0: 7468 6520 6163 7175 6972 6564 2064 6174  the acquired dat
+00019df0: 610d 0a20 2020 2064 6566 2070 7265 7072  a..    def prepr
+00019e00: 6f63 6573 7344 6174 6128 7365 6c66 2c20  ocessData(self, 
+00019e10: 6466 2c20 6461 7973 546f 4c6f 6f6b 6261  df, daysToLookba
+00019e20: 636b 3d4e 6f6e 6529 3a0d 0a20 2020 2020  ck=None):..     
+00019e30: 2020 2061 7373 6572 7420 6973 696e 7374     assert isinst
+00019e40: 616e 6365 2864 662c 2070 642e 4461 7461  ance(df, pd.Data
+00019e50: 4672 616d 6529 0d0a 2020 2020 2020 2020  Frame)..        
+00019e60: 6461 7461 203d 2064 662e 636f 7079 2829  data = df.copy()
+00019e70: 0d0a 2020 2020 2020 2020 7472 793a 0d0a  ..        try:..
+00019e80: 2020 2020 2020 2020 2020 2020 6461 7461              data
+00019e90: 203d 2064 6174 612e 7265 706c 6163 6528   = data.replace(
+00019ea0: 6e70 2e69 6e66 2c20 6e70 2e6e 616e 292e  np.inf, np.nan).
+00019eb0: 7265 706c 6163 6528 2d6e 702e 696e 662c  replace(-np.inf,
+00019ec0: 206e 702e 6e61 6e29 2e64 726f 706e 6128   np.nan).dropna(
+00019ed0: 686f 773d 2261 6c6c 2229 0d0a 2020 2020  how="all")..    
+00019ee0: 2020 2020 2020 2020 2320 7365 6c66 2e64          # self.d
+00019ef0: 6566 6175 6c74 5f6c 6f67 6765 722e 696e  efault_logger.in
+00019f00: 666f 2866 2250 7265 7072 6f63 6573 7369  fo(f"Preprocessi
+00019f10: 6e67 2064 6174 613a 5c6e 7b64 6174 612e  ng data:\n{data.
+00019f20: 6865 6164 2831 297d 5c6e 2229 0d0a 2020  head(1)}\n")..  
+00019f30: 2020 2020 2020 2020 2020 6966 2064 6179            if day
+00019f40: 7354 6f4c 6f6f 6b62 6163 6b20 6973 204e  sToLookback is N
+00019f50: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+00019f60: 2020 2020 2020 6461 7973 546f 4c6f 6f6b        daysToLook
+00019f70: 6261 636b 203d 2073 656c 662e 636f 6e66  back = self.conf
+00019f80: 6967 4d61 6e61 6765 722e 6461 7973 546f  igManager.daysTo
+00019f90: 4c6f 6f6b 6261 636b 0d0a 2020 2020 2020  Lookback..      
+00019fa0: 2020 2020 2020 6966 2073 656c 662e 636f        if self.co
+00019fb0: 6e66 6967 4d61 6e61 6765 722e 7573 6545  nfigManager.useE
+00019fc0: 4d41 3a0d 0a20 2020 2020 2020 2020 2020  MA:..           
+00019fd0: 2020 2020 2073 6d61 203d 2070 6b74 616c       sma = pktal
+00019fe0: 6962 2e45 4d41 2864 6174 615b 2243 6c6f  ib.EMA(data["Clo
+00019ff0: 7365 225d 2c20 7469 6d65 7065 7269 6f64  se"], timeperiod
+0001a000: 3d35 3029 0d0a 2020 2020 2020 2020 2020  =50)..          
+0001a010: 2020 2020 2020 6c6d 6120 3d20 706b 7461        lma = pkta
+0001a020: 6c69 622e 454d 4128 6461 7461 5b22 436c  lib.EMA(data["Cl
+0001a030: 6f73 6522 5d2c 2074 696d 6570 6572 696f  ose"], timeperio
+0001a040: 643d 3230 3029 0d0a 2020 2020 2020 2020  d=200)..        
+0001a050: 2020 2020 2020 2020 7373 6d61 203d 2070          ssma = p
+0001a060: 6b74 616c 6962 2e45 4d41 2864 6174 615b  ktalib.EMA(data[
+0001a070: 2243 6c6f 7365 225d 2c20 7469 6d65 7065  "Close"], timepe
+0001a080: 7269 6f64 3d39 290d 0a20 2020 2020 2020  riod=9)..       
+0001a090: 2020 2020 2020 2020 2064 6174 612e 696e           data.in
+0001a0a0: 7365 7274 286c 656e 2864 6174 612e 636f  sert(len(data.co
+0001a0b0: 6c75 6d6e 7329 2c20 2253 4d41 222c 2073  lumns), "SMA", s
+0001a0c0: 6d61 290d 0a20 2020 2020 2020 2020 2020  ma)..           
+0001a0d0: 2020 2020 2064 6174 612e 696e 7365 7274       data.insert
+0001a0e0: 286c 656e 2864 6174 612e 636f 6c75 6d6e  (len(data.column
+0001a0f0: 7329 2c20 224c 4d41 222c 206c 6d61 290d  s), "LMA", lma).
+0001a100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a110: 2064 6174 612e 696e 7365 7274 286c 656e   data.insert(len
+0001a120: 2864 6174 612e 636f 6c75 6d6e 7329 2c20  (data.columns), 
+0001a130: 2253 534d 4122 2c20 7373 6d61 290d 0a20  "SSMA", ssma).. 
+0001a140: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0001a150: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001a160: 2020 736d 6120 3d20 706b 7461 6c69 622e    sma = pktalib.
+0001a170: 534d 4128 6461 7461 5b22 436c 6f73 6522  SMA(data["Close"
+0001a180: 5d2c 2074 696d 6570 6572 696f 643d 3530  ], timeperiod=50
+0001a190: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0001a1a0: 2020 206c 6d61 203d 2070 6b74 616c 6962     lma = pktalib
+0001a1b0: 2e53 4d41 2864 6174 615b 2243 6c6f 7365  .SMA(data["Close
+0001a1c0: 225d 2c20 7469 6d65 7065 7269 6f64 3d32  "], timeperiod=2
+0001a1d0: 3030 290d 0a20 2020 2020 2020 2020 2020  00)..           
+0001a1e0: 2020 2020 2073 736d 6120 3d20 706b 7461       ssma = pkta
+0001a1f0: 6c69 622e 534d 4128 6461 7461 5b22 436c  lib.SMA(data["Cl
+0001a200: 6f73 6522 5d2c 2074 696d 6570 6572 696f  ose"], timeperio
+0001a210: 643d 3929 0d0a 2020 2020 2020 2020 2020  d=9)..          
+0001a220: 2020 2020 2020 6461 7461 2e69 6e73 6572        data.inser
+0001a230: 7428 6c65 6e28 6461 7461 2e63 6f6c 756d  t(len(data.colum
+0001a240: 6e73 292c 2022 534d 4122 2c20 736d 6129  ns), "SMA", sma)
+0001a250: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001a260: 2020 6461 7461 2e69 6e73 6572 7428 6c65    data.insert(le
+0001a270: 6e28 6461 7461 2e63 6f6c 756d 6e73 292c  n(data.columns),
+0001a280: 2022 4c4d 4122 2c20 6c6d 6129 0d0a 2020   "LMA", lma)..  
+0001a290: 2020 2020 2020 2020 2020 2020 2020 6461                da
+0001a2a0: 7461 2e69 6e73 6572 7428 6c65 6e28 6461  ta.insert(len(da
+0001a2b0: 7461 2e63 6f6c 756d 6e73 292c 2022 5353  ta.columns), "SS
+0001a2c0: 4d41 222c 2073 736d 6129 0d0a 2020 2020  MA", ssma)..    
+0001a2d0: 2020 2020 2020 2020 766f 6c20 3d20 706b          vol = pk
+0001a2e0: 7461 6c69 622e 534d 4128 6461 7461 5b22  talib.SMA(data["
+0001a2f0: 566f 6c75 6d65 225d 2c20 7469 6d65 7065  Volume"], timepe
+0001a300: 7269 6f64 3d32 3029 0d0a 2020 2020 2020  riod=20)..      
+0001a310: 2020 2020 2020 7273 6920 3d20 706b 7461        rsi = pkta
+0001a320: 6c69 622e 5253 4928 6461 7461 5b22 436c  lib.RSI(data["Cl
+0001a330: 6f73 6522 5d2c 2074 696d 6570 6572 696f  ose"], timeperio
+0001a340: 643d 3134 290d 0a20 2020 2020 2020 2020  d=14)..         
+0001a350: 2020 2064 6174 612e 696e 7365 7274 286c     data.insert(l
+0001a360: 656e 2864 6174 612e 636f 6c75 6d6e 7329  en(data.columns)
+0001a370: 2c20 2256 6f6c 4d41 222c 2076 6f6c 290d  , "VolMA", vol).
+0001a380: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+0001a390: 612e 696e 7365 7274 286c 656e 2864 6174  a.insert(len(dat
+0001a3a0: 612e 636f 6c75 6d6e 7329 2c20 2252 5349  a.columns), "RSI
+0001a3b0: 222c 2072 7369 290d 0a20 2020 2020 2020  ", rsi)..       
+0001a3c0: 2020 2020 2063 6369 203d 2070 6b74 616c       cci = pktal
+0001a3d0: 6962 2e43 4349 2864 6174 615b 2248 6967  ib.CCI(data["Hig
+0001a3e0: 6822 5d2c 2064 6174 615b 224c 6f77 225d  h"], data["Low"]
+0001a3f0: 2c20 6461 7461 5b22 436c 6f73 6522 5d2c  , data["Close"],
+0001a400: 2074 696d 6570 6572 696f 643d 3134 290d   timeperiod=14).
+0001a410: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+0001a420: 612e 696e 7365 7274 286c 656e 2864 6174  a.insert(len(dat
+0001a430: 612e 636f 6c75 6d6e 7329 2c20 2243 4349  a.columns), "CCI
+0001a440: 222c 2063 6369 290d 0a20 2020 2020 2020  ", cci)..       
+0001a450: 2020 2020 2074 7279 3a0d 0a20 2020 2020       try:..     
+0001a460: 2020 2020 2020 2020 2020 2066 6173 746b             fastk
+0001a470: 2c20 6661 7374 6420 3d20 706b 7461 6c69  , fastd = pktali
+0001a480: 622e 5354 4f43 4852 5349 280d 0a20 2020  b.STOCHRSI(..   
+0001a490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a4a0: 2064 6174 615b 2243 6c6f 7365 225d 2c20   data["Close"], 
+0001a4b0: 7469 6d65 7065 7269 6f64 3d31 342c 2066  timeperiod=14, f
+0001a4c0: 6173 746b 5f70 6572 696f 643d 352c 2066  astk_period=5, f
+0001a4d0: 6173 7464 5f70 6572 696f 643d 332c 2066  astd_period=3, f
+0001a4e0: 6173 7464 5f6d 6174 7970 653d 300d 0a20  astd_matype=0.. 
+0001a4f0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+0001a500: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001a510: 2020 6461 7461 2e69 6e73 6572 7428 6c65    data.insert(le
+0001a520: 6e28 6461 7461 2e63 6f6c 756d 6e73 292c  n(data.columns),
+0001a530: 2022 4641 5354 4b22 2c20 6661 7374 6b29   "FASTK", fastk)
+0001a540: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001a550: 2020 6461 7461 2e69 6e73 6572 7428 6c65    data.insert(le
+0001a560: 6e28 6461 7461 2e63 6f6c 756d 6e73 292c  n(data.columns),
+0001a570: 2022 4641 5354 4422 2c20 6661 7374 6429   "FASTD", fastd)
+0001a580: 0d0a 2020 2020 2020 2020 2020 2020 6578  ..            ex
+0001a590: 6365 7074 2045 7863 6570 7469 6f6e 2061  cept Exception a
+0001a5a0: 7320 653a 0d0a 2020 2020 2020 2020 2020  s e:..          
+0001a5b0: 2020 2020 2020 7365 6c66 2e64 6566 6175        self.defau
+0001a5c0: 6c74 5f6c 6f67 6765 722e 6465 6275 6728  lt_logger.debug(
+0001a5d0: 652c 2065 7863 5f69 6e66 6f3d 5472 7565  e, exc_info=True
+0001a5e0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0001a5f0: 2020 2070 6173 730d 0a20 2020 2020 2020     pass..       
+0001a600: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+0001a610: 6e20 6173 2065 3a0d 0a20 2020 2020 2020  n as e:..       
+0001a620: 2020 2020 2020 2020 2073 656c 662e 6465           self.de
+0001a630: 6661 756c 745f 6c6f 6767 6572 2e64 6562  fault_logger.deb
+0001a640: 7567 2865 2c20 6578 635f 696e 666f 3d54  ug(e, exc_info=T
+0001a650: 7275 6529 0d0a 2020 2020 2020 2020 2020  rue)..          
+0001a660: 2020 2020 2020 7061 7373 0d0a 2020 2020        pass..    
+0001a670: 2020 2020 6461 7461 203d 2064 6174 615b      data = data[
+0001a680: 3a3a 2d31 5d20 2023 2052 6576 6572 7365  ::-1]  # Reverse
+0001a690: 2074 6865 2064 6174 6166 7261 6d65 0d0a   the dataframe..
+0001a6a0: 2020 2020 2020 2020 2320 6461 7461 203d          # data =
+0001a6b0: 2064 6174 612e 6669 6c6c 6e61 2830 290d   data.fillna(0).
+0001a6c0: 0a20 2020 2020 2020 2023 2064 6174 6120  .        # data 
+0001a6d0: 3d20 6461 7461 2e72 6570 6c61 6365 285b  = data.replace([
+0001a6e0: 6e70 2e69 6e66 2c20 2d6e 702e 696e 665d  np.inf, -np.inf]
+0001a6f0: 2c20 3029 0d0a 2020 2020 2020 2020 6675  , 0)..        fu
+0001a700: 6c6c 4461 7461 203d 2064 6174 610d 0a20  llData = data.. 
+0001a710: 2020 2020 2020 2074 7269 6d6d 6564 4461         trimmedDa
+0001a720: 7461 203d 2064 6174 612e 6865 6164 2864  ta = data.head(d
+0001a730: 6179 7354 6f4c 6f6f 6b62 6163 6b29 0d0a  aysToLookback)..
+0001a740: 2020 2020 2020 2020 7265 7475 726e 2028          return (
+0001a750: 6675 6c6c 4461 7461 2c20 7472 696d 6d65  fullData, trimme
+0001a760: 6444 6174 6129 0d0a 0d0a 2020 2020 2320  dData)....    # 
+0001a770: 5661 6c69 6461 7465 2069 6620 7468 6520  Validate if the 
+0001a780: 7374 6f63 6b20 6973 2062 756c 6c69 7368  stock is bullish
+0001a790: 2069 6e20 7468 6520 7368 6f72 7420 7465   in the short te
+0001a7a0: 726d 0d0a 2020 2020 6465 6620 7661 6c69  rm..    def vali
+0001a7b0: 6461 7465 3135 4d69 6e75 7465 5072 6963  date15MinutePric
+0001a7c0: 6556 6f6c 756d 6542 7265 616b 6f75 7428  eVolumeBreakout(
+0001a7d0: 7365 6c66 2c20 6466 293a 0d0a 2020 2020  self, df):..    
+0001a7e0: 2020 2020 6966 2064 6620 6973 204e 6f6e      if df is Non
+0001a7f0: 6520 6f72 206c 656e 2864 6629 203d 3d20  e or len(df) == 
+0001a800: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
+0001a810: 7265 7475 726e 2046 616c 7365 0d0a 2020  return False..  
+0001a820: 2020 2020 2020 2320 6874 7470 733a 2f2f        # https://
+0001a830: 6368 6172 7469 6e6b 2e63 6f6d 2f73 6372  chartink.com/scr
+0001a840: 6565 6e65 722f 3135 2d6d 696e 2d70 7269  eener/15-min-pri
+0001a850: 6365 2d76 6f6c 756d 652d 6272 6561 6b6f  ce-volume-breako
+0001a860: 7574 0d0a 2020 2020 2020 2020 6461 7461  ut..        data
+0001a870: 203d 2064 662e 636f 7079 2829 0d0a 2020   = df.copy()..  
+0001a880: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
+0001a890: 612e 6669 6c6c 6e61 2830 290d 0a20 2020  a.fillna(0)..   
+0001a8a0: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
+0001a8b0: 2e72 6570 6c61 6365 285b 6e70 2e69 6e66  .replace([np.inf
+0001a8c0: 2c20 2d6e 702e 696e 665d 2c20 3029 0d0a  , -np.inf], 0)..
+0001a8d0: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
+0001a8e0: 6174 615b 3a3a 2d31 5d20 2023 2052 6576  ata[::-1]  # Rev
+0001a8f0: 6572 7365 2074 6865 2064 6174 6166 7261  erse the datafra
+0001a900: 6d65 2073 6f20 7468 6174 2069 7473 2074  me so that its t
+0001a910: 6865 206f 6c64 6573 7420 6461 7465 2066  he oldest date f
+0001a920: 6972 7374 0d0a 2020 2020 2020 2020 6461  irst..        da
+0001a930: 7461 5b22 534d 4132 3022 5d20 3d20 706b  ta["SMA20"] = pk
+0001a940: 7461 6c69 622e 534d 4128 6461 7461 5b22  talib.SMA(data["
+0001a950: 436c 6f73 6522 5d2c 2032 3029 0d0a 2020  Close"], 20)..  
+0001a960: 2020 2020 2020 6461 7461 5b22 534d 4132        data["SMA2
+0001a970: 3056 225d 203d 2070 6b74 616c 6962 2e53  0V"] = pktalib.S
+0001a980: 4d41 2864 6174 615b 2256 6f6c 756d 6522  MA(data["Volume"
+0001a990: 5d2c 2032 3029 0d0a 2020 2020 2020 2020  ], 20)..        
+0001a9a0: 6461 7461 203d 2064 6174 615b 0d0a 2020  data = data[..  
+0001a9b0: 2020 2020 2020 2020 2020 3a3a 2d31 0d0a            ::-1..
+0001a9c0: 2020 2020 2020 2020 5d20 2023 2052 6576          ]  # Rev
+0001a9d0: 6572 7365 2074 6865 2064 6174 6166 7261  erse the datafra
+0001a9e0: 6d65 2073 6f20 7468 6174 2069 7427 7320  me so that it's 
+0001a9f0: 7468 6520 6d6f 7374 2072 6563 656e 7420  the most recent 
+0001aa00: 6461 7465 2066 6972 7374 0d0a 2020 2020  date first..    
+0001aa10: 2020 2020 7265 6365 6e74 203d 2064 6174      recent = dat
+0001aa20: 612e 6865 6164 2833 290d 0a20 2020 2020  a.head(3)..     
+0001aa30: 2020 2069 6620 6c65 6e28 7265 6365 6e74     if len(recent
+0001aa40: 2920 3c20 333a 0d0a 2020 2020 2020 2020  ) < 3:..        
+0001aa50: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+0001aa60: 0d0a 2020 2020 2020 2020 636f 6e64 3120  ..        cond1 
+0001aa70: 3d20 7265 6365 6e74 5b22 436c 6f73 6522  = recent["Close"
+0001aa80: 5d2e 696c 6f63 5b30 5d20 3e20 7265 6365  ].iloc[0] > rece
+0001aa90: 6e74 5b22 436c 6f73 6522 5d2e 696c 6f63  nt["Close"].iloc
+0001aaa0: 5b31 5d0d 0a20 2020 2020 2020 2063 6f6e  [1]..        con
+0001aab0: 6432 203d 2063 6f6e 6431 2061 6e64 2028  d2 = cond1 and (
+0001aac0: 7265 6365 6e74 5b22 436c 6f73 6522 5d2e  recent["Close"].
+0001aad0: 696c 6f63 5b30 5d20 3e20 7265 6365 6e74  iloc[0] > recent
+0001aae0: 5b22 534d 4132 3022 5d2e 696c 6f63 5b30  ["SMA20"].iloc[0
+0001aaf0: 5d29 0d0a 2020 2020 2020 2020 636f 6e64  ])..        cond
+0001ab00: 3320 3d20 636f 6e64 3220 616e 6420 2872  3 = cond2 and (r
+0001ab10: 6563 656e 745b 2243 6c6f 7365 225d 2e69  ecent["Close"].i
+0001ab20: 6c6f 635b 315d 203e 2072 6563 656e 745b  loc[1] > recent[
+0001ab30: 2248 6967 6822 5d2e 696c 6f63 5b32 5d29  "High"].iloc[2])
+0001ab40: 0d0a 2020 2020 2020 2020 636f 6e64 3420  ..        cond4 
+0001ab50: 3d20 636f 6e64 3320 616e 6420 2872 6563  = cond3 and (rec
+0001ab60: 656e 745b 2256 6f6c 756d 6522 5d2e 696c  ent["Volume"].il
+0001ab70: 6f63 5b30 5d20 3e20 7265 6365 6e74 5b22  oc[0] > recent["
+0001ab80: 534d 4132 3056 225d 2e69 6c6f 635b 305d  SMA20V"].iloc[0]
+0001ab90: 290d 0a20 2020 2020 2020 2063 6f6e 6435  )..        cond5
+0001aba0: 203d 2063 6f6e 6434 2061 6e64 2028 7265   = cond4 and (re
+0001abb0: 6365 6e74 5b22 566f 6c75 6d65 225d 2e69  cent["Volume"].i
+0001abc0: 6c6f 635b 315d 203e 2072 6563 656e 745b  loc[1] > recent[
+0001abd0: 2253 4d41 3230 5622 5d2e 696c 6f63 5b30  "SMA20V"].iloc[0
+0001abe0: 5d29 0d0a 2020 2020 2020 2020 7265 7475  ])..        retu
+0001abf0: 726e 2063 6f6e 6435 0d0a 0d0a 2020 2020  rn cond5....    
+0001ac00: 6465 6620 7661 6c69 6461 7465 4275 6c6c  def validateBull
+0001ac10: 6973 6846 6f72 546f 6d6f 7272 6f77 2873  ishForTomorrow(s
+0001ac20: 656c 662c 2064 6629 3a0d 0a20 2020 2020  elf, df):..     
+0001ac30: 2020 2069 6620 6466 2069 7320 4e6f 6e65     if df is None
+0001ac40: 206f 7220 6c65 6e28 6466 2920 3d3d 2030   or len(df) == 0
+0001ac50: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+0001ac60: 6574 7572 6e20 4661 6c73 650d 0a20 2020  eturn False..   
+0001ac70: 2020 2020 2064 6174 6120 3d20 6466 2e63       data = df.c
+0001ac80: 6f70 7928 290d 0a20 2020 2020 2020 2023  opy()..        #
+0001ac90: 2068 7474 7073 3a2f 2f63 6861 7274 696e   https://chartin
+0001aca0: 6b2e 636f 6d2f 7363 7265 656e 6572 2f62  k.com/screener/b
+0001acb0: 756c 6c69 7368 2d66 6f72 2d74 6f6d 6f72  ullish-for-tomor
+0001acc0: 726f 770d 0a20 2020 2020 2020 2064 6174  row..        dat
+0001acd0: 6120 3d20 6461 7461 2e66 696c 6c6e 6128  a = data.fillna(
+0001ace0: 3029 0d0a 2020 2020 2020 2020 6461 7461  0)..        data
+0001acf0: 203d 2064 6174 612e 7265 706c 6163 6528   = data.replace(
+0001ad00: 5b6e 702e 696e 662c 202d 6e70 2e69 6e66  [np.inf, -np.inf
+0001ad10: 5d2c 2030 290d 0a20 2020 2020 2020 2064  ], 0)..        d
+0001ad20: 6174 6120 3d20 6461 7461 5b3a 3a2d 315d  ata = data[::-1]
+0001ad30: 2020 2320 5265 7665 7273 6520 7468 6520    # Reverse the 
+0001ad40: 6461 7461 6672 616d 6520 736f 2074 6861  dataframe so tha
+0001ad50: 7420 6974 7320 7468 6520 6f6c 6465 7374  t its the oldest
+0001ad60: 2064 6174 6520 6669 7273 740d 0a20 2020   date first..   
+0001ad70: 2020 2020 206d 6163 644c 696e 6520 3d20       macdLine = 
+0001ad80: 706b 7461 6c69 622e 4d41 4344 2864 6174  pktalib.MACD(dat
+0001ad90: 615b 2243 6c6f 7365 225d 2c20 3132 2c20  a["Close"], 12, 
+0001ada0: 3236 2c20 3929 5b30 5d2e 7461 696c 2833  26, 9)[0].tail(3
+0001adb0: 290d 0a20 2020 2020 2020 206d 6163 6453  )..        macdS
+0001adc0: 6967 6e61 6c20 3d20 706b 7461 6c69 622e  ignal = pktalib.
+0001add0: 4d41 4344 2864 6174 615b 2243 6c6f 7365  MACD(data["Close
+0001ade0: 225d 2c20 3132 2c20 3236 2c20 3929 5b31  "], 12, 26, 9)[1
+0001adf0: 5d2e 7461 696c 2833 290d 0a20 2020 2020  ].tail(3)..     
+0001ae00: 2020 206d 6163 6448 6973 7420 3d20 706b     macdHist = pk
+0001ae10: 7461 6c69 622e 4d41 4344 2864 6174 615b  talib.MACD(data[
+0001ae20: 2243 6c6f 7365 225d 2c20 3132 2c20 3236  "Close"], 12, 26
+0001ae30: 2c20 3929 5b32 5d2e 7461 696c 2833 290d  , 9)[2].tail(3).
+0001ae40: 0a0d 0a20 2020 2020 2020 2072 6574 7572  ...        retur
+0001ae50: 6e20 280d 0a20 2020 2020 2020 2020 2020  n (..           
+0001ae60: 2028 6d61 6364 4869 7374 2e69 6c6f 635b   (macdHist.iloc[
+0001ae70: 3a31 5d2e 696c 6f63 5b30 5d20 3c20 6d61  :1].iloc[0] < ma
+0001ae80: 6364 4869 7374 2e69 6c6f 635b 3a32 5d2e  cdHist.iloc[:2].
+0001ae90: 696c 6f63 5b31 5d29 0d0a 2020 2020 2020  iloc[1])..      
+0001aea0: 2020 2020 2020 616e 6420 286d 6163 6448        and (macdH
+0001aeb0: 6973 742e 696c 6f63 5b3a 335d 2e69 6c6f  ist.iloc[:3].ilo
+0001aec0: 635b 325d 203e 206d 6163 6448 6973 742e  c[2] > macdHist.
+0001aed0: 696c 6f63 5b3a 325d 2e69 6c6f 635b 315d  iloc[:2].iloc[1]
+0001aee0: 290d 0a20 2020 2020 2020 2020 2020 2061  )..            a
+0001aef0: 6e64 2028 0d0a 2020 2020 2020 2020 2020  nd (..          
+0001af00: 2020 2020 2020 286d 6163 644c 696e 652e        (macdLine.
+0001af10: 696c 6f63 5b3a 335d 2e69 6c6f 635b 325d  iloc[:3].iloc[2]
+0001af20: 202d 206d 6163 6453 6967 6e61 6c2e 696c   - macdSignal.il
+0001af30: 6f63 5b3a 335d 2e69 6c6f 635b 325d 290d  oc[:3].iloc[2]).
+0001af40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001af50: 202d 2028 6d61 6364 4c69 6e65 2e69 6c6f   - (macdLine.ilo
+0001af60: 635b 3a32 5d2e 696c 6f63 5b31 5d20 2d20  c[:2].iloc[1] - 
+0001af70: 6d61 6364 5369 676e 616c 2e69 6c6f 635b  macdSignal.iloc[
+0001af80: 3a32 5d2e 696c 6f63 5b31 5d29 0d0a 2020  :2].iloc[1])..  
+0001af90: 2020 2020 2020 2020 2020 2020 2020 3e3d                >=
+0001afa0: 2030 2e34 0d0a 2020 2020 2020 2020 2020   0.4..          
+0001afb0: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
+0001afc0: 2061 6e64 2028 0d0a 2020 2020 2020 2020   and (..        
+0001afd0: 2020 2020 2020 2020 286d 6163 644c 696e          (macdLin
+0001afe0: 652e 696c 6f63 5b3a 325d 2e69 6c6f 635b  e.iloc[:2].iloc[
+0001aff0: 315d 202d 206d 6163 6453 6967 6e61 6c2e  1] - macdSignal.
+0001b000: 696c 6f63 5b3a 325d 2e69 6c6f 635b 315d  iloc[:2].iloc[1]
+0001b010: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0001b020: 2020 202d 2028 6d61 6364 4c69 6e65 2e69     - (macdLine.i
+0001b030: 6c6f 635b 3a31 5d2e 696c 6f63 5b30 5d20  loc[:1].iloc[0] 
+0001b040: 2d20 6d61 6364 5369 676e 616c 2e69 6c6f  - macdSignal.ilo
+0001b050: 635b 3a31 5d2e 696c 6f63 5b30 5d29 0d0a  c[:1].iloc[0])..
+0001b060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b070: 3c3d 2030 2e32 0d0a 2020 2020 2020 2020  <= 0.2..        
+0001b080: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
+0001b090: 2020 2061 6e64 2028 6d61 6364 4c69 6e65     and (macdLine
+0001b0a0: 2e69 6c6f 635b 3a33 5d2e 696c 6f63 5b32  .iloc[:3].iloc[2
+0001b0b0: 5d20 3e20 6d61 6364 5369 676e 616c 2e69  ] > macdSignal.i
+0001b0c0: 6c6f 635b 3a33 5d2e 696c 6f63 5b32 5d29  loc[:3].iloc[2])
+0001b0d0: 0d0a 2020 2020 2020 2020 2020 2020 616e  ..            an
+0001b0e0: 6420 280d 0a20 2020 2020 2020 2020 2020  d (..           
+0001b0f0: 2020 2020 2028 6d61 6364 4c69 6e65 2e69       (macdLine.i
+0001b100: 6c6f 635b 3a33 5d2e 696c 6f63 5b32 5d20  loc[:3].iloc[2] 
+0001b110: 2d20 6d61 6364 5369 676e 616c 2e69 6c6f  - macdSignal.ilo
+0001b120: 635b 3a33 5d2e 696c 6f63 5b32 5d29 0d0a  c[:3].iloc[2])..
+0001b130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b140: 2d20 286d 6163 644c 696e 652e 696c 6f63  - (macdLine.iloc
+0001b150: 5b3a 325d 2e69 6c6f 635b 315d 202d 206d  [:2].iloc[1] - m
+0001b160: 6163 6453 6967 6e61 6c2e 696c 6f63 5b3a  acdSignal.iloc[:
+0001b170: 325d 2e69 6c6f 635b 315d 290d 0a20 2020  2].iloc[1])..   
+0001b180: 2020 2020 2020 2020 2020 2020 203c 2031               < 1
+0001b190: 0d0a 2020 2020 2020 2020 2020 2020 290d  ..            ).
+0001b1a0: 0a20 2020 2020 2020 2029 0d0a 0d0a 2020  .        )....  
+0001b1b0: 2020 2340 6d65 6173 7572 655f 7469 6d65    #@measure_time
+0001b1c0: 0d0a 2020 2020 2320 7661 6c69 6461 7465  ..    # validate
+0001b1d0: 2069 6620 4343 4920 6973 2077 6974 6869   if CCI is withi
+0001b1e0: 6e20 6769 7665 6e20 7261 6e67 650d 0a20  n given range.. 
+0001b1f0: 2020 2064 6566 2076 616c 6964 6174 6543     def validateC
+0001b200: 4349 2873 656c 662c 2064 662c 2073 6372  CI(self, df, scr
+0001b210: 6565 6e44 6963 742c 2073 6176 6544 6963  eenDict, saveDic
+0001b220: 742c 206d 696e 4343 492c 206d 6178 4343  t, minCCI, maxCC
+0001b230: 4929 3a0d 0a20 2020 2020 2020 2069 6620  I):..        if 
+0001b240: 6466 2069 7320 4e6f 6e65 206f 7220 6c65  df is None or le
+0001b250: 6e28 6466 2920 3d3d 2030 3a0d 0a20 2020  n(df) == 0:..   
+0001b260: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0001b270: 4661 6c73 650d 0a20 2020 2020 2020 2064  False..        d
+0001b280: 6174 6120 3d20 6466 2e63 6f70 7928 290d  ata = df.copy().
+0001b290: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
+0001b2a0: 6461 7461 2e66 696c 6c6e 6128 3029 0d0a  data.fillna(0)..
+0001b2b0: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
+0001b2c0: 6174 612e 7265 706c 6163 6528 5b6e 702e  ata.replace([np.
+0001b2d0: 696e 662c 202d 6e70 2e69 6e66 5d2c 2030  inf, -np.inf], 0
+0001b2e0: 290d 0a20 2020 2020 2020 2063 6369 203d  )..        cci =
+0001b2f0: 2069 6e74 2864 6174 612e 6865 6164 2831   int(data.head(1
+0001b300: 295b 2243 4349 225d 2e69 6c6f 635b 305d  )["CCI"].iloc[0]
+0001b310: 290d 0a20 2020 2020 2020 2073 6176 6544  )..        saveD
+0001b320: 6963 745b 2243 4349 225d 203d 2063 6369  ict["CCI"] = cci
+0001b330: 0d0a 2020 2020 2020 2020 6966 2028 6363  ..        if (cc
+0001b340: 6920 3e3d 206d 696e 4343 4920 616e 6420  i >= minCCI and 
+0001b350: 6363 6920 3c3d 206d 6178 4343 4929 3a0d  cci <= maxCCI):.
+0001b360: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0001b370: 2822 5570 2220 696e 2073 6176 6544 6963  ("Up" in saveDic
+0001b380: 745b 2254 7265 6e64 225d 293a 0d0a 2020  t["Trend"]):..  
+0001b390: 2020 2020 2020 2020 2020 2020 2020 7363                sc
+0001b3a0: 7265 656e 4469 6374 5b22 4343 4922 5d20  reenDict["CCI"] 
+0001b3b0: 3d20 280d 0a20 2020 2020 2020 2020 2020  = (..           
+0001b3c0: 2020 2020 2020 2020 2028 636f 6c6f 7254           (colorT
+0001b3d0: 6578 742e 424f 4c44 2069 6620 2822 5374  ext.BOLD if ("St
+0001b3e0: 726f 6e67 2220 696e 2073 6176 6544 6963  rong" in saveDic
+0001b3f0: 745b 2254 7265 6e64 225d 2920 656c 7365  t["Trend"]) else
+0001b400: 2022 2229 202b 2063 6f6c 6f72 5465 7874   "") + colorText
+0001b410: 2e47 5245 454e 202b 2073 7472 2863 6369  .GREEN + str(cci
+0001b420: 2920 2b20 636f 6c6f 7254 6578 742e 454e  ) + colorText.EN
+0001b430: 440d 0a20 2020 2020 2020 2020 2020 2020  D..             
+0001b440: 2020 2029 0d0a 2020 2020 2020 2020 2020     )..          
+0001b450: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+0001b460: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
+0001b470: 6963 745b 2243 4349 225d 203d 2028 0d0a  ict["CCI"] = (..
+0001b480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b490: 2020 2020 2863 6f6c 6f72 5465 7874 2e42      (colorText.B
+0001b4a0: 4f4c 4420 6966 2028 2253 7472 6f6e 6722  OLD if ("Strong"
+0001b4b0: 2069 6e20 7361 7665 4469 6374 5b22 5472   in saveDict["Tr
+0001b4c0: 656e 6422 5d29 2065 6c73 6520 2222 2920  end"]) else "") 
+0001b4d0: 2b20 636f 6c6f 7254 6578 742e 4641 494c  + colorText.FAIL
+0001b4e0: 202b 2073 7472 2863 6369 2920 2b20 636f   + str(cci) + co
+0001b4f0: 6c6f 7254 6578 742e 454e 440d 0a20 2020  lorText.END..   
+0001b500: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
+0001b510: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0001b520: 726e 2054 7275 650d 0a20 2020 2020 2020  rn True..       
+0001b530: 2073 6372 6565 6e44 6963 745b 2243 4349   screenDict["CCI
+0001b540: 225d 203d 2063 6f6c 6f72 5465 7874 2e42  "] = colorText.B
+0001b550: 4f4c 4420 2b20 636f 6c6f 7254 6578 742e  OLD + colorText.
+0001b560: 4641 494c 202b 2073 7472 2863 6369 2920  FAIL + str(cci) 
+0001b570: 2b20 636f 6c6f 7254 6578 742e 454e 440d  + colorText.END.
+0001b580: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0001b590: 4661 6c73 650d 0a0d 0a20 2020 2023 2046  False....    # F
+0001b5a0: 696e 6420 436f 6e66 6c75 6365 6e63 650d  ind Conflucence.
+0001b5b0: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+0001b5c0: 6543 6f6e 666c 7565 6e63 6528 7365 6c66  eConfluence(self
+0001b5d0: 2c20 7374 6f63 6b2c 2064 662c 2073 6372  , stock, df, scr
+0001b5e0: 6565 6e44 6963 742c 2073 6176 6544 6963  eenDict, saveDic
+0001b5f0: 742c 2070 6572 6365 6e74 6167 653d 302e  t, percentage=0.
+0001b600: 312c 636f 6e66 4669 6c74 6572 3d33 293a  1,confFilter=3):
+0001b610: 0d0a 2020 2020 2020 2020 6966 2064 6620  ..        if df 
+0001b620: 6973 204e 6f6e 6520 6f72 206c 656e 2864  is None or len(d
+0001b630: 6629 203d 3d20 303a 0d0a 2020 2020 2020  f) == 0:..      
+0001b640: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+0001b650: 7365 0d0a 2020 2020 2020 2020 6461 7461  se..        data
+0001b660: 203d 2064 662e 636f 7079 2829 0d0a 2020   = df.copy()..  
+0001b670: 2020 2020 2020 7265 6365 6e74 203d 2064        recent = d
+0001b680: 6174 612e 6865 6164 2832 290d 0a20 2020  ata.head(2)..   
+0001b690: 2020 2020 2069 6620 6c65 6e28 7265 6365       if len(rece
+0001b6a0: 6e74 2920 3c20 323a 0d0a 2020 2020 2020  nt) < 2:..      
+0001b6b0: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+0001b6c0: 7365 0d0a 2020 2020 2020 2020 6973 3530  se..        is50
+0001b6d0: 444d 4155 7054 7265 6e64 203d 2028 7265  DMAUpTrend = (re
+0001b6e0: 6365 6e74 5b22 534d 4122 5d2e 696c 6f63  cent["SMA"].iloc
+0001b6f0: 5b30 5d20 3e20 7265 6365 6e74 5b22 534d  [0] > recent["SM
+0001b700: 4122 5d2e 696c 6f63 5b31 5d29 0d0a 2020  A"].iloc[1])..  
+0001b710: 2020 2020 2020 6973 3530 444d 4144 6f77        is50DMADow
+0001b720: 6e54 7265 6e64 203d 2028 7265 6365 6e74  nTrend = (recent
+0001b730: 5b22 534d 4122 5d2e 696c 6f63 5b30 5d20  ["SMA"].iloc[0] 
+0001b740: 3c20 7265 6365 6e74 5b22 534d 4122 5d2e  < recent["SMA"].
+0001b750: 696c 6f63 5b31 5d29 0d0a 2020 2020 2020  iloc[1])..      
+0001b760: 2020 6973 476f 6c64 656e 4372 6f73 734f    isGoldenCrossO
+0001b770: 7665 7220 3d20 2872 6563 656e 745b 2253  ver = (recent["S
+0001b780: 4d41 225d 2e69 6c6f 635b 305d 203e 3d20  MA"].iloc[0] >= 
+0001b790: 7265 6365 6e74 5b22 4c4d 4122 5d2e 696c  recent["LMA"].il
+0001b7a0: 6f63 5b30 5d29 2061 6e64 205c 0d0a 2020  oc[0]) and \..  
+0001b7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b7c0: 2020 2020 2020 2020 2020 2872 6563 656e            (recen
+0001b7d0: 745b 2253 4d41 225d 2e69 6c6f 635b 315d  t["SMA"].iloc[1]
+0001b7e0: 203c 3d20 7265 6365 6e74 5b22 4c4d 4122   <= recent["LMA"
+0001b7f0: 5d2e 696c 6f63 5b31 5d29 0d0a 2020 2020  ].iloc[1])..    
+0001b800: 2020 2020 6973 4465 6164 4372 6f73 734f      isDeadCrossO
+0001b810: 7665 7220 3d20 2872 6563 656e 745b 2253  ver = (recent["S
+0001b820: 4d41 225d 2e69 6c6f 635b 305d 203c 3d20  MA"].iloc[0] <= 
+0001b830: 7265 6365 6e74 5b22 4c4d 4122 5d2e 696c  recent["LMA"].il
+0001b840: 6f63 5b30 5d29 2061 6e64 205c 0d0a 2020  oc[0]) and \..  
+0001b850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b860: 2020 2020 2020 2020 2020 2872 6563 656e            (recen
+0001b870: 745b 2253 4d41 225d 2e69 6c6f 635b 315d  t["SMA"].iloc[1]
+0001b880: 203e 3d20 7265 6365 6e74 5b22 4c4d 4122   >= recent["LMA"
+0001b890: 5d2e 696c 6f63 5b31 5d29 0d0a 2020 2020  ].iloc[1])..    
+0001b8a0: 2020 2020 6973 3530 444d 4120 3d20 2872      is50DMA = (r
+0001b8b0: 6563 656e 745b 2253 4d41 225d 2e69 6c6f  ecent["SMA"].ilo
+0001b8c0: 635b 305d 203c 3d20 7265 6365 6e74 5b22  c[0] <= recent["
+0001b8d0: 436c 6f73 6522 5d2e 696c 6f63 5b30 5d29  Close"].iloc[0])
+0001b8e0: 0d0a 2020 2020 2020 2020 6973 3230 3044  ..        is200D
+0001b8f0: 4d41 203d 2028 7265 6365 6e74 5b22 4c4d  MA = (recent["LM
+0001b900: 4122 5d2e 696c 6f63 5b30 5d20 3c3d 2072  A"].iloc[0] <= r
+0001b910: 6563 656e 745b 2243 6c6f 7365 225d 2e69  ecent["Close"].i
+0001b920: 6c6f 635b 305d 290d 0a20 2020 2020 2020  loc[0])..       
+0001b930: 2064 6966 6665 7265 6e63 6520 3d20 726f   difference = ro
+0001b940: 756e 6428 2872 6563 656e 745b 2253 4d41  und((recent["SMA
+0001b950: 225d 2e69 6c6f 635b 305d 202d 2072 6563  "].iloc[0] - rec
+0001b960: 656e 745b 224c 4d41 225d 2e69 6c6f 635b  ent["LMA"].iloc[
+0001b970: 305d 290d 0a20 2020 2020 2020 2020 2020  0])..           
+0001b980: 2020 2020 202f 2072 6563 656e 745b 2243       / recent["C
+0001b990: 6c6f 7365 225d 2e69 6c6f 635b 305d 0d0a  lose"].iloc[0]..
+0001b9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b9b0: 2a20 3130 302c 0d0a 2020 2020 2020 2020  * 100,..        
+0001b9c0: 2020 2020 2020 2020 322c 0d0a 2020 2020          2,..    
+0001b9d0: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
+0001b9e0: 2020 2073 6176 6544 6963 745b 2243 6f6e     saveDict["Con
+0001b9f0: 6644 4d41 4469 6666 6572 656e 6365 225d  fDMADifference"]
+0001ba00: 203d 2064 6966 6665 7265 6e63 650d 0a20   = difference.. 
+0001ba10: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
+0001ba20: 745b 2243 6f6e 6644 4d41 4469 6666 6572  t["ConfDMADiffer
+0001ba30: 656e 6365 225d 203d 2064 6966 6665 7265  ence"] = differe
+0001ba40: 6e63 650d 0a20 2020 2020 2020 2073 6176  nce..        sav
+0001ba50: 6564 203d 2073 656c 662e 6669 6e64 4375  ed = self.findCu
+0001ba60: 7272 656e 7453 6176 6564 5661 6c75 6528  rrentSavedValue(
+0001ba70: 7363 7265 656e 4469 6374 2c73 6176 6544  screenDict,saveD
+0001ba80: 6963 742c 224d 412d 5369 676e 616c 2229  ict,"MA-Signal")
+0001ba90: 0d0a 2020 2020 2020 2020 2320 6469 6666  ..        # diff
+0001baa0: 6572 656e 6365 203d 2061 6273 2864 6966  erence = abs(dif
+0001bab0: 6665 7265 6e63 6529 0d0a 2020 2020 2020  ference)..      
+0001bac0: 2020 636f 6e66 5465 7874 203d 2066 227b    confText = f"{
+0001bad0: 2747 6f6c 6465 6e43 726f 7373 6f76 6572  'GoldenCrossover
+0001bae0: 2720 6966 2069 7347 6f6c 6465 6e43 726f  ' if isGoldenCro
+0001baf0: 7373 4f76 6572 2065 6c73 6520 2827 4465  ssOver else ('De
+0001bb00: 6164 4372 6f73 736f 7665 7227 2069 6620  adCrossover' if 
+0001bb10: 6973 4465 6164 4372 6f73 734f 7665 7220  isDeadCrossOver 
+0001bb20: 656c 7365 2028 2743 6f6e 662e 5570 2720  else ('Conf.Up' 
+0001bb30: 6966 2069 7335 3044 4d41 5570 5472 656e  if is50DMAUpTren
+0001bb40: 6420 656c 7365 2028 2743 6f6e 662e 446f  d else ('Conf.Do
+0001bb50: 776e 2720 6966 2069 7335 3044 4d41 446f  wn' if is50DMADo
+0001bb60: 776e 5472 656e 6420 656c 7365 2028 2735  wnTrend else ('5
+0001bb70: 3044 4d41 2720 6966 2069 7335 3044 4d41  0DMA' if is50DMA
+0001bb80: 2065 6c73 6520 2827 3230 3044 4d41 2720   else ('200DMA' 
+0001bb90: 6966 2069 7332 3030 444d 4120 656c 7365  if is200DMA else
+0001bba0: 2027 556e 6b6e 6f77 6e27 2929 2929 297d   'Unknown')))))}
+0001bbb0: 220d 0a20 2020 2020 2020 2069 6620 6162  "..        if ab
+0001bbc0: 7328 7265 6365 6e74 5b22 534d 4122 5d2e  s(recent["SMA"].
+0001bbd0: 696c 6f63 5b30 5d20 2d20 7265 6365 6e74  iloc[0] - recent
+0001bbe0: 5b22 4c4d 4122 5d2e 696c 6f63 5b30 5d29  ["LMA"].iloc[0])
+0001bbf0: 203c 3d20 280d 0a20 2020 2020 2020 2020   <= (..         
+0001bc00: 2020 2072 6563 656e 745b 2253 4d41 225d     recent["SMA"]
+0001bc10: 2e69 6c6f 635b 305d 202a 2070 6572 6365  .iloc[0] * perce
+0001bc20: 6e74 6167 650d 0a20 2020 2020 2020 2029  ntage..        )
+0001bc30: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
+0001bc40: 6620 7265 6365 6e74 5b22 534d 4122 5d2e  f recent["SMA"].
+0001bc50: 696c 6f63 5b30 5d20 3e3d 2072 6563 656e  iloc[0] >= recen
+0001bc60: 745b 224c 4d41 225d 2e69 6c6f 635b 305d  t["LMA"].iloc[0]
+0001bc70: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0001bc80: 2020 2073 6372 6565 6e44 6963 745b 224d     screenDict["M
+0001bc90: 412d 5369 676e 616c 225d 203d 2028 0d0a  A-Signal"] = (..
+0001bca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bcb0: 2020 2020 7361 7665 645b 305d 200d 0a20      saved[0] .. 
+0001bcc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bcd0: 2020 202b 2063 6f6c 6f72 5465 7874 2e42     + colorText.B
+0001bce0: 4f4c 440d 0a20 2020 2020 2020 2020 2020  OLD..           
+0001bcf0: 2020 2020 2020 2020 202b 2028 636f 6c6f           + (colo
+0001bd00: 7254 6578 742e 4752 4545 4e20 6966 2069  rText.GREEN if i
+0001bd10: 7335 3044 4d41 5570 5472 656e 6420 656c  s50DMAUpTrend el
+0001bd20: 7365 2028 636f 6c6f 7254 6578 742e 4641  se (colorText.FA
+0001bd30: 494c 2069 6620 6973 3530 444d 4144 6f77  IL if is50DMADow
+0001bd40: 6e54 7265 6e64 2065 6c73 6520 636f 6c6f  nTrend else colo
+0001bd50: 7254 6578 742e 5741 524e 2929 0d0a 2020  rText.WARN))..  
+0001bd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bd70: 2020 2b20 6622 7b63 6f6e 6654 6578 747d    + f"{confText}
+0001bd80: 2028 7b64 6966 6665 7265 6e63 657d 2529   ({difference}%)
+0001bd90: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
+0001bda0: 2020 2020 2020 202b 2063 6f6c 6f72 5465         + colorTe
+0001bdb0: 7874 2e45 4e44 0d0a 2020 2020 2020 2020  xt.END..        
+0001bdc0: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
+0001bdd0: 2020 2020 2020 2020 2020 2073 6176 6544             saveD
+0001bde0: 6963 745b 224d 412d 5369 676e 616c 225d  ict["MA-Signal"]
+0001bdf0: 203d 2073 6176 6564 5b31 5d20 2b20 6622   = saved[1] + f"
+0001be00: 7b63 6f6e 6654 6578 747d 2028 7b64 6966  {confText} ({dif
+0001be10: 6665 7265 6e63 657d 2529 220d 0a20 2020  ference}%)"..   
+0001be20: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
+0001be30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001be40: 7363 7265 656e 4469 6374 5b22 4d41 2d53  screenDict["MA-S
+0001be50: 6967 6e61 6c22 5d20 3d20 280d 0a20 2020  ignal"] = (..   
+0001be60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001be70: 2073 6176 6564 5b30 5d20 0d0a 2020 2020   saved[0] ..    
+0001be80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001be90: 2b20 636f 6c6f 7254 6578 742e 424f 4c44  + colorText.BOLD
+0001bea0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001beb0: 2020 2020 2020 2b20 2863 6f6c 6f72 5465        + (colorTe
+0001bec0: 7874 2e47 5245 454e 2069 6620 6973 3530  xt.GREEN if is50
+0001bed0: 444d 4155 7054 7265 6e64 2065 6c73 6520  DMAUpTrend else 
+0001bee0: 2863 6f6c 6f72 5465 7874 2e46 4149 4c20  (colorText.FAIL 
+0001bef0: 6966 2069 7335 3044 4d41 446f 776e 5472  if is50DMADownTr
+0001bf00: 656e 6420 656c 7365 2063 6f6c 6f72 5465  end else colorTe
+0001bf10: 7874 2e57 4152 4e29 290d 0a20 2020 2020  xt.WARN))..     
+0001bf20: 2020 2020 2020 2020 2020 2020 2020 202b                 +
+0001bf30: 2066 227b 636f 6e66 5465 7874 7d20 287b   f"{confText} ({
+0001bf40: 6469 6666 6572 656e 6365 7d25 2922 0d0a  difference}%)"..
+0001bf50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bf60: 2020 2020 2b20 636f 6c6f 7254 6578 742e      + colorText.
+0001bf70: 454e 440d 0a20 2020 2020 2020 2020 2020  END..           
+0001bf80: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+0001bf90: 2020 2020 2020 2020 7361 7665 4469 6374          saveDict
+0001bfa0: 5b22 4d41 2d53 6967 6e61 6c22 5d20 3d20  ["MA-Signal"] = 
+0001bfb0: 7361 7665 645b 315d 202b 2066 227b 636f  saved[1] + f"{co
+0001bfc0: 6e66 5465 7874 7d20 287b 6469 6666 6572  nfText} ({differ
+0001bfd0: 656e 6365 7d25 2922 0d0a 2020 2020 2020  ence}%)"..      
+0001bfe0: 2020 2020 2020 7265 7475 726e 2063 6f6e        return con
+0001bff0: 6646 696c 7465 7220 3d3d 2033 206f 7220  fFilter == 3 or 
+0001c000: 5c0d 0a20 2020 2020 2020 2020 2020 2020  \..             
+0001c010: 2020 2028 636f 6e66 4669 6c74 6572 203d     (confFilter =
+0001c020: 3d20 3120 616e 6420 2869 7335 3044 4d41  = 1 and (is50DMA
+0001c030: 5570 5472 656e 6420 6f72 2028 6973 476f  UpTrend or (isGo
+0001c040: 6c64 656e 4372 6f73 734f 7665 7220 6f72  ldenCrossOver or
+0001c050: 2027 5570 2720 696e 2063 6f6e 6654 6578   'Up' in confTex
+0001c060: 7429 2929 206f 7220 5c0d 0a20 2020 2020  t))) or \..     
+0001c070: 2020 2020 2020 2020 2020 2028 636f 6e66             (conf
+0001c080: 4669 6c74 6572 203d 3d20 3220 616e 6420  Filter == 2 and 
+0001c090: 2869 7335 3044 4d41 446f 776e 5472 656e  (is50DMADownTren
+0001c0a0: 6420 6f72 2069 7344 6561 6443 726f 7373  d or isDeadCross
+0001c0b0: 4f76 6572 206f 7220 2744 6f77 6e27 2069  Over or 'Down' i
+0001c0c0: 6e20 636f 6e66 5465 7874 2929 0d0a 2020  n confText))..  
+0001c0d0: 2020 2020 2020 2320 4d61 7962 6520 7468        # Maybe th
+0001c0e0: 6520 6469 6666 6572 656e 6365 2069 7320  e difference is 
+0001c0f0: 6e6f 7420 7769 7468 696e 2074 6865 2072  not within the r
+0001c100: 616e 6765 2c20 6275 7420 7765 2764 2073  ange, but we'd s
+0001c110: 7469 6c6c 206c 696b 6520 746f 206b 6565  till like to kee
+0001c120: 7020 7468 6520 7374 6f63 6b20 696e 0d0a  p the stock in..
+0001c130: 2020 2020 2020 2020 2320 7468 6520 6c69          # the li
+0001c140: 7374 2069 6620 6974 2773 2061 2067 6f6c  st if it's a gol
+0001c150: 6465 6e20 6372 6f73 736f 7665 7220 6f72  den crossover or
+0001c160: 2064 6561 6420 6372 6f73 736f 7665 720d   dead crossover.
+0001c170: 0a20 2020 2020 2020 2069 6620 6973 476f  .        if isGo
+0001c180: 6c64 656e 4372 6f73 734f 7665 7220 6f72  ldenCrossOver or
+0001c190: 2069 7344 6561 6443 726f 7373 4f76 6572   isDeadCrossOver
+0001c1a0: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+0001c1b0: 6372 6565 6e44 6963 745b 224d 412d 5369  creenDict["MA-Si
+0001c1c0: 676e 616c 225d 203d 2028 0d0a 2020 2020  gnal"] = (..    
+0001c1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c1e0: 7361 7665 645b 305d 200d 0a20 2020 2020  saved[0] ..     
+0001c1f0: 2020 2020 2020 2020 2020 2020 2020 202b                 +
+0001c200: 2063 6f6c 6f72 5465 7874 2e42 4f4c 440d   colorText.BOLD.
+0001c210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001c220: 2020 2020 202b 2028 636f 6c6f 7254 6578       + (colorTex
+0001c230: 742e 4752 4545 4e20 6966 2069 7335 3044  t.GREEN if is50D
+0001c240: 4d41 5570 5472 656e 6420 656c 7365 2028  MAUpTrend else (
+0001c250: 636f 6c6f 7254 6578 742e 4641 494c 2069  colorText.FAIL i
+0001c260: 6620 6973 3530 444d 4144 6f77 6e54 7265  f is50DMADownTre
+0001c270: 6e64 2065 6c73 6520 636f 6c6f 7254 6578  nd else colorTex
+0001c280: 742e 5741 524e 2929 0d0a 2020 2020 2020  t.WARN))..      
+0001c290: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+0001c2a0: 6622 7b63 6f6e 6654 6578 747d 2028 7b64  f"{confText} ({d
+0001c2b0: 6966 6665 7265 6e63 657d 2529 220d 0a20  ifference}%)".. 
+0001c2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c2d0: 2020 202b 2063 6f6c 6f72 5465 7874 2e45     + colorText.E
+0001c2e0: 4e44 0d0a 2020 2020 2020 2020 2020 2020  ND..            
+0001c2f0: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
+0001c300: 2020 2073 6176 6544 6963 745b 224d 412d     saveDict["MA-
+0001c310: 5369 676e 616c 225d 203d 2073 6176 6564  Signal"] = saved
+0001c320: 5b31 5d20 2b20 6622 7b63 6f6e 6654 6578  [1] + f"{confTex
+0001c330: 747d 2028 7b64 6966 6665 7265 6e63 657d  t} ({difference}
+0001c340: 2529 220d 0a20 2020 2020 2020 2020 2020  %)"..           
+0001c350: 2072 6574 7572 6e20 636f 6e66 4669 6c74   return confFilt
+0001c360: 6572 203d 3d20 3320 6f72 205c 0d0a 2020  er == 3 or \..  
+0001c370: 2020 2020 2020 2020 2020 2020 2020 2863                (c
+0001c380: 6f6e 6646 696c 7465 7220 3d3d 2031 2061  onfFilter == 1 a
+0001c390: 6e64 2069 7347 6f6c 6465 6e43 726f 7373  nd isGoldenCross
+0001c3a0: 4f76 6572 2920 6f72 205c 0d0a 2020 2020  Over) or \..    
+0001c3b0: 2020 2020 2020 2020 2020 2020 2863 6f6e              (con
+0001c3c0: 6646 696c 7465 7220 3d3d 2032 2061 6e64  fFilter == 2 and
+0001c3d0: 2069 7344 6561 6443 726f 7373 4f76 6572   isDeadCrossOver
+0001c3e0: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+0001c3f0: 6e20 4661 6c73 650d 0a0d 0a20 2020 2023  n False....    #
+0001c400: 406d 6561 7375 7265 5f74 696d 650d 0a20  @measure_time.. 
+0001c410: 2020 2023 2056 616c 6964 6174 6520 6966     # Validate if
+0001c420: 2073 6861 7265 2070 7269 6365 7320 6172   share prices ar
+0001c430: 6520 636f 6e73 6f6c 6964 6174 696e 670d  e consolidating.
+0001c440: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+0001c450: 6543 6f6e 736f 6c69 6461 7469 6f6e 2873  eConsolidation(s
+0001c460: 656c 662c 2064 662c 2073 6372 6565 6e44  elf, df, screenD
+0001c470: 6963 742c 2073 6176 6544 6963 742c 2070  ict, saveDict, p
+0001c480: 6572 6365 6e74 6167 653d 3130 293a 0d0a  ercentage=10):..
+0001c490: 2020 2020 2020 2020 6966 2064 6620 6973          if df is
+0001c4a0: 204e 6f6e 6520 6f72 206c 656e 2864 6629   None or len(df)
+0001c4b0: 203d 3d20 303a 0d0a 2020 2020 2020 2020   == 0:..        
+0001c4c0: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+0001c4d0: 0d0a 2020 2020 2020 2020 6461 7461 203d  ..        data =
+0001c4e0: 2064 662e 636f 7079 2829 0d0a 2020 2020   df.copy()..    
+0001c4f0: 2020 2020 6461 7461 203d 2064 6174 612e      data = data.
+0001c500: 6669 6c6c 6e61 2830 290d 0a20 2020 2020  fillna(0)..     
+0001c510: 2020 2064 6174 6120 3d20 6461 7461 2e72     data = data.r
+0001c520: 6570 6c61 6365 285b 6e70 2e69 6e66 2c20  eplace([np.inf, 
+0001c530: 2d6e 702e 696e 665d 2c20 3029 0d0a 2020  -np.inf], 0)..  
+0001c540: 2020 2020 2020 6863 203d 2064 6174 612e        hc = data.
+0001c550: 6465 7363 7269 6265 2829 5b22 436c 6f73  describe()["Clos
+0001c560: 6522 5d5b 226d 6178 225d 0d0a 2020 2020  e"]["max"]..    
+0001c570: 2020 2020 6c63 203d 2064 6174 612e 6465      lc = data.de
+0001c580: 7363 7269 6265 2829 5b22 436c 6f73 6522  scribe()["Close"
+0001c590: 5d5b 226d 696e 225d 0d0a 2020 2020 2020  ]["min"]..      
+0001c5a0: 2020 6966 2028 6863 202d 206c 6329 203c    if (hc - lc) <
+0001c5b0: 3d20 2868 6320 2a20 7065 7263 656e 7461  = (hc * percenta
+0001c5c0: 6765 202f 2031 3030 2920 616e 6420 2868  ge / 100) and (h
+0001c5d0: 6320 2d20 6c63 2021 3d20 3029 3a0d 0a20  c - lc != 0):.. 
+0001c5e0: 2020 2020 2020 2020 2020 2073 6372 6565             scree
+0001c5f0: 6e44 6963 745b 2243 6f6e 736f 6c2e 225d  nDict["Consol."]
+0001c600: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
+0001c610: 2020 2020 2020 636f 6c6f 7254 6578 742e        colorText.
+0001c620: 424f 4c44 0d0a 2020 2020 2020 2020 2020  BOLD..          
+0001c630: 2020 2020 2020 2b20 636f 6c6f 7254 6578        + colorTex
+0001c640: 742e 4752 4545 4e0d 0a20 2020 2020 2020  t.GREEN..       
+0001c650: 2020 2020 2020 2020 202b 2022 5261 6e67           + "Rang
+0001c660: 653a 220d 0a20 2020 2020 2020 2020 2020  e:"..           
+0001c670: 2020 2020 202b 2073 7472 2872 6f75 6e64       + str(round
+0001c680: 2828 6162 7328 2868 6320 2d20 6c63 2920  ((abs((hc - lc) 
+0001c690: 2f20 6863 2920 2a20 3130 3029 2c20 3129  / hc) * 100), 1)
+0001c6a0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0001c6b0: 2020 202b 2022 2522 0d0a 2020 2020 2020     + "%"..      
+0001c6c0: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
+0001c6d0: 7254 6578 742e 454e 440d 0a20 2020 2020  rText.END..     
+0001c6e0: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+0001c6f0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+0001c700: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
+0001c710: 2243 6f6e 736f 6c2e 225d 203d 2028 0d0a  "Consol."] = (..
+0001c720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c730: 636f 6c6f 7254 6578 742e 424f 4c44 0d0a  colorText.BOLD..
+0001c740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c750: 2b20 636f 6c6f 7254 6578 742e 4641 494c  + colorText.FAIL
+0001c760: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001c770: 2020 2b20 2252 616e 6765 3a22 0d0a 2020    + "Range:"..  
+0001c780: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+0001c790: 7374 7228 726f 756e 6428 2861 6273 2828  str(round((abs((
+0001c7a0: 6863 202d 206c 6329 202f 2068 6329 202a  hc - lc) / hc) *
+0001c7b0: 2031 3030 292c 2031 2929 0d0a 2020 2020   100), 1))..    
+0001c7c0: 2020 2020 2020 2020 2020 2020 2b20 2225              + "%
+0001c7d0: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
+0001c7e0: 2020 202b 2063 6f6c 6f72 5465 7874 2e45     + colorText.E
+0001c7f0: 4e44 0d0a 2020 2020 2020 2020 2020 2020  ND..            
+0001c800: 290d 0a20 2020 2020 2020 2073 6176 6544  )..        saveD
+0001c810: 6963 745b 2243 6f6e 736f 6c2e 225d 203d  ict["Consol."] =
+0001c820: 2066 2752 616e 6765 3a7b 7374 7228 726f   f'Range:{str(ro
+0001c830: 756e 6428 2861 6273 2828 6863 2d6c 6329  und((abs((hc-lc)
+0001c840: 2f68 6329 2a31 3030 292c 3129 292b 2225  /hc)*100),1))+"%
+0001c850: 227d 270d 0a20 2020 2020 2020 2072 6574  "}'..        ret
+0001c860: 7572 6e20 726f 756e 6428 2861 6273 2828  urn round((abs((
+0001c870: 6863 202d 206c 6329 202f 2068 6329 202a  hc - lc) / hc) *
+0001c880: 2031 3030 292c 2031 290d 0a0d 0a20 2020   100), 1)....   
+0001c890: 2023 2076 616c 6964 6174 6520 6966 2074   # validate if t
+0001c8a0: 6865 2073 746f 636b 2068 6173 2062 6565  he stock has bee
+0001c8b0: 6e20 6861 7669 6e67 2068 6967 6865 7220  n having higher 
+0001c8c0: 6869 6768 732c 2068 6967 6865 7220 6c6f  highs, higher lo
+0001c8d0: 7773 0d0a 2020 2020 2320 616e 6420 6869  ws..    # and hi
+0001c8e0: 6768 6572 2063 6c6f 7365 2077 6974 6820  gher close with 
+0001c8f0: 6c61 7465 7374 2063 6c6f 7365 203e 2073  latest close > s
+0001c900: 7570 6572 7472 656e 6420 616e 6420 382d  upertrend and 8-
+0001c910: 454d 412e 0d0a 2020 2020 6465 6620 7661  EMA...    def va
+0001c920: 6c69 6461 7465 4869 6768 6572 4869 6768  lidateHigherHigh
+0001c930: 7348 6967 6865 724c 6f77 7348 6967 6865  sHigherLowsHighe
+0001c940: 7243 6c6f 7365 2873 656c 662c 2064 6629  rClose(self, df)
+0001c950: 3a0d 0a20 2020 2020 2020 2069 6620 6466  :..        if df
+0001c960: 2069 7320 4e6f 6e65 206f 7220 6c65 6e28   is None or len(
+0001c970: 6466 2920 3d3d 2030 3a0d 0a20 2020 2020  df) == 0:..     
+0001c980: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+0001c990: 6c73 650d 0a20 2020 2020 2020 2064 6174  lse..        dat
+0001c9a0: 6120 3d20 6466 2e63 6f70 7928 290d 0a20  a = df.copy().. 
+0001c9b0: 2020 2020 2020 2064 6179 3020 3d20 6461         day0 = da
+0001c9c0: 7461 0d0a 2020 2020 2020 2020 6461 7931  ta..        day1
+0001c9d0: 203d 2064 6174 615b 313a 5d0d 0a20 2020   = data[1:]..   
+0001c9e0: 2020 2020 2064 6179 3220 3d20 6461 7461       day2 = data
+0001c9f0: 5b32 3a5d 0d0a 2020 2020 2020 2020 6461  [2:]..        da
+0001ca00: 7933 203d 2064 6174 615b 333a 5d0d 0a20  y3 = data[3:].. 
+0001ca10: 2020 2020 2020 2069 6620 6c65 6e28 6461         if len(da
+0001ca20: 7931 2920 3c20 3120 6f72 206c 656e 2864  y1) < 1 or len(d
+0001ca30: 6179 3229 203c 2031 206f 7220 6c65 6e28  ay2) < 1 or len(
+0001ca40: 6461 7933 2920 3c20 313a 0d0a 2020 2020  day3) < 1:..    
+0001ca50: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+0001ca60: 616c 7365 0d0a 2020 2020 2020 2020 6869  alse..        hi
+0001ca70: 6768 6572 4869 6768 7320 3d20 280d 0a20  gherHighs = (.. 
+0001ca80: 2020 2020 2020 2020 2020 2028 6461 7930             (day0
+0001ca90: 5b22 4869 6768 225d 2e69 6c6f 635b 305d  ["High"].iloc[0]
+0001caa0: 203e 2064 6179 315b 2248 6967 6822 5d2e   > day1["High"].
+0001cab0: 696c 6f63 5b30 5d29 0d0a 2020 2020 2020  iloc[0])..      
+0001cac0: 2020 2020 2020 616e 6420 2864 6179 315b        and (day1[
+0001cad0: 2248 6967 6822 5d2e 696c 6f63 5b30 5d20  "High"].iloc[0] 
+0001cae0: 3e20 6461 7932 5b22 4869 6768 225d 2e69  > day2["High"].i
+0001caf0: 6c6f 635b 305d 290d 0a20 2020 2020 2020  loc[0])..       
+0001cb00: 2020 2020 2061 6e64 2028 6461 7932 5b22       and (day2["
+0001cb10: 4869 6768 225d 2e69 6c6f 635b 305d 203e  High"].iloc[0] >
+0001cb20: 2064 6179 335b 2248 6967 6822 5d2e 696c   day3["High"].il
+0001cb30: 6f63 5b30 5d29 0d0a 2020 2020 2020 2020  oc[0])..        
+0001cb40: 290d 0a20 2020 2020 2020 2068 6967 6865  )..        highe
+0001cb50: 724c 6f77 7320 3d20 280d 0a20 2020 2020  rLows = (..     
+0001cb60: 2020 2020 2020 2028 6461 7930 5b22 4c6f         (day0["Lo
+0001cb70: 7722 5d2e 696c 6f63 5b30 5d20 3e20 6461  w"].iloc[0] > da
+0001cb80: 7931 5b22 4c6f 7722 5d2e 696c 6f63 5b30  y1["Low"].iloc[0
+0001cb90: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+0001cba0: 616e 6420 2864 6179 315b 224c 6f77 225d  and (day1["Low"]
+0001cbb0: 2e69 6c6f 635b 305d 203e 2064 6179 325b  .iloc[0] > day2[
+0001cbc0: 224c 6f77 225d 2e69 6c6f 635b 305d 290d  "Low"].iloc[0]).
+0001cbd0: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
+0001cbe0: 2028 6461 7932 5b22 4c6f 7722 5d2e 696c   (day2["Low"].il
+0001cbf0: 6f63 5b30 5d20 3e20 6461 7933 5b22 4c6f  oc[0] > day3["Lo
+0001cc00: 7722 5d2e 696c 6f63 5b30 5d29 0d0a 2020  w"].iloc[0])..  
+0001cc10: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+0001cc20: 2068 6967 6865 7243 6c6f 7365 203d 2028   higherClose = (
+0001cc30: 0d0a 2020 2020 2020 2020 2020 2020 2864  ..            (d
+0001cc40: 6179 305b 2243 6c6f 7365 225d 2e69 6c6f  ay0["Close"].ilo
+0001cc50: 635b 305d 203e 2064 6179 315b 2243 6c6f  c[0] > day1["Clo
+0001cc60: 7365 225d 2e69 6c6f 635b 305d 290d 0a20  se"].iloc[0]).. 
+0001cc70: 2020 2020 2020 2020 2020 2061 6e64 2028             and (
+0001cc80: 6461 7931 5b22 436c 6f73 6522 5d2e 696c  day1["Close"].il
+0001cc90: 6f63 5b30 5d20 3e20 6461 7932 5b22 436c  oc[0] > day2["Cl
+0001cca0: 6f73 6522 5d2e 696c 6f63 5b30 5d29 0d0a  ose"].iloc[0])..
+0001ccb0: 2020 2020 2020 2020 2020 2020 616e 6420              and 
+0001ccc0: 2864 6179 325b 2243 6c6f 7365 225d 2e69  (day2["Close"].i
+0001ccd0: 6c6f 635b 305d 203e 2064 6179 335b 2243  loc[0] > day3["C
+0001cce0: 6c6f 7365 225d 2e69 6c6f 635b 305d 290d  lose"].iloc[0]).
+0001ccf0: 0a20 2020 2020 2020 2029 0d0a 2020 2020  .        )..    
+0001cd00: 2020 2020 2320 6869 6768 6572 5253 4920      # higherRSI 
+0001cd10: 3d20 2864 6179 305b 2252 5349 225d 2e69  = (day0["RSI"].i
+0001cd20: 6c6f 635b 305d 203e 2064 6179 315b 2252  loc[0] > day1["R
+0001cd30: 5349 225d 2e69 6c6f 635b 305d 2920 616e  SI"].iloc[0]) an
+0001cd40: 6420 5c0d 0a20 2020 2020 2020 2023 2020  d \..        #  
+0001cd50: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+0001cd60: 6461 7931 5b22 5253 4922 5d2e 696c 6f63  day1["RSI"].iloc
+0001cd70: 5b30 5d20 3e20 6461 7932 5b22 5253 4922  [0] > day2["RSI"
+0001cd80: 5d2e 696c 6f63 5b30 5d29 2061 6e64 205c  ].iloc[0]) and \
+0001cd90: 0d0a 2020 2020 2020 2020 2320 2020 2020  ..        #     
+0001cda0: 2020 2020 2020 2020 2020 2020 2864 6179              (day
+0001cdb0: 325b 2252 5349 225d 2e69 6c6f 635b 305d  2["RSI"].iloc[0]
+0001cdc0: 203e 2064 6179 335b 2252 5349 225d 2e69   > day3["RSI"].i
+0001cdd0: 6c6f 635b 305d 2920 616e 6420 5c0d 0a20  loc[0]) and \.. 
+0001cde0: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+0001cdf0: 2020 2020 2020 2020 2064 6179 335b 2252           day3["R
+0001ce00: 5349 225d 2e69 6c6f 635b 305d 203e 3d20  SI"].iloc[0] >= 
+0001ce10: 3530 2061 6e64 2064 6179 305b 2252 5349  50 and day0["RSI
+0001ce20: 225d 2e69 6c6f 635b 305d 203e 3d20 3635  "].iloc[0] >= 65
+0001ce30: 0d0a 2020 2020 2020 2020 7265 7665 7273  ..        revers
+0001ce40: 6564 4461 7461 203d 2064 6174 615b 3a3a  edData = data[::
+0001ce50: 2d31 5d2e 636f 7079 2829 0d0a 2020 2020  -1].copy()..    
+0001ce60: 2020 2020 7265 7665 7273 6564 4461 7461      reversedData
+0001ce70: 5b22 5355 5045 5254 225d 203d 2070 6b74  ["SUPERT"] = pkt
+0001ce80: 616c 6962 2e73 7570 6572 7472 656e 6428  alib.supertrend(
+0001ce90: 7265 7665 7273 6564 4461 7461 2c20 372c  reversedData, 7,
+0001cea0: 2033 295b 2253 5550 4552 545f 375f 332e   3)["SUPERT_7_3.
+0001ceb0: 3022 5d0d 0a20 2020 2020 2020 2072 6576  0"]..        rev
+0001cec0: 6572 7365 6444 6174 615b 2245 4d41 3822  ersedData["EMA8"
+0001ced0: 5d20 3d20 706b 7461 6c69 622e 454d 4128  ] = pktalib.EMA(
+0001cee0: 7265 7665 7273 6564 4461 7461 5b22 436c  reversedData["Cl
+0001cef0: 6f73 6522 5d2c 2074 696d 6570 6572 696f  ose"], timeperio
+0001cf00: 643d 3929 0d0a 2020 2020 2020 2020 6869  d=9)..        hi
+0001cf10: 6768 6572 436c 6f73 6520 3d20 280d 0a20  gherClose = (.. 
+0001cf20: 2020 2020 2020 2020 2020 2068 6967 6865             highe
+0001cf30: 7243 6c6f 7365 0d0a 2020 2020 2020 2020  rClose..        
+0001cf40: 2020 2020 616e 6420 6461 7930 5b22 436c      and day0["Cl
+0001cf50: 6f73 6522 5d2e 696c 6f63 5b30 5d20 3e20  ose"].iloc[0] > 
+0001cf60: 7265 7665 7273 6564 4461 7461 2e74 6169  reversedData.tai
+0001cf70: 6c28 3129 5b22 5355 5045 5254 225d 2e69  l(1)["SUPERT"].i
+0001cf80: 6c6f 635b 305d 0d0a 2020 2020 2020 2020  loc[0]..        
+0001cf90: 2020 2020 616e 6420 6461 7930 5b22 436c      and day0["Cl
+0001cfa0: 6f73 6522 5d2e 696c 6f63 5b30 5d20 3e20  ose"].iloc[0] > 
+0001cfb0: 7265 7665 7273 6564 4461 7461 2e74 6169  reversedData.tai
+0001cfc0: 6c28 3129 5b22 454d 4138 225d 2e69 6c6f  l(1)["EMA8"].ilo
+0001cfd0: 635b 305d 0d0a 2020 2020 2020 2020 290d  c[0]..        ).
+0001cfe0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0001cff0: 6869 6768 6572 4869 6768 7320 616e 6420  higherHighs and 
+0001d000: 6869 6768 6572 4c6f 7773 2061 6e64 2068  higherLows and h
+0001d010: 6967 6865 7243 6c6f 7365 0d0a 0d0a 2020  igherClose....  
+0001d020: 2020 2340 6d65 6173 7572 655f 7469 6d65    #@measure_time
+0001d030: 0d0a 2020 2020 2320 5661 6c69 6461 7465  ..    # Validate
+0001d040: 2027 496e 7369 6465 2042 6172 2720 7374   'Inside Bar' st
+0001d050: 7275 6374 7572 6520 666f 7220 7265 6365  ructure for rece
+0001d060: 6e74 2064 6179 730d 0a20 2020 2064 6566  nt days..    def
+0001d070: 2076 616c 6964 6174 6549 6e73 6964 6542   validateInsideB
+0001d080: 6172 280d 0a20 2020 2020 2020 2073 656c  ar(..        sel
+0001d090: 662c 2064 662c 2073 6372 6565 6e44 6963  f, df, screenDic
+0001d0a0: 742c 2073 6176 6544 6963 742c 2063 6861  t, saveDict, cha
+0001d0b0: 7274 5061 7474 6572 6e3d 312c 2064 6179  rtPattern=1, day
+0001d0c0: 7354 6f4c 6f6f 6b62 6163 6b3d 350d 0a20  sToLookback=5.. 
+0001d0d0: 2020 2029 3a0d 0a20 2020 2020 2020 2069     ):..        i
+0001d0e0: 6620 6466 2069 7320 4e6f 6e65 206f 7220  f df is None or 
+0001d0f0: 6c65 6e28 6466 2920 3d3d 2030 3a0d 0a20  len(df) == 0:.. 
+0001d100: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0001d110: 6e20 4661 6c73 650d 0a20 2020 2020 2020  n False..       
+0001d120: 2064 6174 6120 3d20 6466 2e63 6f70 7928   data = df.copy(
+0001d130: 290d 0a20 2020 2020 2020 206f 7267 4461  )..        orgDa
+0001d140: 7461 203d 2064 6174 610d 0a20 2020 2020  ta = data..     
+0001d150: 2020 2073 6176 6564 203d 2073 656c 662e     saved = self.
+0001d160: 6669 6e64 4375 7272 656e 7453 6176 6564  findCurrentSaved
+0001d170: 5661 6c75 6528 7363 7265 656e 4469 6374  Value(screenDict
+0001d180: 2c20 7361 7665 4469 6374 2c20 2250 6174  , saveDict, "Pat
+0001d190: 7465 726e 2229 0d0a 2020 2020 2020 2020  tern")..        
+0001d1a0: 666f 7220 6920 696e 2072 616e 6765 2869  for i in range(i
+0001d1b0: 6e74 2864 6179 7354 6f4c 6f6f 6b62 6163  nt(daysToLookbac
+0001d1c0: 6b29 2c20 696e 7428 726f 756e 6428 6461  k), int(round(da
+0001d1d0: 7973 546f 4c6f 6f6b 6261 636b 202a 2030  ysToLookback * 0
+0001d1e0: 2e35 2929 202d 2031 2c20 2d31 293a 0d0a  .5)) - 1, -1):..
+0001d1f0: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+0001d200: 203d 3d20 323a 0d0a 2020 2020 2020 2020   == 2:..        
+0001d210: 2020 2020 2020 2020 7265 7475 726e 2030          return 0
+0001d220: 2020 2320 4578 6974 2069 6620 6f6e 6c79    # Exit if only
+0001d230: 206c 6173 7420 3220 6361 6e64 6c65 7320   last 2 candles 
+0001d240: 6172 6520 6c65 6674 0d0a 2020 2020 2020  are left..      
+0001d250: 2020 2020 2020 6966 2063 6861 7274 5061        if chartPa
+0001d260: 7474 6572 6e20 3d3d 2031 3a0d 0a20 2020  ttern == 1:..   
+0001d270: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0001d280: 2255 7022 2069 6e20 7361 7665 4469 6374  "Up" in saveDict
+0001d290: 5b22 5472 656e 6422 5d20 616e 6420 280d  ["Trend"] and (.
+0001d2a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001d2b0: 2020 2020 2022 4275 6c6c 2220 696e 2073       "Bull" in s
+0001d2c0: 6176 6544 6963 745b 224d 412d 5369 676e  aveDict["MA-Sign
+0001d2d0: 616c 225d 0d0a 2020 2020 2020 2020 2020  al"]..          
+0001d2e0: 2020 2020 2020 2020 2020 6f72 2022 5375            or "Su
+0001d2f0: 7070 6f72 7422 2069 6e20 7361 7665 4469  pport" in saveDi
+0001d300: 6374 5b22 4d41 2d53 6967 6e61 6c22 5d0d  ct["MA-Signal"].
+0001d310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001d320: 2029 3a0d 0a20 2020 2020 2020 2020 2020   ):..           
+0001d330: 2020 2020 2020 2020 2064 6174 6120 3d20           data = 
+0001d340: 6f72 6744 6174 612e 6865 6164 2869 290d  orgData.head(i).
+0001d350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001d360: 2020 2020 2072 6566 4361 6e64 6c65 203d       refCandle =
+0001d370: 2064 6174 612e 7461 696c 2831 290d 0a20   data.tail(1).. 
+0001d380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d390: 2020 2069 6620 280d 0a20 2020 2020 2020     if (..       
+0001d3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d3b0: 2028 6c65 6e28 6461 7461 2e48 6967 685b   (len(data.High[
+0001d3c0: 6461 7461 2e48 6967 6820 3e20 7265 6643  data.High > refC
+0001d3d0: 616e 646c 652e 4869 6768 2e69 7465 6d28  andle.High.item(
+0001d3e0: 295d 2920 3d3d 2030 290d 0a20 2020 2020  )]) == 0)..     
+0001d3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d400: 2020 2061 6e64 2028 6c65 6e28 6461 7461     and (len(data
+0001d410: 2e4c 6f77 5b64 6174 612e 4c6f 7720 3c20  .Low[data.Low < 
+0001d420: 7265 6643 616e 646c 652e 4c6f 772e 6974  refCandle.Low.it
+0001d430: 656d 2829 5d29 203d 3d20 3029 0d0a 2020  em()]) == 0)..  
+0001d440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d450: 2020 2020 2020 616e 6420 286c 656e 2864        and (len(d
+0001d460: 6174 612e 4f70 656e 5b64 6174 612e 4f70  ata.Open[data.Op
+0001d470: 656e 203e 2072 6566 4361 6e64 6c65 2e48  en > refCandle.H
+0001d480: 6967 682e 6974 656d 2829 5d29 203d 3d20  igh.item()]) == 
+0001d490: 3029 0d0a 2020 2020 2020 2020 2020 2020  0)..            
+0001d4a0: 2020 2020 2020 2020 2020 2020 616e 6420              and 
+0001d4b0: 286c 656e 2864 6174 612e 436c 6f73 655b  (len(data.Close[
+0001d4c0: 6461 7461 2e43 6c6f 7365 203c 2072 6566  data.Close < ref
+0001d4d0: 4361 6e64 6c65 2e4c 6f77 2e69 7465 6d28  Candle.Low.item(
+0001d4e0: 295d 2920 3d3d 2030 290d 0a20 2020 2020  )]) == 0)..     
+0001d4f0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+0001d500: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0001d510: 2020 2020 2020 2020 2020 2073 6372 6565             scree
+0001d520: 6e44 6963 745b 2250 6174 7465 726e 225d  nDict["Pattern"]
+0001d530: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
+0001d540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d550: 2020 7361 7665 645b 305d 0d0a 2020 2020    saved[0]..    
+0001d560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d570: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
+0001d580: 6578 742e 424f 4c44 0d0a 2020 2020 2020  ext.BOLD..      
+0001d590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d5a0: 2020 2020 2020 2b20 636f 6c6f 7254 6578        + colorTex
+0001d5b0: 742e 5741 524e 0d0a 2020 2020 2020 2020  t.WARN..        
+0001d5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d5d0: 2020 2020 2b20 2822 496e 7369 6465 2042      + ("Inside B
+0001d5e0: 6172 2028 2564 2922 2025 2069 290d 0a20  ar (%d)" % i).. 
+0001d5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d600: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
+0001d610: 6f72 5465 7874 2e45 4e44 0d0a 2020 2020  orText.END..    
 0001d620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d630: 2020 2020 2020 2020 616e 6420 286c 656e          and (len
-0001d640: 2864 6174 612e 4f70 656e 5b64 6174 612e  (data.Open[data.
-0001d650: 4f70 656e 203e 2072 6566 4361 6e64 6c65  Open > refCandle
-0001d660: 2e48 6967 682e 6974 656d 2829 5d29 203d  .High.item()]) =
-0001d670: 3d20 3029 0d0a 2020 2020 2020 2020 2020  = 0)..          
-0001d680: 2020 2020 2020 2020 2020 2020 2020 616e                an
-0001d690: 6420 286c 656e 2864 6174 612e 436c 6f73  d (len(data.Clos
-0001d6a0: 655b 6461 7461 2e43 6c6f 7365 203c 2072  e[data.Close < r
-0001d6b0: 6566 4361 6e64 6c65 2e4c 6f77 2e69 7465  efCandle.Low.ite
-0001d6c0: 6d28 295d 2920 3d3d 2030 290d 0a20 2020  m()]) == 0)..   
-0001d6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d6e0: 2029 3a0d 0a20 2020 2020 2020 2020 2020   ):..           
-0001d6f0: 2020 2020 2020 2020 2020 2020 2073 6372               scr
-0001d700: 6565 6e44 6963 745b 2250 6174 7465 726e  eenDict["Pattern
-0001d710: 225d 203d 2028 0d0a 2020 2020 2020 2020  "] = (..        
-0001d720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d730: 2020 2020 7361 7665 645b 305d 0d0a 2020      saved[0]..  
-0001d740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d750: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
-0001d760: 7254 6578 742e 424f 4c44 0d0a 2020 2020  rText.BOLD..    
-0001d770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d780: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
-0001d790: 6578 742e 5741 524e 0d0a 2020 2020 2020  ext.WARN..      
-0001d7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d7b0: 2020 2020 2020 2b20 2822 496e 7369 6465        + ("Inside
-0001d7c0: 2042 6172 2028 2564 2922 2025 2069 290d   Bar (%d)" % i).
-0001d7d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001d7e0: 2020 2020 2020 2020 2020 2020 202b 2063               + c
-0001d7f0: 6f6c 6f72 5465 7874 2e45 4e44 0d0a 2020  olorText.END..  
-0001d800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d810: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-0001d820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d830: 2073 6176 6544 6963 745b 2250 6174 7465   saveDict["Patte
-0001d840: 726e 225d 203d 2073 6176 6564 5b31 5d20  rn"] = saved[1] 
-0001d850: 2b20 2249 6e73 6964 6520 4261 7220 2825  + "Inside Bar (%
-0001d860: 6429 2220 2520 690d 0a20 2020 2020 2020  d)" % i..       
-0001d870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d880: 2072 6574 7572 6e20 690d 0a20 2020 2020   return i..     
-0001d890: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0001d8a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001d8b0: 2020 2020 2020 7265 7475 726e 2030 0d0a        return 0..
-0001d8c0: 2020 2020 2020 2020 7265 7475 726e 2030          return 0
-0001d8d0: 0d0a 0d0a 2020 2020 2320 4669 6e64 2049  ....    # Find I
-0001d8e0: 504f 2062 6173 650d 0a20 2020 2064 6566  PO base..    def
-0001d8f0: 2076 616c 6964 6174 6549 706f 4261 7365   validateIpoBase
-0001d900: 2873 656c 662c 2073 746f 636b 2c20 6466  (self, stock, df
-0001d910: 2c20 7363 7265 656e 4469 6374 2c20 7361  , screenDict, sa
-0001d920: 7665 4469 6374 2c20 7065 7263 656e 7461  veDict, percenta
-0001d930: 6765 3d30 2e33 293a 0d0a 2020 2020 2020  ge=0.3):..      
-0001d940: 2020 6966 2064 6620 6973 204e 6f6e 6520    if df is None 
-0001d950: 6f72 206c 656e 2864 6629 203d 3d20 303a  or len(df) == 0:
-0001d960: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-0001d970: 7475 726e 2046 616c 7365 0d0a 2020 2020  turn False..    
-0001d980: 2020 2020 6461 7461 203d 2064 662e 636f      data = df.co
-0001d990: 7079 2829 0d0a 2020 2020 2020 2020 6c69  py()..        li
-0001d9a0: 7374 696e 6750 7269 6365 203d 2064 6174  stingPrice = dat
-0001d9b0: 615b 3a3a 2d31 5d2e 6865 6164 2831 295b  a[::-1].head(1)[
-0001d9c0: 224f 7065 6e22 5d2e 696c 6f63 5b30 5d0d  "Open"].iloc[0].
-0001d9d0: 0a20 2020 2020 2020 2063 7572 7265 6e74  .        current
-0001d9e0: 5072 6963 6520 3d20 6461 7461 2e68 6561  Price = data.hea
-0001d9f0: 6428 3129 5b22 436c 6f73 6522 5d2e 696c  d(1)["Close"].il
-0001da00: 6f63 5b30 5d0d 0a20 2020 2020 2020 2041  oc[0]..        A
-0001da10: 5448 203d 2064 6174 612e 6465 7363 7269  TH = data.descri
-0001da20: 6265 2829 5b22 4869 6768 225d 5b22 6d61  be()["High"]["ma
-0001da30: 7822 5d0d 0a20 2020 2020 2020 2069 6620  x"]..        if 
-0001da40: 4154 4820 3e20 286c 6973 7469 6e67 5072  ATH > (listingPr
-0001da50: 6963 6520 2b20 286c 6973 7469 6e67 5072  ice + (listingPr
-0001da60: 6963 6520 2a20 7065 7263 656e 7461 6765  ice * percentage
-0001da70: 2929 3a0d 0a20 2020 2020 2020 2020 2020  )):..           
-0001da80: 2072 6574 7572 6e20 4661 6c73 650d 0a20   return False.. 
-0001da90: 2020 2020 2020 2061 7761 7920 3d20 726f         away = ro
-0001daa0: 756e 6428 2828 6375 7272 656e 7450 7269  und(((currentPri
-0001dab0: 6365 202d 206c 6973 7469 6e67 5072 6963  ce - listingPric
-0001dac0: 6529 202f 206c 6973 7469 6e67 5072 6963  e) / listingPric
-0001dad0: 6529 202a 2031 3030 2c20 3129 0d0a 2020  e) * 100, 1)..  
-0001dae0: 2020 2020 2020 6966 2028 0d0a 2020 2020        if (..    
-0001daf0: 2020 2020 2020 2020 286c 6973 7469 6e67          (listing
-0001db00: 5072 6963 6520 2d20 286c 6973 7469 6e67  Price - (listing
-0001db10: 5072 6963 6520 2a20 7065 7263 656e 7461  Price * percenta
-0001db20: 6765 2929 0d0a 2020 2020 2020 2020 2020  ge))..          
-0001db30: 2020 3c3d 2063 7572 7265 6e74 5072 6963    <= currentPric
-0001db40: 650d 0a20 2020 2020 2020 2020 2020 203c  e..            <
-0001db50: 3d20 286c 6973 7469 6e67 5072 6963 6520  = (listingPrice 
-0001db60: 2b20 286c 6973 7469 6e67 5072 6963 6520  + (listingPrice 
-0001db70: 2a20 7065 7263 656e 7461 6765 2929 0d0a  * percentage))..
-0001db80: 2020 2020 2020 2020 293a 0d0a 2020 2020          ):..    
-0001db90: 2020 2020 2020 2020 7361 7665 6420 3d20          saved = 
-0001dba0: 7365 6c66 2e66 696e 6443 7572 7265 6e74  self.findCurrent
-0001dbb0: 5361 7665 6456 616c 7565 2873 6372 6565  SavedValue(scree
-0001dbc0: 6e44 6963 742c 2073 6176 6544 6963 742c  nDict, saveDict,
-0001dbd0: 2022 5061 7474 6572 6e22 290d 0a20 2020   "Pattern")..   
-0001dbe0: 2020 2020 2020 2020 2069 6620 6177 6179           if away
-0001dbf0: 203e 2030 3a0d 0a20 2020 2020 2020 2020   > 0:..         
-0001dc00: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
-0001dc10: 745b 2250 6174 7465 726e 225d 203d 2028  t["Pattern"] = (
-0001dc20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001dc30: 2020 2020 2020 7361 7665 645b 305d 200d        saved[0] .
-0001dc40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001dc50: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
-0001dc60: 2e42 4f4c 440d 0a20 2020 2020 2020 2020  .BOLD..         
-0001dc70: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
-0001dc80: 6f72 5465 7874 2e47 5245 454e 0d0a 2020  orText.GREEN..  
-0001dc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dca0: 2020 2b20 6622 4950 4f20 4261 7365 2028    + f"IPO Base (
-0001dcb0: 7b61 7761 797d 2025 2922 0d0a 2020 2020  {away} %)"..    
-0001dcc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dcd0: 2b20 636f 6c6f 7254 6578 742e 454e 440d  + colorText.END.
-0001dce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001dcf0: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
-0001dd00: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-0001dd10: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
-0001dd20: 745b 2250 6174 7465 726e 225d 203d 2028  t["Pattern"] = (
-0001dd30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001dd40: 2020 2020 2020 7361 7665 645b 305d 0d0a        saved[0]..
-0001dd50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dd60: 2020 2020 2b20 636f 6c6f 7254 6578 742e      + colorText.
-0001dd70: 424f 4c44 0d0a 2020 2020 2020 2020 2020  BOLD..          
-0001dd80: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
-0001dd90: 7254 6578 742e 4752 4545 4e0d 0a20 2020  rText.GREEN..   
-0001dda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ddb0: 202b 2022 4950 4f20 4261 7365 2022 0d0a   + "IPO Base "..
-0001ddc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ddd0: 2020 2020 2b20 636f 6c6f 7254 6578 742e      + colorText.
-0001dde0: 4641 494c 0d0a 2020 2020 2020 2020 2020  FAIL..          
-0001ddf0: 2020 2020 2020 2020 2020 2b20 6622 287b            + f"({
-0001de00: 6177 6179 7d20 2529 220d 0a20 2020 2020  away} %)"..     
-0001de10: 2020 2020 2020 2020 2020 2020 2020 202b                 +
-0001de20: 2063 6f6c 6f72 5465 7874 2e45 4e44 0d0a   colorText.END..
-0001de30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001de40: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
-0001de50: 6176 6544 6963 745b 2250 6174 7465 726e  aveDict["Pattern
-0001de60: 225d 203d 2073 6176 6564 5b31 5d20 2b20  "] = saved[1] + 
-0001de70: 6622 4950 4f20 4261 7365 2028 7b61 7761  f"IPO Base ({awa
-0001de80: 797d 2025 2922 0d0a 2020 2020 2020 2020  y} %)"..        
-0001de90: 2020 2020 7265 7475 726e 2054 7275 650d      return True.
-0001dea0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0001deb0: 4661 6c73 650d 0a0d 0a20 2020 2023 406d  False....    #@m
-0001dec0: 6561 7375 7265 5f74 696d 650d 0a20 2020  easure_time..   
-0001ded0: 2023 2056 616c 6964 6174 6520 4c6f 7265   # Validate Lore
-0001dee0: 6e74 7a69 616e 2043 6c61 7373 6966 6963  ntzian Classific
-0001def0: 6174 696f 6e20 7369 676e 616c 0d0a 2020  ation signal..  
-0001df00: 2020 6465 6620 7661 6c69 6461 7465 4c6f    def validateLo
-0001df10: 7265 6e74 7a69 616e 2873 656c 662c 2064  rentzian(self, d
-0001df20: 662c 2073 6372 6565 6e44 6963 742c 2073  f, screenDict, s
-0001df30: 6176 6544 6963 742c 206c 6f6f 6b46 6f72  aveDict, lookFor
-0001df40: 3d33 293a 0d0a 2020 2020 2020 2020 6966  =3):..        if
-0001df50: 2064 6620 6973 204e 6f6e 6520 6f72 206c   df is None or l
-0001df60: 656e 2864 6629 203d 3d20 303a 0d0a 2020  en(df) == 0:..  
-0001df70: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0001df80: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
-0001df90: 6461 7461 203d 2064 662e 636f 7079 2829  data = df.copy()
-0001dfa0: 0d0a 2020 2020 2020 2020 2320 6c6f 6f6b  ..        # look
-0001dfb0: 466f 723a 2031 2d42 7579 2c20 322d 5365  For: 1-Buy, 2-Se
-0001dfc0: 6c6c 2c20 332d 416e 790d 0a20 2020 2020  ll, 3-Any..     
-0001dfd0: 2020 2064 6174 6120 3d20 6461 7461 5b3a     data = data[:
-0001dfe0: 3a2d 315d 2020 2320 5265 7665 7273 6520  :-1]  # Reverse 
-0001dff0: 7468 6520 6461 7461 6672 616d 650d 0a20  the dataframe.. 
-0001e000: 2020 2020 2020 2064 6174 6120 3d20 6461         data = da
-0001e010: 7461 2e72 656e 616d 6528 0d0a 2020 2020  ta.rename(..    
-0001e020: 2020 2020 2020 2020 636f 6c75 6d6e 733d          columns=
-0001e030: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
-0001e040: 2020 2022 4f70 656e 223a 2022 6f70 656e     "Open": "open
-0001e050: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-0001e060: 2020 2020 2243 6c6f 7365 223a 2022 636c      "Close": "cl
-0001e070: 6f73 6522 2c0d 0a20 2020 2020 2020 2020  ose",..         
-0001e080: 2020 2020 2020 2022 4869 6768 223a 2022         "High": "
-0001e090: 6869 6768 222c 0d0a 2020 2020 2020 2020  high",..        
-0001e0a0: 2020 2020 2020 2020 224c 6f77 223a 2022          "Low": "
-0001e0b0: 6c6f 7722 2c0d 0a20 2020 2020 2020 2020  low",..         
-0001e0c0: 2020 2020 2020 2022 566f 6c75 6d65 223a         "Volume":
-0001e0d0: 2022 766f 6c75 6d65 222c 0d0a 2020 2020   "volume",..    
-0001e0e0: 2020 2020 2020 2020 7d0d 0a20 2020 2020          }..     
-0001e0f0: 2020 2029 0d0a 2020 2020 2020 2020 7472     )..        tr
-0001e100: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
-0001e110: 7769 7468 2053 7570 7072 6573 734f 7574  with SuppressOut
-0001e120: 7075 7428 7375 7070 7265 7373 5f73 7464  put(suppress_std
-0001e130: 6f75 743d 5472 7565 2c20 7375 7070 7265  out=True, suppre
-0001e140: 7373 5f73 7464 6572 723d 5472 7565 293a  ss_stderr=True):
-0001e150: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001e160: 2020 6c63 203d 2061 7461 2e4c 6f72 656e    lc = ata.Loren
-0001e170: 747a 6961 6e43 6c61 7373 6966 6963 6174  tzianClassificat
-0001e180: 696f 6e28 6461 7461 3d64 6174 6129 0d0a  ion(data=data)..
-0001e190: 2020 2020 2020 2020 2020 2020 7361 7665              save
-0001e1a0: 6420 3d20 7365 6c66 2e66 696e 6443 7572  d = self.findCur
-0001e1b0: 7265 6e74 5361 7665 6456 616c 7565 2873  rentSavedValue(s
-0001e1c0: 6372 6565 6e44 6963 742c 2073 6176 6544  creenDict, saveD
-0001e1d0: 6963 742c 2022 5061 7474 6572 6e22 290d  ict, "Pattern").
-0001e1e0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0001e1f0: 6c63 2e64 662e 696c 6f63 5b2d 315d 5b22  lc.df.iloc[-1]["
-0001e200: 6973 4e65 7742 7579 5369 676e 616c 225d  isNewBuySignal"]
-0001e210: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0001e220: 2020 2073 6372 6565 6e44 6963 745b 2250     screenDict["P
-0001e230: 6174 7465 726e 225d 203d 2028 0d0a 2020  attern"] = (..  
-0001e240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e250: 2020 7361 7665 645b 305d 202b 2063 6f6c    saved[0] + col
-0001e260: 6f72 5465 7874 2e42 4f4c 4420 2b20 636f  orText.BOLD + co
-0001e270: 6c6f 7254 6578 742e 4752 4545 4e20 2b20  lorText.GREEN + 
-0001e280: 224c 6f72 656e 747a 6961 6e2d 4275 7922  "Lorentzian-Buy"
-0001e290: 202b 2063 6f6c 6f72 5465 7874 2e45 4e44   + colorText.END
-0001e2a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001e2b0: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
-0001e2c0: 2020 2020 2073 6176 6544 6963 745b 2250       saveDict["P
-0001e2d0: 6174 7465 726e 225d 203d 2073 6176 6564  attern"] = saved
-0001e2e0: 5b31 5d20 2b20 224c 6f72 656e 747a 6961  [1] + "Lorentzia
-0001e2f0: 6e2d 4275 7922 0d0a 2020 2020 2020 2020  n-Buy"..        
-0001e300: 2020 2020 2020 2020 6966 206c 6f6f 6b46          if lookF
-0001e310: 6f72 2021 3d20 323a 2023 204e 6f74 2053  or != 2: # Not S
-0001e320: 656c 6c0d 0a20 2020 2020 2020 2020 2020  ell..           
-0001e330: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0001e340: 5472 7565 0d0a 2020 2020 2020 2020 2020  True..          
-0001e350: 2020 656c 6966 206c 632e 6466 2e69 6c6f    elif lc.df.ilo
-0001e360: 635b 2d31 5d5b 2269 734e 6577 5365 6c6c  c[-1]["isNewSell
-0001e370: 5369 676e 616c 225d 3a0d 0a20 2020 2020  Signal"]:..     
-0001e380: 2020 2020 2020 2020 2020 2073 6372 6565             scree
-0001e390: 6e44 6963 745b 2250 6174 7465 726e 225d  nDict["Pattern"]
-0001e3a0: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
-0001e3b0: 2020 2020 2020 2020 2020 7361 7665 645b            saved[
-0001e3c0: 305d 202b 2063 6f6c 6f72 5465 7874 2e42  0] + colorText.B
-0001e3d0: 4f4c 4420 2b20 636f 6c6f 7254 6578 742e  OLD + colorText.
-0001e3e0: 4641 494c 202b 2022 4c6f 7265 6e74 7a69  FAIL + "Lorentzi
-0001e3f0: 616e 2d53 656c 6c22 202b 2063 6f6c 6f72  an-Sell" + color
-0001e400: 5465 7874 2e45 4e44 0d0a 2020 2020 2020  Text.END..      
-0001e410: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
-0001e420: 2020 2020 2020 2020 2020 2020 2073 6176               sav
-0001e430: 6544 6963 745b 2250 6174 7465 726e 225d  eDict["Pattern"]
-0001e440: 203d 2073 6176 6564 5b31 5d20 2b20 224c   = saved[1] + "L
-0001e450: 6f72 656e 747a 6961 6e2d 5365 6c6c 220d  orentzian-Sell".
-0001e460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001e470: 2069 6620 6c6f 6f6b 466f 7220 213d 2031   if lookFor != 1
-0001e480: 3a20 2320 4e6f 7420 4275 790d 0a20 2020  : # Not Buy..   
-0001e490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e4a0: 2072 6574 7572 6e20 5472 7565 0d0a 2020   return True..  
-0001e4b0: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
-0001e4c0: 6570 7469 6f6e 3a20 2023 2070 7261 676d  eption:  # pragm
-0001e4d0: 613a 206e 6f20 636f 7665 720d 0a20 2020  a: no cover..   
-0001e4e0: 2020 2020 2020 2020 2023 2056 616c 7565           # Value
-0001e4f0: 4572 726f 723a 206f 7065 7261 6e64 7320  Error: operands 
-0001e500: 636f 756c 6420 6e6f 7420 6265 2062 726f  could not be bro
-0001e510: 6164 6361 7374 2074 6f67 6574 6865 7220  adcast together 
-0001e520: 7769 7468 2073 6861 7065 7320 2832 302c  with shapes (20,
-0001e530: 2920 2832 362c 290d 0a20 2020 2020 2020  ) (26,)..       
-0001e540: 2020 2020 2023 2046 696c 6520 222f 6f70       # File "/op
-0001e550: 742f 686f 6d65 6272 6577 2f6c 6962 2f70  t/homebrew/lib/p
-0001e560: 7974 686f 6e33 2e31 312f 7369 7465 2d70  ython3.11/site-p
-0001e570: 6163 6b61 6765 732f 6164 7661 6e63 6564  ackages/advanced
-0001e580: 5f74 612f 4c6f 7265 6e74 7a69 616e 436c  _ta/LorentzianCl
-0001e590: 6173 7369 6669 6361 7469 6f6e 2f43 6c61  assification/Cla
-0001e5a0: 7373 6966 6965 722e 7079 222c 206c 696e  ssifier.py", lin
-0001e5b0: 6520 3138 362c 2069 6e20 5f5f 696e 6974  e 186, in __init
-0001e5c0: 5f5f 0d0a 2020 2020 2020 2020 2020 2020  __..            
-0001e5d0: 2320 4669 6c65 2022 2f6f 7074 2f68 6f6d  # File "/opt/hom
-0001e5e0: 6562 7265 772f 6c69 622f 7079 7468 6f6e  ebrew/lib/python
-0001e5f0: 332e 3131 2f73 6974 652d 7061 636b 6167  3.11/site-packag
-0001e600: 6573 2f61 6476 616e 6365 645f 7461 2f4c  es/advanced_ta/L
-0001e610: 6f72 656e 747a 6961 6e43 6c61 7373 6966  orentzianClassif
-0001e620: 6963 6174 696f 6e2f 436c 6173 7369 6669  ication/Classifi
-0001e630: 6572 2e70 7922 2c20 6c69 6e65 2033 3935  er.py", line 395
-0001e640: 2c20 696e 205f 5f63 6c61 7373 6966 790d  , in __classify.
-0001e650: 0a20 2020 2020 2020 2020 2020 2023 2046  .            # F
-0001e660: 696c 6520 222f 6f70 742f 686f 6d65 6272  ile "/opt/homebr
-0001e670: 6577 2f6c 6962 2f70 7974 686f 6e33 2e31  ew/lib/python3.1
-0001e680: 312f 7369 7465 2d70 6163 6b61 6765 732f  1/site-packages/
-0001e690: 7061 6e64 6173 2f63 6f72 652f 6f70 732f  pandas/core/ops/
-0001e6a0: 636f 6d6d 6f6e 2e70 7922 2c20 6c69 6e65  common.py", line
-0001e6b0: 2037 362c 2069 6e20 6e65 775f 6d65 7468   76, in new_meth
-0001e6c0: 6f64 0d0a 2020 2020 2020 2020 2020 2020  od..            
-0001e6d0: 2320 4669 6c65 2022 2f6f 7074 2f68 6f6d  # File "/opt/hom
-0001e6e0: 6562 7265 772f 6c69 622f 7079 7468 6f6e  ebrew/lib/python
-0001e6f0: 332e 3131 2f73 6974 652d 7061 636b 6167  3.11/site-packag
-0001e700: 6573 2f70 616e 6461 732f 636f 7265 2f61  es/pandas/core/a
-0001e710: 7272 6179 6c69 6b65 2e70 7922 2c20 6c69  rraylike.py", li
-0001e720: 6e65 2037 302c 2069 6e20 5f5f 616e 645f  ne 70, in __and_
-0001e730: 5f0d 0a20 2020 2020 2020 2020 2020 2023  _..            #
-0001e740: 2046 696c 6520 222f 6f70 742f 686f 6d65   File "/opt/home
-0001e750: 6272 6577 2f6c 6962 2f70 7974 686f 6e33  brew/lib/python3
-0001e760: 2e31 312f 7369 7465 2d70 6163 6b61 6765  .11/site-package
-0001e770: 732f 7061 6e64 6173 2f63 6f72 652f 7365  s/pandas/core/se
-0001e780: 7269 6573 2e70 7922 2c20 6c69 6e65 2035  ries.py", line 5
-0001e790: 3831 302c 2069 6e20 5f6c 6f67 6963 616c  810, in _logical
-0001e7a0: 5f6d 6574 686f 640d 0a20 2020 2020 2020  _method..       
-0001e7b0: 2020 2020 2023 2046 696c 6520 222f 6f70       # File "/op
-0001e7c0: 742f 686f 6d65 6272 6577 2f6c 6962 2f70  t/homebrew/lib/p
-0001e7d0: 7974 686f 6e33 2e31 312f 7369 7465 2d70  ython3.11/site-p
-0001e7e0: 6163 6b61 6765 732f 7061 6e64 6173 2f63  ackages/pandas/c
-0001e7f0: 6f72 652f 6f70 732f 6172 7261 795f 6f70  ore/ops/array_op
-0001e800: 732e 7079 222c 206c 696e 6520 3435 362c  s.py", line 456,
-0001e810: 2069 6e20 6c6f 6769 6361 6c5f 6f70 0d0a   in logical_op..
-0001e820: 2020 2020 2020 2020 2020 2020 2320 4669              # Fi
-0001e830: 6c65 2022 2f6f 7074 2f68 6f6d 6562 7265  le "/opt/homebre
-0001e840: 772f 6c69 622f 7079 7468 6f6e 332e 3131  w/lib/python3.11
-0001e850: 2f73 6974 652d 7061 636b 6167 6573 2f70  /site-packages/p
-0001e860: 616e 6461 732f 636f 7265 2f6f 7073 2f61  andas/core/ops/a
-0001e870: 7272 6179 5f6f 7073 2e70 7922 2c20 6c69  rray_ops.py", li
-0001e880: 6e65 2033 3634 2c20 696e 206e 615f 6c6f  ne 364, in na_lo
-0001e890: 6769 6361 6c5f 6f70 0d0a 2020 2020 2020  gical_op..      
-0001e8a0: 2020 2020 2020 2320 7365 6c66 2e64 6566        # self.def
-0001e8b0: 6175 6c74 5f6c 6f67 6765 722e 6465 6275  ault_logger.debu
-0001e8c0: 6728 652c 2065 7863 5f69 6e66 6f3d 5472  g(e, exc_info=Tr
-0001e8d0: 7565 290d 0a20 2020 2020 2020 2020 2020  ue)..           
-0001e8e0: 2070 6173 730d 0a20 2020 2020 2020 2072   pass..        r
-0001e8f0: 6574 7572 6e20 4661 6c73 650d 0a0d 0a20  eturn False.... 
-0001e900: 2020 2023 2076 616c 6964 6174 6520 6966     # validate if
-0001e910: 2074 6865 2073 746f 636b 2068 6173 2062   the stock has b
-0001e920: 6565 6e20 6861 7669 6e67 206c 6f77 6572  een having lower
-0001e930: 206c 6f77 732c 206c 6f77 6572 2068 6967   lows, lower hig
-0001e940: 6873 0d0a 2020 2020 6465 6620 7661 6c69  hs..    def vali
-0001e950: 6461 7465 4c6f 7765 7248 6967 6873 4c6f  dateLowerHighsLo
-0001e960: 7765 724c 6f77 7328 7365 6c66 2c20 6466  werLows(self, df
-0001e970: 293a 0d0a 2020 2020 2020 2020 6966 2064  ):..        if d
-0001e980: 6620 6973 204e 6f6e 6520 6f72 206c 656e  f is None or len
-0001e990: 2864 6629 203d 3d20 303a 0d0a 2020 2020  (df) == 0:..    
-0001e9a0: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-0001e9b0: 616c 7365 0d0a 2020 2020 2020 2020 6461  alse..        da
-0001e9c0: 7461 203d 2064 662e 636f 7079 2829 0d0a  ta = df.copy()..
-0001e9d0: 2020 2020 2020 2020 6461 7930 203d 2064          day0 = d
-0001e9e0: 6174 610d 0a20 2020 2020 2020 2064 6179  ata..        day
-0001e9f0: 3120 3d20 6461 7461 5b31 3a5d 0d0a 2020  1 = data[1:]..  
-0001ea00: 2020 2020 2020 6461 7932 203d 2064 6174        day2 = dat
-0001ea10: 615b 323a 5d0d 0a20 2020 2020 2020 2064  a[2:]..        d
-0001ea20: 6179 3320 3d20 6461 7461 5b33 3a5d 0d0a  ay3 = data[3:]..
-0001ea30: 2020 2020 2020 2020 6c6f 7765 7248 6967          lowerHig
-0001ea40: 6873 203d 2028 0d0a 2020 2020 2020 2020  hs = (..        
-0001ea50: 2020 2020 2864 6179 305b 2248 6967 6822      (day0["High"
-0001ea60: 5d2e 696c 6f63 5b30 5d20 3c20 6461 7931  ].iloc[0] < day1
-0001ea70: 5b22 4869 6768 225d 2e69 6c6f 635b 305d  ["High"].iloc[0]
-0001ea80: 290d 0a20 2020 2020 2020 2020 2020 2061  )..            a
-0001ea90: 6e64 2028 6461 7931 5b22 4869 6768 225d  nd (day1["High"]
-0001eaa0: 2e69 6c6f 635b 305d 203c 2064 6179 325b  .iloc[0] < day2[
-0001eab0: 2248 6967 6822 5d2e 696c 6f63 5b30 5d29  "High"].iloc[0])
-0001eac0: 0d0a 2020 2020 2020 2020 2020 2020 616e  ..            an
-0001ead0: 6420 2864 6179 325b 2248 6967 6822 5d2e  d (day2["High"].
-0001eae0: 696c 6f63 5b30 5d20 3c20 6461 7933 5b22  iloc[0] < day3["
-0001eaf0: 4869 6768 225d 2e69 6c6f 635b 305d 290d  High"].iloc[0]).
-0001eb00: 0a20 2020 2020 2020 2029 0d0a 2020 2020  .        )..    
-0001eb10: 2020 2020 6c6f 7765 724c 6f77 7320 3d20      lowerLows = 
-0001eb20: 280d 0a20 2020 2020 2020 2020 2020 2028  (..            (
-0001eb30: 6461 7930 5b22 4c6f 7722 5d2e 696c 6f63  day0["Low"].iloc
-0001eb40: 5b30 5d20 3c20 6461 7931 5b22 4c6f 7722  [0] < day1["Low"
-0001eb50: 5d2e 696c 6f63 5b30 5d29 0d0a 2020 2020  ].iloc[0])..    
-0001eb60: 2020 2020 2020 2020 616e 6420 2864 6179          and (day
-0001eb70: 315b 224c 6f77 225d 2e69 6c6f 635b 305d  1["Low"].iloc[0]
-0001eb80: 203c 2064 6179 325b 224c 6f77 225d 2e69   < day2["Low"].i
-0001eb90: 6c6f 635b 305d 290d 0a20 2020 2020 2020  loc[0])..       
-0001eba0: 2020 2020 2061 6e64 2028 6461 7932 5b22       and (day2["
-0001ebb0: 4c6f 7722 5d2e 696c 6f63 5b30 5d20 3c20  Low"].iloc[0] < 
-0001ebc0: 6461 7933 5b22 4c6f 7722 5d2e 696c 6f63  day3["Low"].iloc
-0001ebd0: 5b30 5d29 0d0a 2020 2020 2020 2020 290d  [0])..        ).
-0001ebe0: 0a20 2020 2020 2020 2068 6967 6865 7252  .        higherR
-0001ebf0: 5349 203d 2028 0d0a 2020 2020 2020 2020  SI = (..        
-0001ec00: 2020 2020 2864 6179 305b 2252 5349 225d      (day0["RSI"]
-0001ec10: 2e69 6c6f 635b 305d 203c 2064 6179 315b  .iloc[0] < day1[
-0001ec20: 2252 5349 225d 2e69 6c6f 635b 305d 290d  "RSI"].iloc[0]).
-0001ec30: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
-0001ec40: 2028 6461 7931 5b22 5253 4922 5d2e 696c   (day1["RSI"].il
-0001ec50: 6f63 5b30 5d20 3c20 6461 7932 5b22 5253  oc[0] < day2["RS
-0001ec60: 4922 5d2e 696c 6f63 5b30 5d29 0d0a 2020  I"].iloc[0])..  
-0001ec70: 2020 2020 2020 2020 2020 616e 6420 2864            and (d
-0001ec80: 6179 325b 2252 5349 225d 2e69 6c6f 635b  ay2["RSI"].iloc[
-0001ec90: 305d 203c 2064 6179 335b 2252 5349 225d  0] < day3["RSI"]
-0001eca0: 2e69 6c6f 635b 305d 290d 0a20 2020 2020  .iloc[0])..     
-0001ecb0: 2020 2020 2020 2061 6e64 2064 6179 305b         and day0[
-0001ecc0: 2252 5349 225d 2e69 6c6f 635b 305d 203e  "RSI"].iloc[0] >
-0001ecd0: 3d20 3530 0d0a 2020 2020 2020 2020 290d  = 50..        ).
-0001ece0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0001ecf0: 6c6f 7765 7248 6967 6873 2061 6e64 206c  lowerHighs and l
-0001ed00: 6f77 6572 4c6f 7773 2061 6e64 2068 6967  owerLows and hig
-0001ed10: 6865 7252 5349 0d0a 0d0a 2020 2020 2320  herRSI....    # 
-0001ed20: 5661 6c69 6461 7465 2069 6620 7265 6365  Validate if rece
-0001ed30: 6e74 2076 6f6c 756d 6520 6973 206c 6f77  nt volume is low
-0001ed40: 6573 7420 6f66 206c 6173 7420 274e 2720  est of last 'N' 
-0001ed50: 4461 7973 0d0a 2020 2020 6465 6620 7661  Days..    def va
-0001ed60: 6c69 6461 7465 4c6f 7765 7374 566f 6c75  lidateLowestVolu
-0001ed70: 6d65 2873 656c 662c 2064 662c 2064 6179  me(self, df, day
-0001ed80: 7346 6f72 4c6f 7765 7374 566f 6c75 6d65  sForLowestVolume
-0001ed90: 293a 0d0a 2020 2020 2020 2020 6966 2064  ):..        if d
-0001eda0: 6620 6973 204e 6f6e 6520 6f72 206c 656e  f is None or len
-0001edb0: 2864 6629 203d 3d20 303a 0d0a 2020 2020  (df) == 0:..    
-0001edc0: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-0001edd0: 616c 7365 0d0a 2020 2020 2020 2020 6461  alse..        da
-0001ede0: 7461 203d 2064 662e 636f 7079 2829 0d0a  ta = df.copy()..
-0001edf0: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
-0001ee00: 6174 612e 6669 6c6c 6e61 2830 290d 0a20  ata.fillna(0).. 
-0001ee10: 2020 2020 2020 2064 6174 6120 3d20 6461         data = da
-0001ee20: 7461 2e72 6570 6c61 6365 285b 6e70 2e69  ta.replace([np.i
-0001ee30: 6e66 2c20 2d6e 702e 696e 665d 2c20 3029  nf, -np.inf], 0)
-0001ee40: 0d0a 2020 2020 2020 2020 6966 2064 6179  ..        if day
-0001ee50: 7346 6f72 4c6f 7765 7374 566f 6c75 6d65  sForLowestVolume
-0001ee60: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
-0001ee70: 2020 2020 2020 2064 6179 7346 6f72 4c6f         daysForLo
-0001ee80: 7765 7374 566f 6c75 6d65 203d 2033 300d  westVolume = 30.
-0001ee90: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
-0001eea0: 6461 7461 2920 3c20 6461 7973 466f 724c  data) < daysForL
-0001eeb0: 6f77 6573 7456 6f6c 756d 653a 0d0a 2020  owestVolume:..  
-0001eec0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0001eed0: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
-0001eee0: 6461 7461 203d 2064 6174 612e 6865 6164  data = data.head
-0001eef0: 2864 6179 7346 6f72 4c6f 7765 7374 566f  (daysForLowestVo
-0001ef00: 6c75 6d65 290d 0a20 2020 2020 2020 2072  lume)..        r
-0001ef10: 6563 656e 7420 3d20 6461 7461 2e68 6561  ecent = data.hea
-0001ef20: 6428 3129 0d0a 2020 2020 2020 2020 6966  d(1)..        if
-0001ef30: 206c 656e 2872 6563 656e 7429 203c 2031   len(recent) < 1
-0001ef40: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-0001ef50: 6574 7572 6e20 4661 6c73 650d 0a20 2020  eturn False..   
-0001ef60: 2020 2020 2069 6620 2872 6563 656e 745b       if (recent[
-0001ef70: 2256 6f6c 756d 6522 5d2e 696c 6f63 5b30  "Volume"].iloc[0
-0001ef80: 5d20 3c3d 2064 6174 612e 6465 7363 7269  ] <= data.descri
-0001ef90: 6265 2829 5b22 566f 6c75 6d65 225d 5b22  be()["Volume"]["
-0001efa0: 6d69 6e22 5d29 2061 6e64 2072 6563 656e  min"]) and recen
-0001efb0: 745b 0d0a 2020 2020 2020 2020 2020 2020  t[..            
-0001efc0: 2256 6f6c 756d 6522 0d0a 2020 2020 2020  "Volume"..      
-0001efd0: 2020 5d5b 305d 2021 3d20 6e70 2e6e 616e    ][0] != np.nan
-0001efe0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-0001eff0: 6574 7572 6e20 5472 7565 0d0a 2020 2020  eturn True..    
-0001f000: 2020 2020 7265 7475 726e 2046 616c 7365      return False
-0001f010: 0d0a 0d0a 2020 2020 2320 5661 6c69 6461  ....    # Valida
-0001f020: 7465 204c 5450 2077 6974 6869 6e20 6c69  te LTP within li
-0001f030: 6d69 7473 0d0a 2020 2020 6465 6620 7661  mits..    def va
-0001f040: 6c69 6461 7465 4c54 5028 7365 6c66 2c20  lidateLTP(self, 
-0001f050: 6466 2c20 7363 7265 656e 4469 6374 2c20  df, screenDict, 
-0001f060: 7361 7665 4469 6374 2c20 6d69 6e4c 5450  saveDict, minLTP
-0001f070: 3d4e 6f6e 652c 206d 6178 4c54 503d 4e6f  =None, maxLTP=No
-0001f080: 6e65 2c6d 696e 4368 616e 6765 3d30 293a  ne,minChange=0):
-0001f090: 0d0a 2020 2020 2020 2020 6461 7461 203d  ..        data =
-0001f0a0: 2064 662e 636f 7079 2829 0d0a 2020 2020   df.copy()..    
-0001f0b0: 2020 2020 6c74 7056 616c 6964 203d 2046      ltpValid = F
-0001f0c0: 616c 7365 0d0a 2020 2020 2020 2020 6966  alse..        if
-0001f0d0: 206d 696e 4c54 5020 6973 204e 6f6e 653a   minLTP is None:
-0001f0e0: 0d0a 2020 2020 2020 2020 2020 2020 6d69  ..            mi
-0001f0f0: 6e4c 5450 203d 2073 656c 662e 636f 6e66  nLTP = self.conf
-0001f100: 6967 4d61 6e61 6765 722e 6d69 6e4c 5450  igManager.minLTP
-0001f110: 0d0a 2020 2020 2020 2020 6966 206d 6178  ..        if max
-0001f120: 4c54 5020 6973 204e 6f6e 653a 0d0a 2020  LTP is None:..  
-0001f130: 2020 2020 2020 2020 2020 6d61 784c 5450            maxLTP
-0001f140: 203d 2073 656c 662e 636f 6e66 6967 4d61   = self.configMa
-0001f150: 6e61 6765 722e 6d61 784c 5450 0d0a 2020  nager.maxLTP..  
-0001f160: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
-0001f170: 612e 6669 6c6c 6e61 2830 290d 0a20 2020  a.fillna(0)..   
-0001f180: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
-0001f190: 2e72 6570 6c61 6365 285b 6e70 2e69 6e66  .replace([np.inf
-0001f1a0: 2c20 2d6e 702e 696e 665d 2c20 3029 0d0a  , -np.inf], 0)..
-0001f1b0: 2020 2020 2020 2020 7265 6365 6e74 203d          recent =
-0001f1c0: 2064 6174 612e 6865 6164 2831 290d 0a0d   data.head(1)...
-0001f1d0: 0a20 2020 2020 2020 2070 6374 5f63 6861  .        pct_cha
-0001f1e0: 6e67 6520 3d20 2864 6174 615b 3a3a 2d31  nge = (data[::-1
-0001f1f0: 5d5b 2243 6c6f 7365 225d 2e70 6374 5f63  ]["Close"].pct_c
-0001f200: 6861 6e67 6528 2920 2a20 3130 3029 2e69  hange() * 100).i
-0001f210: 6c6f 635b 2d31 5d0d 0a20 2020 2020 2020  loc[-1]..       
-0001f220: 2069 6620 7063 745f 6368 616e 6765 203d   if pct_change =
-0001f230: 3d20 6e70 2e69 6e66 206f 7220 7063 745f  = np.inf or pct_
-0001f240: 6368 616e 6765 203d 3d20 2d6e 702e 696e  change == -np.in
-0001f250: 663a 0d0a 2020 2020 2020 2020 2020 2020  f:..            
-0001f260: 7063 745f 6368 616e 6765 203d 2030 0d0a  pct_change = 0..
-0001f270: 2020 2020 2020 2020 7063 745f 7361 7665          pct_save
-0001f280: 203d 2022 252e 3166 2525 2220 2520 7063   = "%.1f%%" % pc
-0001f290: 745f 6368 616e 6765 0d0a 2020 2020 2020  t_change..      
-0001f2a0: 2020 6966 2070 6374 5f63 6861 6e67 6520    if pct_change 
-0001f2b0: 3e20 302e 323a 0d0a 2020 2020 2020 2020  > 0.2:..        
-0001f2c0: 2020 2020 7063 745f 6368 616e 6765 203d      pct_change =
-0001f2d0: 2063 6f6c 6f72 5465 7874 2e47 5245 454e   colorText.GREEN
-0001f2e0: 202b 2028 2225 2e31 6625 2522 2025 2070   + ("%.1f%%" % p
-0001f2f0: 6374 5f63 6861 6e67 6529 202b 2063 6f6c  ct_change) + col
-0001f300: 6f72 5465 7874 2e45 4e44 0d0a 2020 2020  orText.END..    
-0001f310: 2020 2020 656c 6966 2070 6374 5f63 6861      elif pct_cha
-0001f320: 6e67 6520 3c20 2d30 2e32 3a0d 0a20 2020  nge < -0.2:..   
-0001f330: 2020 2020 2020 2020 2070 6374 5f63 6861           pct_cha
-0001f340: 6e67 6520 3d20 636f 6c6f 7254 6578 742e  nge = colorText.
-0001f350: 4641 494c 202b 2028 2225 2e31 6625 2522  FAIL + ("%.1f%%"
-0001f360: 2025 2070 6374 5f63 6861 6e67 6529 202b   % pct_change) +
-0001f370: 2063 6f6c 6f72 5465 7874 2e45 4e44 0d0a   colorText.END..
-0001f380: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-0001f390: 2020 2020 2020 2020 2020 2070 6374 5f63             pct_c
-0001f3a0: 6861 6e67 6520 3d20 636f 6c6f 7254 6578  hange = colorTex
-0001f3b0: 742e 5741 524e 202b 2028 2225 2e31 6625  t.WARN + ("%.1f%
-0001f3c0: 2522 2025 2070 6374 5f63 6861 6e67 6529  %" % pct_change)
-0001f3d0: 202b 2063 6f6c 6f72 5465 7874 2e45 4e44   + colorText.END
-0001f3e0: 0d0a 2020 2020 2020 2020 7361 7665 4469  ..        saveDi
-0001f3f0: 6374 5b22 2543 686e 6722 5d20 3d20 7063  ct["%Chng"] = pc
-0001f400: 745f 7361 7665 0d0a 2020 2020 2020 2020  t_save..        
-0001f410: 7363 7265 656e 4469 6374 5b22 2543 686e  screenDict["%Chn
-0001f420: 6722 5d20 3d20 7063 745f 6368 616e 6765  g"] = pct_change
-0001f430: 0d0a 2020 2020 2020 2020 6c74 7020 3d20  ..        ltp = 
-0001f440: 726f 756e 6428 7265 6365 6e74 5b22 436c  round(recent["Cl
-0001f450: 6f73 6522 5d2e 696c 6f63 5b30 5d2c 2032  ose"].iloc[0], 2
-0001f460: 290d 0a20 2020 2020 2020 2076 6572 6966  )..        verif
-0001f470: 7953 7461 6765 5477 6f20 3d20 5472 7565  yStageTwo = True
-0001f480: 0d0a 2020 2020 2020 2020 6966 206c 656e  ..        if len
-0001f490: 2864 6174 6129 203e 2032 3530 3a0d 0a20  (data) > 250:.. 
-0001f4a0: 2020 2020 2020 2020 2020 2079 6561 726c             yearl
-0001f4b0: 794c 6f77 203d 2064 6174 612e 6865 6164  yLow = data.head
-0001f4c0: 2832 3530 295b 2243 6c6f 7365 225d 2e6d  (250)["Close"].m
-0001f4d0: 696e 2829 0d0a 2020 2020 2020 2020 2020  in()..          
-0001f4e0: 2020 7965 6172 6c79 4869 6768 203d 2064    yearlyHigh = d
-0001f4f0: 6174 612e 6865 6164 2832 3530 295b 2243  ata.head(250)["C
-0001f500: 6c6f 7365 225d 2e6d 6178 2829 0d0a 2020  lose"].max()..  
-0001f510: 2020 2020 2020 2020 2020 6966 206c 7470            if ltp
-0001f520: 203c 2028 3220 2a20 7965 6172 6c79 4c6f   < (2 * yearlyLo
-0001f530: 7729 2061 6e64 206c 7470 203c 2028 302e  w) and ltp < (0.
-0001f540: 3735 202a 2079 6561 726c 7948 6967 6829  75 * yearlyHigh)
-0001f550: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0001f560: 2020 2076 6572 6966 7953 7461 6765 5477     verifyStageTw
-0001f570: 6f20 3d20 4661 6c73 650d 0a20 2020 2020  o = False..     
-0001f580: 2020 2020 2020 2020 2020 2073 6372 6565             scree
-0001f590: 6e44 6963 745b 2253 746f 636b 225d 203d  nDict["Stock"] =
-0001f5a0: 2063 6f6c 6f72 5465 7874 2e46 4149 4c20   colorText.FAIL 
-0001f5b0: 2b20 7361 7665 4469 6374 5b22 5374 6f63  + saveDict["Stoc
-0001f5c0: 6b22 5d20 2b20 636f 6c6f 7254 6578 742e  k"] + colorText.
-0001f5d0: 454e 440d 0a20 2020 2020 2020 2069 6620  END..        if 
-0001f5e0: 6c74 7020 3e3d 206d 696e 4c54 5020 616e  ltp >= minLTP an
-0001f5f0: 6420 6c74 7020 3c3d 206d 6178 4c54 503a  d ltp <= maxLTP:
-0001f600: 0d0a 2020 2020 2020 2020 2020 2020 6c74  ..            lt
-0001f610: 7056 616c 6964 203d 2054 7275 650d 0a20  pValid = True.. 
-0001f620: 2020 2020 2020 2020 2020 2069 6620 6d69             if mi
-0001f630: 6e43 6861 6e67 6520 213d 2030 3a0d 0a20  nChange != 0:.. 
-0001f640: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0001f650: 2055 7365 7220 6861 7320 7375 7070 6c69   User has suppli
-0001f660: 6564 2073 6f6d 6520 6669 6c74 6572 2066  ed some filter f
-0001f670: 6f72 2070 6572 6365 6e74 6167 6520 6368  or percentage ch
-0001f680: 616e 6765 0d0a 2020 2020 2020 2020 2020  ange..          
-0001f690: 2020 2020 2020 6c74 7056 616c 6964 203d        ltpValid =
-0001f6a0: 2066 6c6f 6174 2873 7472 2870 6374 5f73   float(str(pct_s
-0001f6b0: 6176 6529 2e72 6570 6c61 6365 2822 2522  ave).replace("%"
-0001f6c0: 2c22 2229 2920 3e3d 206d 696e 4368 616e  ,"")) >= minChan
-0001f6d0: 6765 0d0a 2020 2020 2020 2020 2020 2020  ge..            
-0001f6e0: 7361 7665 4469 6374 5b22 4c54 5022 5d20  saveDict["LTP"] 
-0001f6f0: 3d20 726f 756e 6428 6c74 702c 2032 290d  = round(ltp, 2).
-0001f700: 0a20 2020 2020 2020 2020 2020 2073 6372  .            scr
-0001f710: 6565 6e44 6963 745b 224c 5450 225d 203d  eenDict["LTP"] =
-0001f720: 2028 636f 6c6f 7254 6578 742e 4752 4545   (colorText.GREE
-0001f730: 4e20 6966 206c 7470 5661 6c69 6420 656c  N if ltpValid el
-0001f740: 7365 2063 6f6c 6f72 5465 7874 2e46 4149  se colorText.FAI
-0001f750: 4c29 202b 2028 2225 2e32 6622 2025 206c  L) + ("%.2f" % l
-0001f760: 7470 2920 2b20 636f 6c6f 7254 6578 742e  tp) + colorText.
-0001f770: 454e 440d 0a20 2020 2020 2020 2020 2020  END..           
-0001f780: 2072 6574 7572 6e20 6c74 7056 616c 6964   return ltpValid
-0001f790: 2c20 7665 7269 6679 5374 6167 6554 776f  , verifyStageTwo
-0001f7a0: 0d0a 2020 2020 2020 2020 7363 7265 656e  ..        screen
-0001f7b0: 4469 6374 5b22 4c54 5022 5d20 3d20 636f  Dict["LTP"] = co
-0001f7c0: 6c6f 7254 6578 742e 4641 494c 202b 2028  lorText.FAIL + (
-0001f7d0: 2225 2e32 6622 2025 206c 7470 2920 2b20  "%.2f" % ltp) + 
-0001f7e0: 636f 6c6f 7254 6578 742e 454e 440d 0a20  colorText.END.. 
-0001f7f0: 2020 2020 2020 2073 6176 6544 6963 745b         saveDict[
-0001f800: 224c 5450 225d 203d 2072 6f75 6e64 286c  "LTP"] = round(l
-0001f810: 7470 2c20 3229 0d0a 2020 2020 2020 2020  tp, 2)..        
-0001f820: 7265 7475 726e 206c 7470 5661 6c69 642c  return ltpValid,
-0001f830: 2076 6572 6966 7953 7461 6765 5477 6f0d   verifyStageTwo.
-0001f840: 0a0d 0a20 2020 2064 6566 2076 616c 6964  ...    def valid
-0001f850: 6174 654c 5450 466f 7250 6f72 7466 6f6c  ateLTPForPortfol
-0001f860: 696f 4361 6c63 2873 656c 662c 2064 662c  ioCalc(self, df,
-0001f870: 2073 6372 6565 6e44 6963 742c 2073 6176   screenDict, sav
-0001f880: 6544 6963 742c 7265 7175 6573 7465 6450  eDict,requestedP
-0001f890: 6572 696f 643d 3029 3a0d 0a20 2020 2020  eriod=0):..     
-0001f8a0: 2020 2064 6174 6120 3d20 6466 2e63 6f70     data = df.cop
-0001f8b0: 7928 290d 0a20 2020 2020 2020 2070 6572  y()..        per
-0001f8c0: 696f 6473 203d 2073 656c 662e 636f 6e66  iods = self.conf
-0001f8d0: 6967 4d61 6e61 6765 722e 7065 7269 6f64  igManager.period
-0001f8e0: 7352 616e 6765 0d0a 2020 2020 2020 2020  sRange..        
-0001f8f0: 6966 2072 6571 7565 7374 6564 5065 7269  if requestedPeri
-0001f900: 6f64 203e 2030 2061 6e64 2072 6571 7565  od > 0 and reque
-0001f910: 7374 6564 5065 7269 6f64 206e 6f74 2069  stedPeriod not i
-0001f920: 6e20 7065 7269 6f64 733a 0d0a 2020 2020  n periods:..    
-0001f930: 2020 2020 2020 2020 7065 7269 6f64 732e          periods.
-0001f940: 6170 7065 6e64 2872 6571 7565 7374 6564  append(requested
-0001f950: 5065 7269 6f64 290d 0a20 2020 2020 2020  Period)..       
-0001f960: 2070 7265 7669 6f75 735f 7265 6365 6e74   previous_recent
-0001f970: 203d 2064 6174 612e 6865 6164 2831 290d   = data.head(1).
-0001f980: 0a20 2020 2020 2020 2070 7265 7669 6f75  .        previou
-0001f990: 735f 7265 6365 6e74 2e72 6573 6574 5f69  s_recent.reset_i
-0001f9a0: 6e64 6578 2869 6e70 6c61 6365 3d54 7275  ndex(inplace=Tru
-0001f9b0: 6529 0d0a 2020 2020 2020 2020 6361 6c63  e)..        calc
-0001f9c0: 5f64 6174 6520 3d20 7374 7228 7072 6576  _date = str(prev
-0001f9d0: 696f 7573 5f72 6563 656e 742e 696c 6f63  ious_recent.iloc
-0001f9e0: 5b3a 2c20 305d 5b30 5d29 2e73 706c 6974  [:, 0][0]).split
-0001f9f0: 2822 2022 295b 305d 0d0a 2020 2020 2020  (" ")[0]..      
-0001fa00: 2020 666f 7220 7072 6420 696e 2070 6572    for prd in per
-0001fa10: 696f 6473 3a0d 0a20 2020 2020 2020 2020  iods:..         
-0001fa20: 2020 2069 6620 6c65 6e28 6461 7461 2920     if len(data) 
-0001fa30: 3e3d 2070 7264 202b 2031 3a0d 0a20 2020  >= prd + 1:..   
-0001fa40: 2020 2020 2020 2020 2020 2020 2070 7265               pre
-0001fa50: 764c 7470 203d 2064 6174 615b 2243 6c6f  vLtp = data["Clo
-0001fa60: 7365 225d 2e69 6c6f 635b 305d 0d0a 2020  se"].iloc[0]..  
-0001fa70: 2020 2020 2020 2020 2020 2020 2020 6c74                lt
-0001fa80: 7054 6479 203d 2064 6174 615b 2243 6c6f  pTdy = data["Clo
-0001fa90: 7365 225d 2e69 6c6f 635b 7072 645d 0d0a  se"].iloc[prd]..
-0001faa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fab0: 6966 2069 7369 6e73 7461 6e63 6528 7072  if isinstance(pr
-0001fac0: 6576 4c74 702c 7064 2e53 6572 6965 7329  evLtp,pd.Series)
-0001fad0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0001fae0: 2020 2020 2020 2070 7265 764c 7470 203d         prevLtp =
-0001faf0: 2070 7265 764c 7470 5b30 5d0d 0a20 2020   prevLtp[0]..   
-0001fb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fb10: 206c 7470 5464 7920 3d20 6c74 7054 6479   ltpTdy = ltpTdy
-0001fb20: 5b30 5d0d 0a20 2020 2020 2020 2020 2020  [0]..           
-0001fb30: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
-0001fb40: 6622 4c54 507b 7072 647d 225d 203d 2028  f"LTP{prd}"] = (
-0001fb50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001fb60: 2020 2020 2020 2863 6f6c 6f72 5465 7874        (colorText
-0001fb70: 2e47 5245 454e 2069 6620 286c 7470 5464  .GREEN if (ltpTd
-0001fb80: 7920 3e3d 2070 7265 764c 7470 2920 656c  y >= prevLtp) el
-0001fb90: 7365 2028 636f 6c6f 7254 6578 742e 4641  se (colorText.FA
-0001fba0: 494c 2929 0d0a 2020 2020 2020 2020 2020  IL))..          
-0001fbb0: 2020 2020 2020 2020 2020 2b20 7374 7228            + str(
-0001fbc0: 227b 3a2e 3266 7d22 2e66 6f72 6d61 7428  "{:.2f}".format(
-0001fbd0: 6c74 7054 6479 2929 0d0a 2020 2020 2020  ltpTdy))..      
-0001fbe0: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-0001fbf0: 636f 6c6f 7254 6578 742e 454e 440d 0a20  colorText.END.. 
-0001fc00: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0001fc10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001fc20: 2020 7363 7265 656e 4469 6374 5b66 2247    screenDict[f"G
-0001fc30: 726f 7774 687b 7072 647d 225d 203d 2028  rowth{prd}"] = (
-0001fc40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001fc50: 2020 2020 2020 2863 6f6c 6f72 5465 7874        (colorText
-0001fc60: 2e47 5245 454e 2069 6620 286c 7470 5464  .GREEN if (ltpTd
-0001fc70: 7920 3e3d 2070 7265 764c 7470 2920 656c  y >= prevLtp) el
-0001fc80: 7365 2028 636f 6c6f 7254 6578 742e 4641  se (colorText.FA
-0001fc90: 494c 2929 0d0a 2020 2020 2020 2020 2020  IL))..          
-0001fca0: 2020 2020 2020 2020 2020 2b20 7374 7228            + str(
-0001fcb0: 227b 3a2e 3266 7d22 2e66 6f72 6d61 7428  "{:.2f}".format(
-0001fcc0: 6c74 7054 6479 202d 2070 7265 764c 7470  ltpTdy - prevLtp
-0001fcd0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-0001fce0: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
-0001fcf0: 6578 742e 454e 440d 0a20 2020 2020 2020  ext.END..       
-0001fd00: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
-0001fd10: 2020 2020 2020 2020 2020 2020 7361 7665              save
-0001fd20: 4469 6374 5b66 224c 5450 7b70 7264 7d22  Dict[f"LTP{prd}"
-0001fd30: 5d20 3d20 726f 756e 6428 6c74 7054 6479  ] = round(ltpTdy
-0001fd40: 2c20 3229 0d0a 2020 2020 2020 2020 2020  , 2)..          
-0001fd50: 2020 2020 2020 7361 7665 4469 6374 5b66        saveDict[f
-0001fd60: 2247 726f 7774 687b 7072 647d 225d 203d  "Growth{prd}"] =
-0001fd70: 2072 6f75 6e64 286c 7470 5464 7920 2d20   round(ltpTdy - 
-0001fd80: 7072 6576 4c74 702c 2032 290d 0a20 2020  prevLtp, 2)..   
-0001fd90: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0001fda0: 7072 6420 3d3d 2032 3220 6f72 2028 7072  prd == 22 or (pr
-0001fdb0: 6420 3d3d 2072 6571 7565 7374 6564 5065  d == requestedPe
-0001fdc0: 7269 6f64 293a 0d0a 2020 2020 2020 2020  riod):..        
-0001fdd0: 2020 2020 2020 2020 2020 2020 6368 616e              chan
-0001fde0: 6765 5065 7263 656e 7420 3d20 726f 756e  gePercent = roun
-0001fdf0: 6428 2828 7072 6576 4c74 702d 6c74 7054  d(((prevLtp-ltpT
-0001fe00: 6479 2920 6966 2072 6571 7565 7374 6564  dy) if requested
-0001fe10: 5065 7269 6f64 203d 3d30 2065 6c73 6520  Period ==0 else 
-0001fe20: 286c 7470 5464 7920 2d20 7072 6576 4c74  (ltpTdy - prevLt
-0001fe30: 7029 292a 3130 302f 6c74 7054 6479 2c20  p))*100/ltpTdy, 
-0001fe40: 3229 0d0a 2020 2020 2020 2020 2020 2020  2)..            
-0001fe50: 2020 2020 2020 2020 7361 7665 4469 6374          saveDict
-0001fe60: 5b66 227b 7072 647d 2d50 6420 2522 5d20  [f"{prd}-Pd %"] 
-0001fe70: 3d20 6622 7b63 6861 6e67 6550 6572 6365  = f"{changePerce
-0001fe80: 6e74 7d25 220d 0a20 2020 2020 2020 2020  nt}%"..         
-0001fe90: 2020 2020 2020 2020 2020 2073 6372 6565             scree
-0001fea0: 6e44 6963 745b 6622 7b70 7264 7d2d 5064  nDict[f"{prd}-Pd
-0001feb0: 2025 225d 203d 2028 636f 6c6f 7254 6578   %"] = (colorTex
-0001fec0: 742e 4752 4545 4e20 6966 2063 6861 6e67  t.GREEN if chang
-0001fed0: 6550 6572 6365 6e74 203e 3d30 2065 6c73  ePercent >=0 els
-0001fee0: 6520 636f 6c6f 7254 6578 742e 4641 494c  e colorText.FAIL
-0001fef0: 2920 2b20 6622 7b63 6861 6e67 6550 6572  ) + f"{changePer
-0001ff00: 6365 6e74 7d25 2220 2b20 636f 6c6f 7254  cent}%" + colorT
-0001ff10: 6578 742e 454e 440d 0a20 2020 2020 2020  ext.END..       
-0001ff20: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
-0001ff30: 6963 745b 2244 6174 6522 5d20 3d20 6361  ict["Date"] = ca
-0001ff40: 6c63 5f64 6174 650d 0a20 2020 2020 2020  lc_date..       
-0001ff50: 2020 2020 2020 2020 2073 6176 6544 6963           saveDic
-0001ff60: 745b 2244 6174 6522 5d20 3d20 6361 6c63  t["Date"] = calc
-0001ff70: 5f64 6174 650d 0a20 2020 2020 2020 2020  _date..         
-0001ff80: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-0001ff90: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
-0001ffa0: 6374 5b66 224c 5450 7b70 7264 7d22 5d20  ct[f"LTP{prd}"] 
-0001ffb0: 3d20 6e70 2e6e 616e 0d0a 2020 2020 2020  = np.nan..      
-0001ffc0: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
-0001ffd0: 6374 5b66 2247 726f 7774 687b 7072 647d  ct[f"Growth{prd}
-0001ffe0: 225d 203d 206e 702e 6e61 6e0d 0a20 2020  "] = np.nan..   
-0001fff0: 2020 2020 2020 2020 2020 2020 2073 6372               scr
-00020000: 6565 6e44 6963 745b 2244 6174 6522 5d20  eenDict["Date"] 
-00020010: 3d20 6361 6c63 5f64 6174 650d 0a20 2020  = calc_date..   
-00020020: 2020 2020 2020 2020 2020 2020 2073 6176               sav
-00020030: 6544 6963 745b 2244 6174 6522 5d20 3d20  eDict["Date"] = 
-00020040: 6361 6c63 5f64 6174 650d 0a0d 0a20 2020  calc_date....   
-00020050: 2023 2046 696e 6420 7374 6f63 6b73 2074   # Find stocks t
-00020060: 6861 7420 6172 6520 6265 6172 6973 6820  hat are bearish 
-00020070: 696e 7472 6164 6179 3a20 4d61 6364 2048  intraday: Macd H
-00020080: 6973 746f 6772 616d 206e 6567 6174 6976  istogram negativ
-00020090: 650d 0a20 2020 2064 6566 2076 616c 6964  e..    def valid
-000200a0: 6174 654d 4143 4448 6973 746f 6772 616d  ateMACDHistogram
-000200b0: 4265 6c6f 7730 2873 656c 662c 2064 6629  Below0(self, df)
-000200c0: 3a0d 0a20 2020 2020 2020 2069 6620 6466  :..        if df
-000200d0: 2069 7320 4e6f 6e65 206f 7220 6c65 6e28   is None or len(
-000200e0: 6466 2920 3d3d 2030 3a0d 0a20 2020 2020  df) == 0:..     
-000200f0: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-00020100: 6c73 650d 0a20 2020 2020 2020 2064 6174  lse..        dat
-00020110: 6120 3d20 6466 2e63 6f70 7928 290d 0a20  a = df.copy().. 
-00020120: 2020 2020 2020 2064 6174 6120 3d20 6461         data = da
-00020130: 7461 2e66 696c 6c6e 6128 3029 0d0a 2020  ta.fillna(0)..  
-00020140: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
-00020150: 612e 7265 706c 6163 6528 5b6e 702e 696e  a.replace([np.in
-00020160: 662c 202d 6e70 2e69 6e66 5d2c 2030 290d  f, -np.inf], 0).
-00020170: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
-00020180: 6461 7461 5b3a 3a2d 315d 2020 2320 5265  data[::-1]  # Re
-00020190: 7665 7273 6520 7468 6520 6461 7461 6672  verse the datafr
-000201a0: 616d 6520 736f 2074 6861 7420 6974 7320  ame so that its 
-000201b0: 7468 6520 6f6c 6465 7374 2064 6174 6520  the oldest date 
-000201c0: 6669 7273 740d 0a20 2020 2020 2020 206d  first..        m
-000201d0: 6163 6420 3d20 706b 7461 6c69 622e 4d41  acd = pktalib.MA
-000201e0: 4344 2864 6174 615b 2243 6c6f 7365 225d  CD(data["Close"]
-000201f0: 2c20 3132 2c20 3236 2c20 3929 5b32 5d2e  , 12, 26, 9)[2].
-00020200: 7461 696c 2831 290d 0a20 2020 2020 2020  tail(1)..       
-00020210: 2072 6574 7572 6e20 6d61 6364 2e69 6c6f   return macd.ilo
-00020220: 635b 3a31 5d5b 305d 203c 2030 0d0a 0d0a  c[:1][0] < 0....
-00020230: 2020 2020 2340 6d65 6173 7572 655f 7469      #@measure_ti
-00020240: 6d65 0d0a 2020 2020 2320 4669 6e64 2069  me..    # Find i
-00020250: 6620 7374 6f63 6b20 6761 696e 696e 6720  f stock gaining 
-00020260: 6275 6c6c 6973 6820 6d6f 6d65 6e74 756d  bullish momentum
-00020270: 0d0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
-00020280: 7465 4d6f 6d65 6e74 756d 2873 656c 662c  teMomentum(self,
-00020290: 2064 662c 2073 6372 6565 6e44 6963 742c   df, screenDict,
-000202a0: 2073 6176 6544 6963 7429 3a0d 0a20 2020   saveDict):..   
-000202b0: 2020 2020 2069 6620 6466 2069 7320 4e6f       if df is No
-000202c0: 6e65 206f 7220 6c65 6e28 6466 2920 3d3d  ne or len(df) ==
-000202d0: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
-000202e0: 2072 6574 7572 6e20 4661 6c73 650d 0a20   return False.. 
-000202f0: 2020 2020 2020 2064 6174 6120 3d20 6466         data = df
-00020300: 2e63 6f70 7928 290d 0a20 2020 2020 2020  .copy()..       
-00020310: 2074 7279 3a0d 0a20 2020 2020 2020 2020   try:..         
-00020320: 2020 2064 6174 6120 3d20 6461 7461 2e68     data = data.h
-00020330: 6561 6428 3329 0d0a 2020 2020 2020 2020  ead(3)..        
-00020340: 2020 2020 6966 206c 656e 2864 6174 6129      if len(data)
-00020350: 203c 2033 3a0d 0a20 2020 2020 2020 2020   < 3:..         
-00020360: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-00020370: 6c73 650d 0a20 2020 2020 2020 2020 2020  lse..           
-00020380: 2066 6f72 2072 6f77 2069 6e20 6461 7461   for row in data
-00020390: 2e69 7465 7272 6f77 7328 293a 0d0a 2020  .iterrows():..  
-000203a0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-000203b0: 416c 6c20 3320 6361 6e64 6c65 7320 7368  All 3 candles sh
-000203c0: 6f75 6c64 2062 6520 4772 6565 6e20 616e  ould be Green an
-000203d0: 6420 4e4f 5420 4369 7263 7569 7473 0d0a  d NOT Circuits..
-000203e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000203f0: 7963 203d 2072 6f77 5b31 5d5b 2243 6c6f  yc = row[1]["Clo
-00020400: 7365 225d 0d0a 2020 2020 2020 2020 2020  se"]..          
-00020410: 2020 2020 2020 796f 203d 2072 6f77 5b31        yo = row[1
-00020420: 5d5b 224f 7065 6e22 5d0d 0a20 2020 2020  ]["Open"]..     
-00020430: 2020 2020 2020 2020 2020 2069 6620 7963             if yc
-00020440: 203c 3d20 796f 3a0d 0a20 2020 2020 2020   <= yo:..       
-00020450: 2020 2020 2020 2020 2020 2020 2023 2073               # s
-00020460: 656c 662e 6465 6661 756c 745f 6c6f 6767  elf.default_logg
-00020470: 6572 2e69 6e66 6f28 0d0a 2020 2020 2020  er.info(..      
-00020480: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00020490: 2020 2020 6627 5374 6f63 6b3a 7b73 6176      f'Stock:{sav
-000204a0: 6544 6963 745b 2253 746f 636b 225d 7d2c  eDict["Stock"]},
-000204b0: 2069 7320 6e6f 7420 6120 6d6f 6d65 6e74   is not a moment
-000204c0: 756d 2d67 6169 6e65 7220 6265 6361 7573  um-gainer becaus
-000204d0: 6520 7965 7374 6572 6461 792d 636c 6f73  e yesterday-clos
-000204e0: 6520 287b 7963 7d29 203c 3d20 7965 7374  e ({yc}) <= yest
-000204f0: 6572 6461 792d 6f70 656e 2028 7b79 6f7d  erday-open ({yo}
-00020500: 2927 0d0a 2020 2020 2020 2020 2020 2020  )'..            
-00020510: 2020 2020 2020 2020 2320 290d 0a20 2020          # )..   
-00020520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020530: 2072 6574 7572 6e20 4661 6c73 650d 0a20   return False.. 
-00020540: 2020 2020 2020 2020 2020 206f 7065 6e44             openD
-00020550: 6573 6320 3d20 6461 7461 2e73 6f72 745f  esc = data.sort_
-00020560: 7661 6c75 6573 2862 793d 5b22 4f70 656e  values(by=["Open
-00020570: 225d 2c20 6173 6365 6e64 696e 673d 4661  "], ascending=Fa
-00020580: 6c73 6529 0d0a 2020 2020 2020 2020 2020  lse)..          
-00020590: 2020 636c 6f73 6544 6573 6320 3d20 6461    closeDesc = da
-000205a0: 7461 2e73 6f72 745f 7661 6c75 6573 2862  ta.sort_values(b
-000205b0: 793d 5b22 436c 6f73 6522 5d2c 2061 7363  y=["Close"], asc
-000205c0: 656e 6469 6e67 3d46 616c 7365 290d 0a20  ending=False).. 
-000205d0: 2020 2020 2020 2020 2020 2076 6f6c 4465             volDe
-000205e0: 7363 203d 2064 6174 612e 736f 7274 5f76  sc = data.sort_v
-000205f0: 616c 7565 7328 6279 3d5b 2256 6f6c 756d  alues(by=["Volum
-00020600: 6522 5d2c 2061 7363 656e 6469 6e67 3d46  e"], ascending=F
-00020610: 616c 7365 290d 0a20 2020 2020 2020 2020  alse)..         
-00020620: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
-00020630: 2020 2020 2020 2020 2069 6620 280d 0a20           if (.. 
-00020640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020650: 2020 2064 6174 612e 6571 7561 6c73 286f     data.equals(o
-00020660: 7065 6e44 6573 6329 0d0a 2020 2020 2020  penDesc)..      
-00020670: 2020 2020 2020 2020 2020 2020 2020 616e                an
-00020680: 6420 6461 7461 2e65 7175 616c 7328 636c  d data.equals(cl
-00020690: 6f73 6544 6573 6329 0d0a 2020 2020 2020  oseDesc)..      
-000206a0: 2020 2020 2020 2020 2020 2020 2020 616e                an
-000206b0: 6420 6461 7461 2e65 7175 616c 7328 766f  d data.equals(vo
-000206c0: 6c44 6573 6329 0d0a 2020 2020 2020 2020  lDesc)..        
-000206d0: 2020 2020 2020 2020 293a 0d0a 2020 2020          ):..    
-000206e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000206f0: 2320 7365 6c66 2e64 6566 6175 6c74 5f6c  # self.default_l
-00020700: 6f67 6765 722e 696e 666f 280d 0a20 2020  ogger.info(..   
-00020710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020720: 2023 2020 2020 2066 2753 746f 636b 3a7b   #     f'Stock:{
-00020730: 7361 7665 4469 6374 5b22 5374 6f63 6b22  saveDict["Stock"
-00020740: 5d7d 2c20 6f70 656e 2c63 6c6f 7365 2061  ]}, open,close a
-00020750: 6e64 2076 6f6c 756d 6520 6571 7561 6c20  nd volume equal 
-00020760: 6672 6f6d 2064 6179 2062 6566 6f72 6520  from day before 
-00020770: 7965 7374 6572 6461 792e 2041 2070 6f74  yesterday. A pot
-00020780: 656e 7469 616c 206d 6f6d 656e 7475 6d2d  ential momentum-
-00020790: 6761 696e 6572 2127 0d0a 2020 2020 2020  gainer!'..      
-000207a0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-000207b0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000207c0: 2020 2020 2020 2074 6f20 3d20 6461 7461         to = data
-000207d0: 5b22 4f70 656e 225d 2e69 6c6f 635b 305d  ["Open"].iloc[0]
-000207e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000207f0: 2020 2020 2020 7963 203d 2064 6174 615b        yc = data[
-00020800: 2243 6c6f 7365 225d 2e69 6c6f 635b 315d  "Close"].iloc[1]
-00020810: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00020820: 2020 2020 2020 796f 203d 2064 6174 615b        yo = data[
-00020830: 224f 7065 6e22 5d2e 696c 6f63 5b31 5d0d  "Open"].iloc[1].
-00020840: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00020850: 2020 2020 2064 7963 203d 2064 6174 615b       dyc = data[
-00020860: 2243 6c6f 7365 225d 2e69 6c6f 635b 325d  "Close"].iloc[2]
-00020870: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00020880: 2020 2020 2020 6966 2028 746f 203e 3d20        if (to >= 
-00020890: 7963 2920 616e 6420 2879 6f20 3e3d 2064  yc) and (yo >= d
-000208a0: 7963 293a 0d0a 2020 2020 2020 2020 2020  yc):..          
-000208b0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-000208c0: 7365 6c66 2e64 6566 6175 6c74 5f6c 6f67  self.default_log
-000208d0: 6765 722e 696e 666f 280d 0a20 2020 2020  ger.info(..     
-000208e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000208f0: 2020 2023 2020 2020 2066 2753 746f 636b     #     f'Stock
-00020900: 3a7b 7361 7665 4469 6374 5b22 5374 6f63  :{saveDict["Stoc
-00020910: 6b22 5d7d 2c20 6973 2061 206d 6f6d 656e  k"]}, is a momen
-00020920: 7475 6d2d 6761 696e 6572 2062 6563 6175  tum-gainer becau
-00020930: 7365 2074 6f64 6179 2d6f 7065 6e20 287b  se today-open ({
-00020940: 746f 7d29 203e 3d20 7965 7374 6572 6461  to}) >= yesterda
-00020950: 792d 636c 6f73 6520 287b 7963 7d29 2061  y-close ({yc}) a
-00020960: 6e64 2079 6573 7465 7264 6179 2d6f 7065  nd yesterday-ope
-00020970: 6e28 7b79 6f7d 2920 3e3d 2064 6179 2d62  n({yo}) >= day-b
-00020980: 6566 6f72 652d 636c 6f73 6528 7b64 7963  efore-close({dyc
-00020990: 7d29 270d 0a20 2020 2020 2020 2020 2020  })'..           
-000209a0: 2020 2020 2020 2020 2020 2020 2023 2029               # )
-000209b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000209c0: 2020 2020 2020 2020 2020 7361 7665 6420            saved 
-000209d0: 3d20 7365 6c66 2e66 696e 6443 7572 7265  = self.findCurre
-000209e0: 6e74 5361 7665 6456 616c 7565 2873 6372  ntSavedValue(scr
-000209f0: 6565 6e44 6963 742c 2073 6176 6544 6963  eenDict, saveDic
-00020a00: 742c 2022 5061 7474 6572 6e22 290d 0a20  t, "Pattern").. 
-00020a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020a20: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
-00020a30: 745b 2250 6174 7465 726e 225d 203d 2028  t["Pattern"] = (
-00020a40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00020a50: 2020 2020 2020 2020 2020 2020 2020 7361                sa
-00020a60: 7665 645b 305d 0d0a 2020 2020 2020 2020  ved[0]..        
+0001d630: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
+0001d640: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001d650: 6176 6544 6963 745b 2250 6174 7465 726e  aveDict["Pattern
+0001d660: 225d 203d 2073 6176 6564 5b31 5d20 2b20  "] = saved[1] + 
+0001d670: 2249 6e73 6964 6520 4261 7220 2825 6429  "Inside Bar (%d)
+0001d680: 2220 2520 690d 0a20 2020 2020 2020 2020  " % i..         
+0001d690: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0001d6a0: 6574 7572 6e20 690d 0a20 2020 2020 2020  eturn i..       
+0001d6b0: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
+0001d6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d6d0: 2020 2020 7265 7475 726e 2030 0d0a 2020      return 0..  
+0001d6e0: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
+0001d6f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001d700: 2069 6620 2244 6f77 6e22 2069 6e20 7361   if "Down" in sa
+0001d710: 7665 4469 6374 5b22 5472 656e 6422 5d20  veDict["Trend"] 
+0001d720: 616e 6420 280d 0a20 2020 2020 2020 2020  and (..         
+0001d730: 2020 2020 2020 2020 2020 2022 4265 6172             "Bear
+0001d740: 2220 696e 2073 6176 6544 6963 745b 224d  " in saveDict["M
+0001d750: 412d 5369 676e 616c 225d 206f 7220 2252  A-Signal"] or "R
+0001d760: 6573 6973 7422 2069 6e20 7361 7665 4469  esist" in saveDi
+0001d770: 6374 5b22 4d41 2d53 6967 6e61 6c22 5d0d  ct["MA-Signal"].
+0001d780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001d790: 2029 3a0d 0a20 2020 2020 2020 2020 2020   ):..           
+0001d7a0: 2020 2020 2020 2020 2064 6174 6120 3d20           data = 
+0001d7b0: 6f72 6744 6174 612e 6865 6164 2869 290d  orgData.head(i).
+0001d7c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001d7d0: 2020 2020 2072 6566 4361 6e64 6c65 203d       refCandle =
+0001d7e0: 2064 6174 612e 7461 696c 2831 290d 0a20   data.tail(1).. 
+0001d7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d800: 2020 2069 6620 280d 0a20 2020 2020 2020     if (..       
+0001d810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d820: 2028 6c65 6e28 6461 7461 2e48 6967 685b   (len(data.High[
+0001d830: 6461 7461 2e48 6967 6820 3e20 7265 6643  data.High > refC
+0001d840: 616e 646c 652e 4869 6768 2e69 7465 6d28  andle.High.item(
+0001d850: 295d 2920 3d3d 2030 290d 0a20 2020 2020  )]) == 0)..     
+0001d860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d870: 2020 2061 6e64 2028 6c65 6e28 6461 7461     and (len(data
+0001d880: 2e4c 6f77 5b64 6174 612e 4c6f 7720 3c20  .Low[data.Low < 
+0001d890: 7265 6643 616e 646c 652e 4c6f 772e 6974  refCandle.Low.it
+0001d8a0: 656d 2829 5d29 203d 3d20 3029 0d0a 2020  em()]) == 0)..  
+0001d8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d8c0: 2020 2020 2020 616e 6420 286c 656e 2864        and (len(d
+0001d8d0: 6174 612e 4f70 656e 5b64 6174 612e 4f70  ata.Open[data.Op
+0001d8e0: 656e 203e 2072 6566 4361 6e64 6c65 2e48  en > refCandle.H
+0001d8f0: 6967 682e 6974 656d 2829 5d29 203d 3d20  igh.item()]) == 
+0001d900: 3029 0d0a 2020 2020 2020 2020 2020 2020  0)..            
+0001d910: 2020 2020 2020 2020 2020 2020 616e 6420              and 
+0001d920: 286c 656e 2864 6174 612e 436c 6f73 655b  (len(data.Close[
+0001d930: 6461 7461 2e43 6c6f 7365 203c 2072 6566  data.Close < ref
+0001d940: 4361 6e64 6c65 2e4c 6f77 2e69 7465 6d28  Candle.Low.item(
+0001d950: 295d 2920 3d3d 2030 290d 0a20 2020 2020  )]) == 0)..     
+0001d960: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+0001d970: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0001d980: 2020 2020 2020 2020 2020 2073 6372 6565             scree
+0001d990: 6e44 6963 745b 2250 6174 7465 726e 225d  nDict["Pattern"]
+0001d9a0: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
+0001d9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d9c0: 2020 7361 7665 645b 305d 0d0a 2020 2020    saved[0]..    
+0001d9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d9e0: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
+0001d9f0: 6578 742e 424f 4c44 0d0a 2020 2020 2020  ext.BOLD..      
+0001da00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001da10: 2020 2020 2020 2b20 636f 6c6f 7254 6578        + colorTex
+0001da20: 742e 5741 524e 0d0a 2020 2020 2020 2020  t.WARN..        
+0001da30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001da40: 2020 2020 2b20 2822 496e 7369 6465 2042      + ("Inside B
+0001da50: 6172 2028 2564 2922 2025 2069 290d 0a20  ar (%d)" % i).. 
+0001da60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001da70: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
+0001da80: 6f72 5465 7874 2e45 4e44 0d0a 2020 2020  orText.END..    
+0001da90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001daa0: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
+0001dab0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001dac0: 6176 6544 6963 745b 2250 6174 7465 726e  aveDict["Pattern
+0001dad0: 225d 203d 2073 6176 6564 5b31 5d20 2b20  "] = saved[1] + 
+0001dae0: 2249 6e73 6964 6520 4261 7220 2825 6429  "Inside Bar (%d)
+0001daf0: 2220 2520 690d 0a20 2020 2020 2020 2020  " % i..         
+0001db00: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0001db10: 6574 7572 6e20 690d 0a20 2020 2020 2020  eturn i..       
+0001db20: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
+0001db30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001db40: 2020 2020 7265 7475 726e 2030 0d0a 2020      return 0..  
+0001db50: 2020 2020 2020 7265 7475 726e 2030 0d0a        return 0..
+0001db60: 0d0a 2020 2020 2320 4669 6e64 2049 504f  ..    # Find IPO
+0001db70: 2062 6173 650d 0a20 2020 2064 6566 2076   base..    def v
+0001db80: 616c 6964 6174 6549 706f 4261 7365 2873  alidateIpoBase(s
+0001db90: 656c 662c 2073 746f 636b 2c20 6466 2c20  elf, stock, df, 
+0001dba0: 7363 7265 656e 4469 6374 2c20 7361 7665  screenDict, save
+0001dbb0: 4469 6374 2c20 7065 7263 656e 7461 6765  Dict, percentage
+0001dbc0: 3d30 2e33 293a 0d0a 2020 2020 2020 2020  =0.3):..        
+0001dbd0: 6966 2064 6620 6973 204e 6f6e 6520 6f72  if df is None or
+0001dbe0: 206c 656e 2864 6629 203d 3d20 303a 0d0a   len(df) == 0:..
+0001dbf0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0001dc00: 726e 2046 616c 7365 0d0a 2020 2020 2020  rn False..      
+0001dc10: 2020 6461 7461 203d 2064 662e 636f 7079    data = df.copy
+0001dc20: 2829 0d0a 2020 2020 2020 2020 6c69 7374  ()..        list
+0001dc30: 696e 6750 7269 6365 203d 2064 6174 615b  ingPrice = data[
+0001dc40: 3a3a 2d31 5d2e 6865 6164 2831 295b 224f  ::-1].head(1)["O
+0001dc50: 7065 6e22 5d2e 696c 6f63 5b30 5d0d 0a20  pen"].iloc[0].. 
+0001dc60: 2020 2020 2020 2063 7572 7265 6e74 5072         currentPr
+0001dc70: 6963 6520 3d20 6461 7461 2e68 6561 6428  ice = data.head(
+0001dc80: 3129 5b22 436c 6f73 6522 5d2e 696c 6f63  1)["Close"].iloc
+0001dc90: 5b30 5d0d 0a20 2020 2020 2020 2041 5448  [0]..        ATH
+0001dca0: 203d 2064 6174 612e 6465 7363 7269 6265   = data.describe
+0001dcb0: 2829 5b22 4869 6768 225d 5b22 6d61 7822  ()["High"]["max"
+0001dcc0: 5d0d 0a20 2020 2020 2020 2069 6620 4154  ]..        if AT
+0001dcd0: 4820 3e20 286c 6973 7469 6e67 5072 6963  H > (listingPric
+0001dce0: 6520 2b20 286c 6973 7469 6e67 5072 6963  e + (listingPric
+0001dcf0: 6520 2a20 7065 7263 656e 7461 6765 2929  e * percentage))
+0001dd00: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+0001dd10: 6574 7572 6e20 4661 6c73 650d 0a20 2020  eturn False..   
+0001dd20: 2020 2020 2061 7761 7920 3d20 726f 756e       away = roun
+0001dd30: 6428 2828 6375 7272 656e 7450 7269 6365  d(((currentPrice
+0001dd40: 202d 206c 6973 7469 6e67 5072 6963 6529   - listingPrice)
+0001dd50: 202f 206c 6973 7469 6e67 5072 6963 6529   / listingPrice)
+0001dd60: 202a 2031 3030 2c20 3129 0d0a 2020 2020   * 100, 1)..    
+0001dd70: 2020 2020 6966 2028 0d0a 2020 2020 2020      if (..      
+0001dd80: 2020 2020 2020 286c 6973 7469 6e67 5072        (listingPr
+0001dd90: 6963 6520 2d20 286c 6973 7469 6e67 5072  ice - (listingPr
+0001dda0: 6963 6520 2a20 7065 7263 656e 7461 6765  ice * percentage
+0001ddb0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+0001ddc0: 3c3d 2063 7572 7265 6e74 5072 6963 650d  <= currentPrice.
+0001ddd0: 0a20 2020 2020 2020 2020 2020 203c 3d20  .            <= 
+0001dde0: 286c 6973 7469 6e67 5072 6963 6520 2b20  (listingPrice + 
+0001ddf0: 286c 6973 7469 6e67 5072 6963 6520 2a20  (listingPrice * 
+0001de00: 7065 7263 656e 7461 6765 2929 0d0a 2020  percentage))..  
+0001de10: 2020 2020 2020 293a 0d0a 2020 2020 2020        ):..      
+0001de20: 2020 2020 2020 7361 7665 6420 3d20 7365        saved = se
+0001de30: 6c66 2e66 696e 6443 7572 7265 6e74 5361  lf.findCurrentSa
+0001de40: 7665 6456 616c 7565 2873 6372 6565 6e44  vedValue(screenD
+0001de50: 6963 742c 2073 6176 6544 6963 742c 2022  ict, saveDict, "
+0001de60: 5061 7474 6572 6e22 290d 0a20 2020 2020  Pattern")..     
+0001de70: 2020 2020 2020 2069 6620 6177 6179 203e         if away >
+0001de80: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
+0001de90: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
+0001dea0: 2250 6174 7465 726e 225d 203d 2028 0d0a  "Pattern"] = (..
+0001deb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dec0: 2020 2020 7361 7665 645b 305d 200d 0a20      saved[0] .. 
+0001ded0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dee0: 2020 202b 2063 6f6c 6f72 5465 7874 2e42     + colorText.B
+0001def0: 4f4c 440d 0a20 2020 2020 2020 2020 2020  OLD..           
+0001df00: 2020 2020 2020 2020 202b 2063 6f6c 6f72           + color
+0001df10: 5465 7874 2e47 5245 454e 0d0a 2020 2020  Text.GREEN..    
+0001df20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001df30: 2b20 6622 4950 4f20 4261 7365 2028 7b61  + f"IPO Base ({a
+0001df40: 7761 797d 2025 2922 0d0a 2020 2020 2020  way} %)"..      
+0001df50: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+0001df60: 636f 6c6f 7254 6578 742e 454e 440d 0a20  colorText.END.. 
+0001df70: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+0001df80: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
+0001df90: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+0001dfa0: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
+0001dfb0: 2250 6174 7465 726e 225d 203d 2028 0d0a  "Pattern"] = (..
+0001dfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dfd0: 2020 2020 7361 7665 645b 305d 0d0a 2020      saved[0]..  
+0001dfe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dff0: 2020 2b20 636f 6c6f 7254 6578 742e 424f    + colorText.BO
+0001e000: 4c44 0d0a 2020 2020 2020 2020 2020 2020  LD..            
+0001e010: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
+0001e020: 6578 742e 4752 4545 4e0d 0a20 2020 2020  ext.GREEN..     
+0001e030: 2020 2020 2020 2020 2020 2020 2020 202b                 +
+0001e040: 2022 4950 4f20 4261 7365 2022 0d0a 2020   "IPO Base "..  
+0001e050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e060: 2020 2b20 636f 6c6f 7254 6578 742e 4641    + colorText.FA
+0001e070: 494c 0d0a 2020 2020 2020 2020 2020 2020  IL..            
+0001e080: 2020 2020 2020 2020 2b20 6622 287b 6177          + f"({aw
+0001e090: 6179 7d20 2529 220d 0a20 2020 2020 2020  ay} %)"..       
+0001e0a0: 2020 2020 2020 2020 2020 2020 202b 2063               + c
+0001e0b0: 6f6c 6f72 5465 7874 2e45 4e44 0d0a 2020  olorText.END..  
+0001e0c0: 2020 2020 2020 2020 2020 2020 2020 290d                ).
+0001e0d0: 0a20 2020 2020 2020 2020 2020 2073 6176  .            sav
+0001e0e0: 6544 6963 745b 2250 6174 7465 726e 225d  eDict["Pattern"]
+0001e0f0: 203d 2073 6176 6564 5b31 5d20 2b20 6622   = saved[1] + f"
+0001e100: 4950 4f20 4261 7365 2028 7b61 7761 797d  IPO Base ({away}
+0001e110: 2025 2922 0d0a 2020 2020 2020 2020 2020   %)"..          
+0001e120: 2020 7265 7475 726e 2054 7275 650d 0a20    return True.. 
+0001e130: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+0001e140: 6c73 650d 0a0d 0a20 2020 2023 406d 6561  lse....    #@mea
+0001e150: 7375 7265 5f74 696d 650d 0a20 2020 2023  sure_time..    #
+0001e160: 2056 616c 6964 6174 6520 4c6f 7265 6e74   Validate Lorent
+0001e170: 7a69 616e 2043 6c61 7373 6966 6963 6174  zian Classificat
+0001e180: 696f 6e20 7369 676e 616c 0d0a 2020 2020  ion signal..    
+0001e190: 6465 6620 7661 6c69 6461 7465 4c6f 7265  def validateLore
+0001e1a0: 6e74 7a69 616e 2873 656c 662c 2064 662c  ntzian(self, df,
+0001e1b0: 2073 6372 6565 6e44 6963 742c 2073 6176   screenDict, sav
+0001e1c0: 6544 6963 742c 206c 6f6f 6b46 6f72 3d33  eDict, lookFor=3
+0001e1d0: 293a 0d0a 2020 2020 2020 2020 6966 2064  ):..        if d
+0001e1e0: 6620 6973 204e 6f6e 6520 6f72 206c 656e  f is None or len
+0001e1f0: 2864 6629 203d 3d20 303a 0d0a 2020 2020  (df) == 0:..    
+0001e200: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+0001e210: 616c 7365 0d0a 2020 2020 2020 2020 6461  alse..        da
+0001e220: 7461 203d 2064 662e 636f 7079 2829 0d0a  ta = df.copy()..
+0001e230: 2020 2020 2020 2020 2320 6c6f 6f6b 466f          # lookFo
+0001e240: 723a 2031 2d42 7579 2c20 322d 5365 6c6c  r: 1-Buy, 2-Sell
+0001e250: 2c20 332d 416e 790d 0a20 2020 2020 2020  , 3-Any..       
+0001e260: 2064 6174 6120 3d20 6461 7461 5b3a 3a2d   data = data[::-
+0001e270: 315d 2020 2320 5265 7665 7273 6520 7468  1]  # Reverse th
+0001e280: 6520 6461 7461 6672 616d 650d 0a20 2020  e dataframe..   
+0001e290: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
+0001e2a0: 2e72 656e 616d 6528 0d0a 2020 2020 2020  .rename(..      
+0001e2b0: 2020 2020 2020 636f 6c75 6d6e 733d 7b0d        columns={.
+0001e2c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001e2d0: 2022 4f70 656e 223a 2022 6f70 656e 222c   "Open": "open",
+0001e2e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001e2f0: 2020 2243 6c6f 7365 223a 2022 636c 6f73    "Close": "clos
+0001e300: 6522 2c0d 0a20 2020 2020 2020 2020 2020  e",..           
+0001e310: 2020 2020 2022 4869 6768 223a 2022 6869       "High": "hi
+0001e320: 6768 222c 0d0a 2020 2020 2020 2020 2020  gh",..          
+0001e330: 2020 2020 2020 224c 6f77 223a 2022 6c6f        "Low": "lo
+0001e340: 7722 2c0d 0a20 2020 2020 2020 2020 2020  w",..           
+0001e350: 2020 2020 2022 566f 6c75 6d65 223a 2022       "Volume": "
+0001e360: 766f 6c75 6d65 222c 0d0a 2020 2020 2020  volume",..      
+0001e370: 2020 2020 2020 7d0d 0a20 2020 2020 2020        }..       
+0001e380: 2029 0d0a 2020 2020 2020 2020 7472 793a   )..        try:
+0001e390: 0d0a 2020 2020 2020 2020 2020 2020 7769  ..            wi
+0001e3a0: 7468 2053 7570 7072 6573 734f 7574 7075  th SuppressOutpu
+0001e3b0: 7428 7375 7070 7265 7373 5f73 7464 6f75  t(suppress_stdou
+0001e3c0: 743d 5472 7565 2c20 7375 7070 7265 7373  t=True, suppress
+0001e3d0: 5f73 7464 6572 723d 5472 7565 293a 0d0a  _stderr=True):..
+0001e3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e3f0: 6c63 203d 2061 7461 2e4c 6f72 656e 747a  lc = ata.Lorentz
+0001e400: 6961 6e43 6c61 7373 6966 6963 6174 696f  ianClassificatio
+0001e410: 6e28 6461 7461 3d64 6174 6129 0d0a 2020  n(data=data)..  
+0001e420: 2020 2020 2020 2020 2020 7361 7665 6420            saved 
+0001e430: 3d20 7365 6c66 2e66 696e 6443 7572 7265  = self.findCurre
+0001e440: 6e74 5361 7665 6456 616c 7565 2873 6372  ntSavedValue(scr
+0001e450: 6565 6e44 6963 742c 2073 6176 6544 6963  eenDict, saveDic
+0001e460: 742c 2022 5061 7474 6572 6e22 290d 0a20  t, "Pattern").. 
+0001e470: 2020 2020 2020 2020 2020 2069 6620 6c63             if lc
+0001e480: 2e64 662e 696c 6f63 5b2d 315d 5b22 6973  .df.iloc[-1]["is
+0001e490: 4e65 7742 7579 5369 676e 616c 225d 3a0d  NewBuySignal"]:.
+0001e4a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001e4b0: 2073 6372 6565 6e44 6963 745b 2250 6174   screenDict["Pat
+0001e4c0: 7465 726e 225d 203d 2028 0d0a 2020 2020  tern"] = (..    
+0001e4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e4e0: 7361 7665 645b 305d 202b 2063 6f6c 6f72  saved[0] + color
+0001e4f0: 5465 7874 2e42 4f4c 4420 2b20 636f 6c6f  Text.BOLD + colo
+0001e500: 7254 6578 742e 4752 4545 4e20 2b20 224c  rText.GREEN + "L
+0001e510: 6f72 656e 747a 6961 6e2d 4275 7922 202b  orentzian-Buy" +
+0001e520: 2063 6f6c 6f72 5465 7874 2e45 4e44 0d0a   colorText.END..
+0001e530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e540: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0001e550: 2020 2073 6176 6544 6963 745b 2250 6174     saveDict["Pat
+0001e560: 7465 726e 225d 203d 2073 6176 6564 5b31  tern"] = saved[1
+0001e570: 5d20 2b20 224c 6f72 656e 747a 6961 6e2d  ] + "Lorentzian-
+0001e580: 4275 7922 0d0a 2020 2020 2020 2020 2020  Buy"..          
+0001e590: 2020 2020 2020 6966 206c 6f6f 6b46 6f72        if lookFor
+0001e5a0: 2021 3d20 323a 2023 204e 6f74 2053 656c   != 2: # Not Sel
+0001e5b0: 6c0d 0a20 2020 2020 2020 2020 2020 2020  l..             
+0001e5c0: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
+0001e5d0: 7565 0d0a 2020 2020 2020 2020 2020 2020  ue..            
+0001e5e0: 656c 6966 206c 632e 6466 2e69 6c6f 635b  elif lc.df.iloc[
+0001e5f0: 2d31 5d5b 2269 734e 6577 5365 6c6c 5369  -1]["isNewSellSi
+0001e600: 676e 616c 225d 3a0d 0a20 2020 2020 2020  gnal"]:..       
+0001e610: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
+0001e620: 6963 745b 2250 6174 7465 726e 225d 203d  ict["Pattern"] =
+0001e630: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
+0001e640: 2020 2020 2020 2020 7361 7665 645b 305d          saved[0]
+0001e650: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
+0001e660: 4420 2b20 636f 6c6f 7254 6578 742e 4641  D + colorText.FA
+0001e670: 494c 202b 2022 4c6f 7265 6e74 7a69 616e  IL + "Lorentzian
+0001e680: 2d53 656c 6c22 202b 2063 6f6c 6f72 5465  -Sell" + colorTe
+0001e690: 7874 2e45 4e44 0d0a 2020 2020 2020 2020  xt.END..        
+0001e6a0: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
+0001e6b0: 2020 2020 2020 2020 2020 2073 6176 6544             saveD
+0001e6c0: 6963 745b 2250 6174 7465 726e 225d 203d  ict["Pattern"] =
+0001e6d0: 2073 6176 6564 5b31 5d20 2b20 224c 6f72   saved[1] + "Lor
+0001e6e0: 656e 747a 6961 6e2d 5365 6c6c 220d 0a20  entzian-Sell".. 
+0001e6f0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0001e700: 6620 6c6f 6f6b 466f 7220 213d 2031 3a20  f lookFor != 1: 
+0001e710: 2320 4e6f 7420 4275 790d 0a20 2020 2020  # Not Buy..     
+0001e720: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0001e730: 6574 7572 6e20 5472 7565 0d0a 2020 2020  eturn True..    
+0001e740: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
+0001e750: 7469 6f6e 3a20 2023 2070 7261 676d 613a  tion:  # pragma:
+0001e760: 206e 6f20 636f 7665 720d 0a20 2020 2020   no cover..     
+0001e770: 2020 2020 2020 2023 2056 616c 7565 4572         # ValueEr
+0001e780: 726f 723a 206f 7065 7261 6e64 7320 636f  ror: operands co
+0001e790: 756c 6420 6e6f 7420 6265 2062 726f 6164  uld not be broad
+0001e7a0: 6361 7374 2074 6f67 6574 6865 7220 7769  cast together wi
+0001e7b0: 7468 2073 6861 7065 7320 2832 302c 2920  th shapes (20,) 
+0001e7c0: 2832 362c 290d 0a20 2020 2020 2020 2020  (26,)..         
+0001e7d0: 2020 2023 2046 696c 6520 222f 6f70 742f     # File "/opt/
+0001e7e0: 686f 6d65 6272 6577 2f6c 6962 2f70 7974  homebrew/lib/pyt
+0001e7f0: 686f 6e33 2e31 312f 7369 7465 2d70 6163  hon3.11/site-pac
+0001e800: 6b61 6765 732f 6164 7661 6e63 6564 5f74  kages/advanced_t
+0001e810: 612f 4c6f 7265 6e74 7a69 616e 436c 6173  a/LorentzianClas
+0001e820: 7369 6669 6361 7469 6f6e 2f43 6c61 7373  sification/Class
+0001e830: 6966 6965 722e 7079 222c 206c 696e 6520  ifier.py", line 
+0001e840: 3138 362c 2069 6e20 5f5f 696e 6974 5f5f  186, in __init__
+0001e850: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+0001e860: 4669 6c65 2022 2f6f 7074 2f68 6f6d 6562  File "/opt/homeb
+0001e870: 7265 772f 6c69 622f 7079 7468 6f6e 332e  rew/lib/python3.
+0001e880: 3131 2f73 6974 652d 7061 636b 6167 6573  11/site-packages
+0001e890: 2f61 6476 616e 6365 645f 7461 2f4c 6f72  /advanced_ta/Lor
+0001e8a0: 656e 747a 6961 6e43 6c61 7373 6966 6963  entzianClassific
+0001e8b0: 6174 696f 6e2f 436c 6173 7369 6669 6572  ation/Classifier
+0001e8c0: 2e70 7922 2c20 6c69 6e65 2033 3935 2c20  .py", line 395, 
+0001e8d0: 696e 205f 5f63 6c61 7373 6966 790d 0a20  in __classify.. 
+0001e8e0: 2020 2020 2020 2020 2020 2023 2046 696c             # Fil
+0001e8f0: 6520 222f 6f70 742f 686f 6d65 6272 6577  e "/opt/homebrew
+0001e900: 2f6c 6962 2f70 7974 686f 6e33 2e31 312f  /lib/python3.11/
+0001e910: 7369 7465 2d70 6163 6b61 6765 732f 7061  site-packages/pa
+0001e920: 6e64 6173 2f63 6f72 652f 6f70 732f 636f  ndas/core/ops/co
+0001e930: 6d6d 6f6e 2e70 7922 2c20 6c69 6e65 2037  mmon.py", line 7
+0001e940: 362c 2069 6e20 6e65 775f 6d65 7468 6f64  6, in new_method
+0001e950: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+0001e960: 4669 6c65 2022 2f6f 7074 2f68 6f6d 6562  File "/opt/homeb
+0001e970: 7265 772f 6c69 622f 7079 7468 6f6e 332e  rew/lib/python3.
+0001e980: 3131 2f73 6974 652d 7061 636b 6167 6573  11/site-packages
+0001e990: 2f70 616e 6461 732f 636f 7265 2f61 7272  /pandas/core/arr
+0001e9a0: 6179 6c69 6b65 2e70 7922 2c20 6c69 6e65  aylike.py", line
+0001e9b0: 2037 302c 2069 6e20 5f5f 616e 645f 5f0d   70, in __and__.
+0001e9c0: 0a20 2020 2020 2020 2020 2020 2023 2046  .            # F
+0001e9d0: 696c 6520 222f 6f70 742f 686f 6d65 6272  ile "/opt/homebr
+0001e9e0: 6577 2f6c 6962 2f70 7974 686f 6e33 2e31  ew/lib/python3.1
+0001e9f0: 312f 7369 7465 2d70 6163 6b61 6765 732f  1/site-packages/
+0001ea00: 7061 6e64 6173 2f63 6f72 652f 7365 7269  pandas/core/seri
+0001ea10: 6573 2e70 7922 2c20 6c69 6e65 2035 3831  es.py", line 581
+0001ea20: 302c 2069 6e20 5f6c 6f67 6963 616c 5f6d  0, in _logical_m
+0001ea30: 6574 686f 640d 0a20 2020 2020 2020 2020  ethod..         
+0001ea40: 2020 2023 2046 696c 6520 222f 6f70 742f     # File "/opt/
+0001ea50: 686f 6d65 6272 6577 2f6c 6962 2f70 7974  homebrew/lib/pyt
+0001ea60: 686f 6e33 2e31 312f 7369 7465 2d70 6163  hon3.11/site-pac
+0001ea70: 6b61 6765 732f 7061 6e64 6173 2f63 6f72  kages/pandas/cor
+0001ea80: 652f 6f70 732f 6172 7261 795f 6f70 732e  e/ops/array_ops.
+0001ea90: 7079 222c 206c 696e 6520 3435 362c 2069  py", line 456, i
+0001eaa0: 6e20 6c6f 6769 6361 6c5f 6f70 0d0a 2020  n logical_op..  
+0001eab0: 2020 2020 2020 2020 2020 2320 4669 6c65            # File
+0001eac0: 2022 2f6f 7074 2f68 6f6d 6562 7265 772f   "/opt/homebrew/
+0001ead0: 6c69 622f 7079 7468 6f6e 332e 3131 2f73  lib/python3.11/s
+0001eae0: 6974 652d 7061 636b 6167 6573 2f70 616e  ite-packages/pan
+0001eaf0: 6461 732f 636f 7265 2f6f 7073 2f61 7272  das/core/ops/arr
+0001eb00: 6179 5f6f 7073 2e70 7922 2c20 6c69 6e65  ay_ops.py", line
+0001eb10: 2033 3634 2c20 696e 206e 615f 6c6f 6769   364, in na_logi
+0001eb20: 6361 6c5f 6f70 0d0a 2020 2020 2020 2020  cal_op..        
+0001eb30: 2020 2020 2320 7365 6c66 2e64 6566 6175      # self.defau
+0001eb40: 6c74 5f6c 6f67 6765 722e 6465 6275 6728  lt_logger.debug(
+0001eb50: 652c 2065 7863 5f69 6e66 6f3d 5472 7565  e, exc_info=True
+0001eb60: 290d 0a20 2020 2020 2020 2020 2020 2070  )..            p
+0001eb70: 6173 730d 0a20 2020 2020 2020 2072 6574  ass..        ret
+0001eb80: 7572 6e20 4661 6c73 650d 0a0d 0a20 2020  urn False....   
+0001eb90: 2023 2076 616c 6964 6174 6520 6966 2074   # validate if t
+0001eba0: 6865 2073 746f 636b 2068 6173 2062 6565  he stock has bee
+0001ebb0: 6e20 6861 7669 6e67 206c 6f77 6572 206c  n having lower l
+0001ebc0: 6f77 732c 206c 6f77 6572 2068 6967 6873  ows, lower highs
+0001ebd0: 0d0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
+0001ebe0: 7465 4c6f 7765 7248 6967 6873 4c6f 7765  teLowerHighsLowe
+0001ebf0: 724c 6f77 7328 7365 6c66 2c20 6466 293a  rLows(self, df):
+0001ec00: 0d0a 2020 2020 2020 2020 6966 2064 6620  ..        if df 
+0001ec10: 6973 204e 6f6e 6520 6f72 206c 656e 2864  is None or len(d
+0001ec20: 6629 203d 3d20 303a 0d0a 2020 2020 2020  f) == 0:..      
+0001ec30: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+0001ec40: 7365 0d0a 2020 2020 2020 2020 6461 7461  se..        data
+0001ec50: 203d 2064 662e 636f 7079 2829 0d0a 2020   = df.copy()..  
+0001ec60: 2020 2020 2020 6461 7930 203d 2064 6174        day0 = dat
+0001ec70: 610d 0a20 2020 2020 2020 2064 6179 3120  a..        day1 
+0001ec80: 3d20 6461 7461 5b31 3a5d 0d0a 2020 2020  = data[1:]..    
+0001ec90: 2020 2020 6461 7932 203d 2064 6174 615b      day2 = data[
+0001eca0: 323a 5d0d 0a20 2020 2020 2020 2064 6179  2:]..        day
+0001ecb0: 3320 3d20 6461 7461 5b33 3a5d 0d0a 2020  3 = data[3:]..  
+0001ecc0: 2020 2020 2020 6c6f 7765 7248 6967 6873        lowerHighs
+0001ecd0: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
+0001ece0: 2020 2864 6179 305b 2248 6967 6822 5d2e    (day0["High"].
+0001ecf0: 696c 6f63 5b30 5d20 3c20 6461 7931 5b22  iloc[0] < day1["
+0001ed00: 4869 6768 225d 2e69 6c6f 635b 305d 290d  High"].iloc[0]).
+0001ed10: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
+0001ed20: 2028 6461 7931 5b22 4869 6768 225d 2e69   (day1["High"].i
+0001ed30: 6c6f 635b 305d 203c 2064 6179 325b 2248  loc[0] < day2["H
+0001ed40: 6967 6822 5d2e 696c 6f63 5b30 5d29 0d0a  igh"].iloc[0])..
+0001ed50: 2020 2020 2020 2020 2020 2020 616e 6420              and 
+0001ed60: 2864 6179 325b 2248 6967 6822 5d2e 696c  (day2["High"].il
+0001ed70: 6f63 5b30 5d20 3c20 6461 7933 5b22 4869  oc[0] < day3["Hi
+0001ed80: 6768 225d 2e69 6c6f 635b 305d 290d 0a20  gh"].iloc[0]).. 
+0001ed90: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+0001eda0: 2020 6c6f 7765 724c 6f77 7320 3d20 280d    lowerLows = (.
+0001edb0: 0a20 2020 2020 2020 2020 2020 2028 6461  .            (da
+0001edc0: 7930 5b22 4c6f 7722 5d2e 696c 6f63 5b30  y0["Low"].iloc[0
+0001edd0: 5d20 3c20 6461 7931 5b22 4c6f 7722 5d2e  ] < day1["Low"].
+0001ede0: 696c 6f63 5b30 5d29 0d0a 2020 2020 2020  iloc[0])..      
+0001edf0: 2020 2020 2020 616e 6420 2864 6179 315b        and (day1[
+0001ee00: 224c 6f77 225d 2e69 6c6f 635b 305d 203c  "Low"].iloc[0] <
+0001ee10: 2064 6179 325b 224c 6f77 225d 2e69 6c6f   day2["Low"].ilo
+0001ee20: 635b 305d 290d 0a20 2020 2020 2020 2020  c[0])..         
+0001ee30: 2020 2061 6e64 2028 6461 7932 5b22 4c6f     and (day2["Lo
+0001ee40: 7722 5d2e 696c 6f63 5b30 5d20 3c20 6461  w"].iloc[0] < da
+0001ee50: 7933 5b22 4c6f 7722 5d2e 696c 6f63 5b30  y3["Low"].iloc[0
+0001ee60: 5d29 0d0a 2020 2020 2020 2020 290d 0a20  ])..        ).. 
+0001ee70: 2020 2020 2020 2068 6967 6865 7252 5349         higherRSI
+0001ee80: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
+0001ee90: 2020 2864 6179 305b 2252 5349 225d 2e69    (day0["RSI"].i
+0001eea0: 6c6f 635b 305d 203c 2064 6179 315b 2252  loc[0] < day1["R
+0001eeb0: 5349 225d 2e69 6c6f 635b 305d 290d 0a20  SI"].iloc[0]).. 
+0001eec0: 2020 2020 2020 2020 2020 2061 6e64 2028             and (
+0001eed0: 6461 7931 5b22 5253 4922 5d2e 696c 6f63  day1["RSI"].iloc
+0001eee0: 5b30 5d20 3c20 6461 7932 5b22 5253 4922  [0] < day2["RSI"
+0001eef0: 5d2e 696c 6f63 5b30 5d29 0d0a 2020 2020  ].iloc[0])..    
+0001ef00: 2020 2020 2020 2020 616e 6420 2864 6179          and (day
+0001ef10: 325b 2252 5349 225d 2e69 6c6f 635b 305d  2["RSI"].iloc[0]
+0001ef20: 203c 2064 6179 335b 2252 5349 225d 2e69   < day3["RSI"].i
+0001ef30: 6c6f 635b 305d 290d 0a20 2020 2020 2020  loc[0])..       
+0001ef40: 2020 2020 2061 6e64 2064 6179 305b 2252       and day0["R
+0001ef50: 5349 225d 2e69 6c6f 635b 305d 203e 3d20  SI"].iloc[0] >= 
+0001ef60: 3530 0d0a 2020 2020 2020 2020 290d 0a20  50..        ).. 
+0001ef70: 2020 2020 2020 2072 6574 7572 6e20 6c6f         return lo
+0001ef80: 7765 7248 6967 6873 2061 6e64 206c 6f77  werHighs and low
+0001ef90: 6572 4c6f 7773 2061 6e64 2068 6967 6865  erLows and highe
+0001efa0: 7252 5349 0d0a 0d0a 2020 2020 2320 5661  rRSI....    # Va
+0001efb0: 6c69 6461 7465 2069 6620 7265 6365 6e74  lidate if recent
+0001efc0: 2076 6f6c 756d 6520 6973 206c 6f77 6573   volume is lowes
+0001efd0: 7420 6f66 206c 6173 7420 274e 2720 4461  t of last 'N' Da
+0001efe0: 7973 0d0a 2020 2020 6465 6620 7661 6c69  ys..    def vali
+0001eff0: 6461 7465 4c6f 7765 7374 566f 6c75 6d65  dateLowestVolume
+0001f000: 2873 656c 662c 2064 662c 2064 6179 7346  (self, df, daysF
+0001f010: 6f72 4c6f 7765 7374 566f 6c75 6d65 293a  orLowestVolume):
+0001f020: 0d0a 2020 2020 2020 2020 6966 2064 6620  ..        if df 
+0001f030: 6973 204e 6f6e 6520 6f72 206c 656e 2864  is None or len(d
+0001f040: 6629 203d 3d20 303a 0d0a 2020 2020 2020  f) == 0:..      
+0001f050: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+0001f060: 7365 0d0a 2020 2020 2020 2020 6461 7461  se..        data
+0001f070: 203d 2064 662e 636f 7079 2829 0d0a 2020   = df.copy()..  
+0001f080: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
+0001f090: 612e 6669 6c6c 6e61 2830 290d 0a20 2020  a.fillna(0)..   
+0001f0a0: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
+0001f0b0: 2e72 6570 6c61 6365 285b 6e70 2e69 6e66  .replace([np.inf
+0001f0c0: 2c20 2d6e 702e 696e 665d 2c20 3029 0d0a  , -np.inf], 0)..
+0001f0d0: 2020 2020 2020 2020 6966 2064 6179 7346          if daysF
+0001f0e0: 6f72 4c6f 7765 7374 566f 6c75 6d65 2069  orLowestVolume i
+0001f0f0: 7320 4e6f 6e65 3a0d 0a20 2020 2020 2020  s None:..       
+0001f100: 2020 2020 2064 6179 7346 6f72 4c6f 7765       daysForLowe
+0001f110: 7374 566f 6c75 6d65 203d 2033 300d 0a20  stVolume = 30.. 
+0001f120: 2020 2020 2020 2069 6620 6c65 6e28 6461         if len(da
+0001f130: 7461 2920 3c20 6461 7973 466f 724c 6f77  ta) < daysForLow
+0001f140: 6573 7456 6f6c 756d 653a 0d0a 2020 2020  estVolume:..    
+0001f150: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+0001f160: 616c 7365 0d0a 2020 2020 2020 2020 6461  alse..        da
+0001f170: 7461 203d 2064 6174 612e 6865 6164 2864  ta = data.head(d
+0001f180: 6179 7346 6f72 4c6f 7765 7374 566f 6c75  aysForLowestVolu
+0001f190: 6d65 290d 0a20 2020 2020 2020 2072 6563  me)..        rec
+0001f1a0: 656e 7420 3d20 6461 7461 2e68 6561 6428  ent = data.head(
+0001f1b0: 3129 0d0a 2020 2020 2020 2020 6966 206c  1)..        if l
+0001f1c0: 656e 2872 6563 656e 7429 203c 2031 3a0d  en(recent) < 1:.
+0001f1d0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0001f1e0: 7572 6e20 4661 6c73 650d 0a20 2020 2020  urn False..     
+0001f1f0: 2020 2069 6620 2872 6563 656e 745b 2256     if (recent["V
+0001f200: 6f6c 756d 6522 5d2e 696c 6f63 5b30 5d20  olume"].iloc[0] 
+0001f210: 3c3d 2064 6174 612e 6465 7363 7269 6265  <= data.describe
+0001f220: 2829 5b22 566f 6c75 6d65 225d 5b22 6d69  ()["Volume"]["mi
+0001f230: 6e22 5d29 2061 6e64 2072 6563 656e 745b  n"]) and recent[
+0001f240: 0d0a 2020 2020 2020 2020 2020 2020 2256  ..            "V
+0001f250: 6f6c 756d 6522 0d0a 2020 2020 2020 2020  olume"..        
+0001f260: 5d5b 305d 2021 3d20 6e70 2e6e 616e 3a0d  ][0] != np.nan:.
+0001f270: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0001f280: 7572 6e20 5472 7565 0d0a 2020 2020 2020  urn True..      
+0001f290: 2020 7265 7475 726e 2046 616c 7365 0d0a    return False..
+0001f2a0: 0d0a 2020 2020 2320 5661 6c69 6461 7465  ..    # Validate
+0001f2b0: 204c 5450 2077 6974 6869 6e20 6c69 6d69   LTP within limi
+0001f2c0: 7473 0d0a 2020 2020 6465 6620 7661 6c69  ts..    def vali
+0001f2d0: 6461 7465 4c54 5028 7365 6c66 2c20 6466  dateLTP(self, df
+0001f2e0: 2c20 7363 7265 656e 4469 6374 2c20 7361  , screenDict, sa
+0001f2f0: 7665 4469 6374 2c20 6d69 6e4c 5450 3d4e  veDict, minLTP=N
+0001f300: 6f6e 652c 206d 6178 4c54 503d 4e6f 6e65  one, maxLTP=None
+0001f310: 2c6d 696e 4368 616e 6765 3d30 293a 0d0a  ,minChange=0):..
+0001f320: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
+0001f330: 662e 636f 7079 2829 0d0a 2020 2020 2020  f.copy()..      
+0001f340: 2020 6c74 7056 616c 6964 203d 2046 616c    ltpValid = Fal
+0001f350: 7365 0d0a 2020 2020 2020 2020 6966 206d  se..        if m
+0001f360: 696e 4c54 5020 6973 204e 6f6e 653a 0d0a  inLTP is None:..
+0001f370: 2020 2020 2020 2020 2020 2020 6d69 6e4c              minL
+0001f380: 5450 203d 2073 656c 662e 636f 6e66 6967  TP = self.config
+0001f390: 4d61 6e61 6765 722e 6d69 6e4c 5450 0d0a  Manager.minLTP..
+0001f3a0: 2020 2020 2020 2020 6966 206d 6178 4c54          if maxLT
+0001f3b0: 5020 6973 204e 6f6e 653a 0d0a 2020 2020  P is None:..    
+0001f3c0: 2020 2020 2020 2020 6d61 784c 5450 203d          maxLTP =
+0001f3d0: 2073 656c 662e 636f 6e66 6967 4d61 6e61   self.configMana
+0001f3e0: 6765 722e 6d61 784c 5450 0d0a 2020 2020  ger.maxLTP..    
+0001f3f0: 2020 2020 6461 7461 203d 2064 6174 612e      data = data.
+0001f400: 6669 6c6c 6e61 2830 290d 0a20 2020 2020  fillna(0)..     
+0001f410: 2020 2064 6174 6120 3d20 6461 7461 2e72     data = data.r
+0001f420: 6570 6c61 6365 285b 6e70 2e69 6e66 2c20  eplace([np.inf, 
+0001f430: 2d6e 702e 696e 665d 2c20 3029 0d0a 2020  -np.inf], 0)..  
+0001f440: 2020 2020 2020 7265 6365 6e74 203d 2064        recent = d
+0001f450: 6174 612e 6865 6164 2831 290d 0a0d 0a20  ata.head(1).... 
+0001f460: 2020 2020 2020 2070 6374 5f63 6861 6e67         pct_chang
+0001f470: 6520 3d20 2864 6174 615b 3a3a 2d31 5d5b  e = (data[::-1][
+0001f480: 2243 6c6f 7365 225d 2e70 6374 5f63 6861  "Close"].pct_cha
+0001f490: 6e67 6528 2920 2a20 3130 3029 2e69 6c6f  nge() * 100).ilo
+0001f4a0: 635b 2d31 5d0d 0a20 2020 2020 2020 2069  c[-1]..        i
+0001f4b0: 6620 7063 745f 6368 616e 6765 203d 3d20  f pct_change == 
+0001f4c0: 6e70 2e69 6e66 206f 7220 7063 745f 6368  np.inf or pct_ch
+0001f4d0: 616e 6765 203d 3d20 2d6e 702e 696e 663a  ange == -np.inf:
+0001f4e0: 0d0a 2020 2020 2020 2020 2020 2020 7063  ..            pc
+0001f4f0: 745f 6368 616e 6765 203d 2030 0d0a 2020  t_change = 0..  
+0001f500: 2020 2020 2020 7063 745f 7361 7665 203d        pct_save =
+0001f510: 2022 252e 3166 2525 2220 2520 7063 745f   "%.1f%%" % pct_
+0001f520: 6368 616e 6765 0d0a 2020 2020 2020 2020  change..        
+0001f530: 6966 2070 6374 5f63 6861 6e67 6520 3e20  if pct_change > 
+0001f540: 302e 323a 0d0a 2020 2020 2020 2020 2020  0.2:..          
+0001f550: 2020 7063 745f 6368 616e 6765 203d 2063    pct_change = c
+0001f560: 6f6c 6f72 5465 7874 2e47 5245 454e 202b  olorText.GREEN +
+0001f570: 2028 2225 2e31 6625 2522 2025 2070 6374   ("%.1f%%" % pct
+0001f580: 5f63 6861 6e67 6529 202b 2063 6f6c 6f72  _change) + color
+0001f590: 5465 7874 2e45 4e44 0d0a 2020 2020 2020  Text.END..      
+0001f5a0: 2020 656c 6966 2070 6374 5f63 6861 6e67    elif pct_chang
+0001f5b0: 6520 3c20 2d30 2e32 3a0d 0a20 2020 2020  e < -0.2:..     
+0001f5c0: 2020 2020 2020 2070 6374 5f63 6861 6e67         pct_chang
+0001f5d0: 6520 3d20 636f 6c6f 7254 6578 742e 4641  e = colorText.FA
+0001f5e0: 494c 202b 2028 2225 2e31 6625 2522 2025  IL + ("%.1f%%" %
+0001f5f0: 2070 6374 5f63 6861 6e67 6529 202b 2063   pct_change) + c
+0001f600: 6f6c 6f72 5465 7874 2e45 4e44 0d0a 2020  olorText.END..  
+0001f610: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+0001f620: 2020 2020 2020 2020 2070 6374 5f63 6861           pct_cha
+0001f630: 6e67 6520 3d20 636f 6c6f 7254 6578 742e  nge = colorText.
+0001f640: 5741 524e 202b 2028 2225 2e31 6625 2522  WARN + ("%.1f%%"
+0001f650: 2025 2070 6374 5f63 6861 6e67 6529 202b   % pct_change) +
+0001f660: 2063 6f6c 6f72 5465 7874 2e45 4e44 0d0a   colorText.END..
+0001f670: 2020 2020 2020 2020 7361 7665 4469 6374          saveDict
+0001f680: 5b22 2543 686e 6722 5d20 3d20 7063 745f  ["%Chng"] = pct_
+0001f690: 7361 7665 0d0a 2020 2020 2020 2020 7363  save..        sc
+0001f6a0: 7265 656e 4469 6374 5b22 2543 686e 6722  reenDict["%Chng"
+0001f6b0: 5d20 3d20 7063 745f 6368 616e 6765 0d0a  ] = pct_change..
+0001f6c0: 2020 2020 2020 2020 6c74 7020 3d20 726f          ltp = ro
+0001f6d0: 756e 6428 7265 6365 6e74 5b22 436c 6f73  und(recent["Clos
+0001f6e0: 6522 5d2e 696c 6f63 5b30 5d2c 2032 290d  e"].iloc[0], 2).
+0001f6f0: 0a20 2020 2020 2020 2076 6572 6966 7953  .        verifyS
+0001f700: 7461 6765 5477 6f20 3d20 5472 7565 0d0a  tageTwo = True..
+0001f710: 2020 2020 2020 2020 6966 206c 656e 2864          if len(d
+0001f720: 6174 6129 203e 2032 3530 3a0d 0a20 2020  ata) > 250:..   
+0001f730: 2020 2020 2020 2020 2079 6561 726c 794c           yearlyL
+0001f740: 6f77 203d 2064 6174 612e 6865 6164 2832  ow = data.head(2
+0001f750: 3530 295b 2243 6c6f 7365 225d 2e6d 696e  50)["Close"].min
+0001f760: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
+0001f770: 7965 6172 6c79 4869 6768 203d 2064 6174  yearlyHigh = dat
+0001f780: 612e 6865 6164 2832 3530 295b 2243 6c6f  a.head(250)["Clo
+0001f790: 7365 225d 2e6d 6178 2829 0d0a 2020 2020  se"].max()..    
+0001f7a0: 2020 2020 2020 2020 6966 206c 7470 203c          if ltp <
+0001f7b0: 2028 3220 2a20 7965 6172 6c79 4c6f 7729   (2 * yearlyLow)
+0001f7c0: 2061 6e64 206c 7470 203c 2028 302e 3735   and ltp < (0.75
+0001f7d0: 202a 2079 6561 726c 7948 6967 6829 3a0d   * yearlyHigh):.
+0001f7e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001f7f0: 2076 6572 6966 7953 7461 6765 5477 6f20   verifyStageTwo 
+0001f800: 3d20 4661 6c73 650d 0a20 2020 2020 2020  = False..       
+0001f810: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
+0001f820: 6963 745b 2253 746f 636b 225d 203d 2063  ict["Stock"] = c
+0001f830: 6f6c 6f72 5465 7874 2e46 4149 4c20 2b20  olorText.FAIL + 
+0001f840: 7361 7665 4469 6374 5b22 5374 6f63 6b22  saveDict["Stock"
+0001f850: 5d20 2b20 636f 6c6f 7254 6578 742e 454e  ] + colorText.EN
+0001f860: 440d 0a20 2020 2020 2020 2069 6620 6c74  D..        if lt
+0001f870: 7020 3e3d 206d 696e 4c54 5020 616e 6420  p >= minLTP and 
+0001f880: 6c74 7020 3c3d 206d 6178 4c54 503a 0d0a  ltp <= maxLTP:..
+0001f890: 2020 2020 2020 2020 2020 2020 6c74 7056              ltpV
+0001f8a0: 616c 6964 203d 2054 7275 650d 0a20 2020  alid = True..   
+0001f8b0: 2020 2020 2020 2020 2069 6620 6d69 6e43           if minC
+0001f8c0: 6861 6e67 6520 213d 2030 3a0d 0a20 2020  hange != 0:..   
+0001f8d0: 2020 2020 2020 2020 2020 2020 2023 2055               # U
+0001f8e0: 7365 7220 6861 7320 7375 7070 6c69 6564  ser has supplied
+0001f8f0: 2073 6f6d 6520 6669 6c74 6572 2066 6f72   some filter for
+0001f900: 2070 6572 6365 6e74 6167 6520 6368 616e   percentage chan
+0001f910: 6765 0d0a 2020 2020 2020 2020 2020 2020  ge..            
+0001f920: 2020 2020 6c74 7056 616c 6964 203d 2066      ltpValid = f
+0001f930: 6c6f 6174 2873 7472 2870 6374 5f73 6176  loat(str(pct_sav
+0001f940: 6529 2e72 6570 6c61 6365 2822 2522 2c22  e).replace("%","
+0001f950: 2229 2920 3e3d 206d 696e 4368 616e 6765  ")) >= minChange
+0001f960: 0d0a 2020 2020 2020 2020 2020 2020 7361  ..            sa
+0001f970: 7665 4469 6374 5b22 4c54 5022 5d20 3d20  veDict["LTP"] = 
+0001f980: 726f 756e 6428 6c74 702c 2032 290d 0a20  round(ltp, 2).. 
+0001f990: 2020 2020 2020 2020 2020 2073 6372 6565             scree
+0001f9a0: 6e44 6963 745b 224c 5450 225d 203d 2028  nDict["LTP"] = (
+0001f9b0: 636f 6c6f 7254 6578 742e 4752 4545 4e20  colorText.GREEN 
+0001f9c0: 6966 206c 7470 5661 6c69 6420 656c 7365  if ltpValid else
+0001f9d0: 2063 6f6c 6f72 5465 7874 2e46 4149 4c29   colorText.FAIL)
+0001f9e0: 202b 2028 2225 2e32 6622 2025 206c 7470   + ("%.2f" % ltp
+0001f9f0: 2920 2b20 636f 6c6f 7254 6578 742e 454e  ) + colorText.EN
+0001fa00: 440d 0a20 2020 2020 2020 2020 2020 2072  D..            r
+0001fa10: 6574 7572 6e20 6c74 7056 616c 6964 2c20  eturn ltpValid, 
+0001fa20: 7665 7269 6679 5374 6167 6554 776f 0d0a  verifyStageTwo..
+0001fa30: 2020 2020 2020 2020 7363 7265 656e 4469          screenDi
+0001fa40: 6374 5b22 4c54 5022 5d20 3d20 636f 6c6f  ct["LTP"] = colo
+0001fa50: 7254 6578 742e 4641 494c 202b 2028 2225  rText.FAIL + ("%
+0001fa60: 2e32 6622 2025 206c 7470 2920 2b20 636f  .2f" % ltp) + co
+0001fa70: 6c6f 7254 6578 742e 454e 440d 0a20 2020  lorText.END..   
+0001fa80: 2020 2020 2073 6176 6544 6963 745b 224c       saveDict["L
+0001fa90: 5450 225d 203d 2072 6f75 6e64 286c 7470  TP"] = round(ltp
+0001faa0: 2c20 3229 0d0a 2020 2020 2020 2020 7265  , 2)..        re
+0001fab0: 7475 726e 206c 7470 5661 6c69 642c 2076  turn ltpValid, v
+0001fac0: 6572 6966 7953 7461 6765 5477 6f0d 0a0d  erifyStageTwo...
+0001fad0: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+0001fae0: 654c 5450 466f 7250 6f72 7466 6f6c 696f  eLTPForPortfolio
+0001faf0: 4361 6c63 2873 656c 662c 2064 662c 2073  Calc(self, df, s
+0001fb00: 6372 6565 6e44 6963 742c 2073 6176 6544  creenDict, saveD
+0001fb10: 6963 742c 7265 7175 6573 7465 6450 6572  ict,requestedPer
+0001fb20: 696f 643d 3029 3a0d 0a20 2020 2020 2020  iod=0):..       
+0001fb30: 2064 6174 6120 3d20 6466 2e63 6f70 7928   data = df.copy(
+0001fb40: 290d 0a20 2020 2020 2020 2070 6572 696f  )..        perio
+0001fb50: 6473 203d 2073 656c 662e 636f 6e66 6967  ds = self.config
+0001fb60: 4d61 6e61 6765 722e 7065 7269 6f64 7352  Manager.periodsR
+0001fb70: 616e 6765 0d0a 2020 2020 2020 2020 6966  ange..        if
+0001fb80: 2072 6571 7565 7374 6564 5065 7269 6f64   requestedPeriod
+0001fb90: 203e 2030 2061 6e64 2072 6571 7565 7374   > 0 and request
+0001fba0: 6564 5065 7269 6f64 206e 6f74 2069 6e20  edPeriod not in 
+0001fbb0: 7065 7269 6f64 733a 0d0a 2020 2020 2020  periods:..      
+0001fbc0: 2020 2020 2020 7065 7269 6f64 732e 6170        periods.ap
+0001fbd0: 7065 6e64 2872 6571 7565 7374 6564 5065  pend(requestedPe
+0001fbe0: 7269 6f64 290d 0a20 2020 2020 2020 2070  riod)..        p
+0001fbf0: 7265 7669 6f75 735f 7265 6365 6e74 203d  revious_recent =
+0001fc00: 2064 6174 612e 6865 6164 2831 290d 0a20   data.head(1).. 
+0001fc10: 2020 2020 2020 2070 7265 7669 6f75 735f         previous_
+0001fc20: 7265 6365 6e74 2e72 6573 6574 5f69 6e64  recent.reset_ind
+0001fc30: 6578 2869 6e70 6c61 6365 3d54 7275 6529  ex(inplace=True)
+0001fc40: 0d0a 2020 2020 2020 2020 6361 6c63 5f64  ..        calc_d
+0001fc50: 6174 6520 3d20 7374 7228 7072 6576 696f  ate = str(previo
+0001fc60: 7573 5f72 6563 656e 742e 696c 6f63 5b3a  us_recent.iloc[:
+0001fc70: 2c20 305d 5b30 5d29 2e73 706c 6974 2822  , 0][0]).split("
+0001fc80: 2022 295b 305d 0d0a 2020 2020 2020 2020   ")[0]..        
+0001fc90: 666f 7220 7072 6420 696e 2070 6572 696f  for prd in perio
+0001fca0: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
+0001fcb0: 2069 6620 6c65 6e28 6461 7461 2920 3e3d   if len(data) >=
+0001fcc0: 2070 7264 202b 2031 3a0d 0a20 2020 2020   prd + 1:..     
+0001fcd0: 2020 2020 2020 2020 2020 2070 7265 764c             prevL
+0001fce0: 7470 203d 2064 6174 615b 2243 6c6f 7365  tp = data["Close
+0001fcf0: 225d 2e69 6c6f 635b 305d 0d0a 2020 2020  "].iloc[0]..    
+0001fd00: 2020 2020 2020 2020 2020 2020 6c74 7054              ltpT
+0001fd10: 6479 203d 2064 6174 615b 2243 6c6f 7365  dy = data["Close
+0001fd20: 225d 2e69 6c6f 635b 7072 645d 0d0a 2020  "].iloc[prd]..  
+0001fd30: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0001fd40: 2069 7369 6e73 7461 6e63 6528 7072 6576   isinstance(prev
+0001fd50: 4c74 702c 7064 2e53 6572 6965 7329 3a0d  Ltp,pd.Series):.
+0001fd60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001fd70: 2020 2020 2070 7265 764c 7470 203d 2070       prevLtp = p
+0001fd80: 7265 764c 7470 5b30 5d0d 0a20 2020 2020  revLtp[0]..     
+0001fd90: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+0001fda0: 7470 5464 7920 3d20 6c74 7054 6479 5b30  tpTdy = ltpTdy[0
+0001fdb0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+0001fdc0: 2020 2073 6372 6565 6e44 6963 745b 6622     screenDict[f"
+0001fdd0: 4c54 507b 7072 647d 225d 203d 2028 0d0a  LTP{prd}"] = (..
+0001fde0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001fdf0: 2020 2020 2863 6f6c 6f72 5465 7874 2e47      (colorText.G
+0001fe00: 5245 454e 2069 6620 286c 7470 5464 7920  REEN if (ltpTdy 
+0001fe10: 3e3d 2070 7265 764c 7470 2920 656c 7365  >= prevLtp) else
+0001fe20: 2028 636f 6c6f 7254 6578 742e 4641 494c   (colorText.FAIL
+0001fe30: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+0001fe40: 2020 2020 2020 2020 2b20 7374 7228 227b          + str("{
+0001fe50: 3a2e 3266 7d22 2e66 6f72 6d61 7428 6c74  :.2f}".format(lt
+0001fe60: 7054 6479 2929 0d0a 2020 2020 2020 2020  pTdy))..        
+0001fe70: 2020 2020 2020 2020 2020 2020 2b20 636f              + co
+0001fe80: 6c6f 7254 6578 742e 454e 440d 0a20 2020  lorText.END..   
+0001fe90: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
+0001fea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001feb0: 7363 7265 656e 4469 6374 5b66 2247 726f  screenDict[f"Gro
+0001fec0: 7774 687b 7072 647d 225d 203d 2028 0d0a  wth{prd}"] = (..
+0001fed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001fee0: 2020 2020 2863 6f6c 6f72 5465 7874 2e47      (colorText.G
+0001fef0: 5245 454e 2069 6620 286c 7470 5464 7920  REEN if (ltpTdy 
+0001ff00: 3e3d 2070 7265 764c 7470 2920 656c 7365  >= prevLtp) else
+0001ff10: 2028 636f 6c6f 7254 6578 742e 4641 494c   (colorText.FAIL
+0001ff20: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+0001ff30: 2020 2020 2020 2020 2b20 7374 7228 227b          + str("{
+0001ff40: 3a2e 3266 7d22 2e66 6f72 6d61 7428 6c74  :.2f}".format(lt
+0001ff50: 7054 6479 202d 2070 7265 764c 7470 2929  pTdy - prevLtp))
+0001ff60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001ff70: 2020 2020 2020 2b20 636f 6c6f 7254 6578        + colorTex
+0001ff80: 742e 454e 440d 0a20 2020 2020 2020 2020  t.END..         
+0001ff90: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+0001ffa0: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
+0001ffb0: 6374 5b66 224c 5450 7b70 7264 7d22 5d20  ct[f"LTP{prd}"] 
+0001ffc0: 3d20 726f 756e 6428 6c74 7054 6479 2c20  = round(ltpTdy, 
+0001ffd0: 3229 0d0a 2020 2020 2020 2020 2020 2020  2)..            
+0001ffe0: 2020 2020 7361 7665 4469 6374 5b66 2247      saveDict[f"G
+0001fff0: 726f 7774 687b 7072 647d 225d 203d 2072  rowth{prd}"] = r
+00020000: 6f75 6e64 286c 7470 5464 7920 2d20 7072  ound(ltpTdy - pr
+00020010: 6576 4c74 702c 2032 290d 0a20 2020 2020  evLtp, 2)..     
+00020020: 2020 2020 2020 2020 2020 2069 6620 7072             if pr
+00020030: 6420 3d3d 2032 3220 6f72 2028 7072 6420  d == 22 or (prd 
+00020040: 3d3d 2072 6571 7565 7374 6564 5065 7269  == requestedPeri
+00020050: 6f64 293a 0d0a 2020 2020 2020 2020 2020  od):..          
+00020060: 2020 2020 2020 2020 2020 6368 616e 6765            change
+00020070: 5065 7263 656e 7420 3d20 726f 756e 6428  Percent = round(
+00020080: 2828 7072 6576 4c74 702d 6c74 7054 6479  ((prevLtp-ltpTdy
+00020090: 2920 6966 2072 6571 7565 7374 6564 5065  ) if requestedPe
+000200a0: 7269 6f64 203d 3d30 2065 6c73 6520 286c  riod ==0 else (l
+000200b0: 7470 5464 7920 2d20 7072 6576 4c74 7029  tpTdy - prevLtp)
+000200c0: 292a 3130 302f 6c74 7054 6479 2c20 3229  )*100/ltpTdy, 2)
+000200d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000200e0: 2020 2020 2020 7361 7665 4469 6374 5b66        saveDict[f
+000200f0: 227b 7072 647d 2d50 6420 2522 5d20 3d20  "{prd}-Pd %"] = 
+00020100: 6622 7b63 6861 6e67 6550 6572 6365 6e74  f"{changePercent
+00020110: 7d25 220d 0a20 2020 2020 2020 2020 2020  }%"..           
+00020120: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
+00020130: 6963 745b 6622 7b70 7264 7d2d 5064 2025  ict[f"{prd}-Pd %
+00020140: 225d 203d 2028 636f 6c6f 7254 6578 742e  "] = (colorText.
+00020150: 4752 4545 4e20 6966 2063 6861 6e67 6550  GREEN if changeP
+00020160: 6572 6365 6e74 203e 3d30 2065 6c73 6520  ercent >=0 else 
+00020170: 636f 6c6f 7254 6578 742e 4641 494c 2920  colorText.FAIL) 
+00020180: 2b20 6622 7b63 6861 6e67 6550 6572 6365  + f"{changePerce
+00020190: 6e74 7d25 2220 2b20 636f 6c6f 7254 6578  nt}%" + colorTex
+000201a0: 742e 454e 440d 0a20 2020 2020 2020 2020  t.END..         
+000201b0: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
+000201c0: 745b 2244 6174 6522 5d20 3d20 6361 6c63  t["Date"] = calc
+000201d0: 5f64 6174 650d 0a20 2020 2020 2020 2020  _date..         
+000201e0: 2020 2020 2020 2073 6176 6544 6963 745b         saveDict[
+000201f0: 2244 6174 6522 5d20 3d20 6361 6c63 5f64  "Date"] = calc_d
+00020200: 6174 650d 0a20 2020 2020 2020 2020 2020  ate..           
+00020210: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+00020220: 2020 2020 2020 2020 7361 7665 4469 6374          saveDict
+00020230: 5b66 224c 5450 7b70 7264 7d22 5d20 3d20  [f"LTP{prd}"] = 
+00020240: 6e70 2e6e 616e 0d0a 2020 2020 2020 2020  np.nan..        
+00020250: 2020 2020 2020 2020 7361 7665 4469 6374          saveDict
+00020260: 5b66 2247 726f 7774 687b 7072 647d 225d  [f"Growth{prd}"]
+00020270: 203d 206e 702e 6e61 6e0d 0a20 2020 2020   = np.nan..     
+00020280: 2020 2020 2020 2020 2020 2073 6372 6565             scree
+00020290: 6e44 6963 745b 2244 6174 6522 5d20 3d20  nDict["Date"] = 
+000202a0: 6361 6c63 5f64 6174 650d 0a20 2020 2020  calc_date..     
+000202b0: 2020 2020 2020 2020 2020 2073 6176 6544             saveD
+000202c0: 6963 745b 2244 6174 6522 5d20 3d20 6361  ict["Date"] = ca
+000202d0: 6c63 5f64 6174 650d 0a0d 0a20 2020 2023  lc_date....    #
+000202e0: 2046 696e 6420 7374 6f63 6b73 2074 6861   Find stocks tha
+000202f0: 7420 6172 6520 6265 6172 6973 6820 696e  t are bearish in
+00020300: 7472 6164 6179 3a20 4d61 6364 2048 6973  traday: Macd His
+00020310: 746f 6772 616d 206e 6567 6174 6976 650d  togram negative.
+00020320: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+00020330: 654d 4143 4448 6973 746f 6772 616d 4265  eMACDHistogramBe
+00020340: 6c6f 7730 2873 656c 662c 2064 6629 3a0d  low0(self, df):.
+00020350: 0a20 2020 2020 2020 2069 6620 6466 2069  .        if df i
+00020360: 7320 4e6f 6e65 206f 7220 6c65 6e28 6466  s None or len(df
+00020370: 2920 3d3d 2030 3a0d 0a20 2020 2020 2020  ) == 0:..       
+00020380: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+00020390: 650d 0a20 2020 2020 2020 2064 6174 6120  e..        data 
+000203a0: 3d20 6466 2e63 6f70 7928 290d 0a20 2020  = df.copy()..   
+000203b0: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
+000203c0: 2e66 696c 6c6e 6128 3029 0d0a 2020 2020  .fillna(0)..    
+000203d0: 2020 2020 6461 7461 203d 2064 6174 612e      data = data.
+000203e0: 7265 706c 6163 6528 5b6e 702e 696e 662c  replace([np.inf,
+000203f0: 202d 6e70 2e69 6e66 5d2c 2030 290d 0a20   -np.inf], 0).. 
+00020400: 2020 2020 2020 2064 6174 6120 3d20 6461         data = da
+00020410: 7461 5b3a 3a2d 315d 2020 2320 5265 7665  ta[::-1]  # Reve
+00020420: 7273 6520 7468 6520 6461 7461 6672 616d  rse the datafram
+00020430: 6520 736f 2074 6861 7420 6974 7320 7468  e so that its th
+00020440: 6520 6f6c 6465 7374 2064 6174 6520 6669  e oldest date fi
+00020450: 7273 740d 0a20 2020 2020 2020 206d 6163  rst..        mac
+00020460: 6420 3d20 706b 7461 6c69 622e 4d41 4344  d = pktalib.MACD
+00020470: 2864 6174 615b 2243 6c6f 7365 225d 2c20  (data["Close"], 
+00020480: 3132 2c20 3236 2c20 3929 5b32 5d2e 7461  12, 26, 9)[2].ta
+00020490: 696c 2831 290d 0a20 2020 2020 2020 2072  il(1)..        r
+000204a0: 6574 7572 6e20 6d61 6364 2e69 6c6f 635b  eturn macd.iloc[
+000204b0: 3a31 5d5b 305d 203c 2030 0d0a 0d0a 2020  :1][0] < 0....  
+000204c0: 2020 2340 6d65 6173 7572 655f 7469 6d65    #@measure_time
+000204d0: 0d0a 2020 2020 2320 4669 6e64 2069 6620  ..    # Find if 
+000204e0: 7374 6f63 6b20 6761 696e 696e 6720 6275  stock gaining bu
+000204f0: 6c6c 6973 6820 6d6f 6d65 6e74 756d 0d0a  llish momentum..
+00020500: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+00020510: 4d6f 6d65 6e74 756d 2873 656c 662c 2064  Momentum(self, d
+00020520: 662c 2073 6372 6565 6e44 6963 742c 2073  f, screenDict, s
+00020530: 6176 6544 6963 7429 3a0d 0a20 2020 2020  aveDict):..     
+00020540: 2020 2069 6620 6466 2069 7320 4e6f 6e65     if df is None
+00020550: 206f 7220 6c65 6e28 6466 2920 3d3d 2030   or len(df) == 0
+00020560: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+00020570: 6574 7572 6e20 4661 6c73 650d 0a20 2020  eturn False..   
+00020580: 2020 2020 2064 6174 6120 3d20 6466 2e63       data = df.c
+00020590: 6f70 7928 290d 0a20 2020 2020 2020 2074  opy()..        t
+000205a0: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
+000205b0: 2064 6174 6120 3d20 6461 7461 2e68 6561   data = data.hea
+000205c0: 6428 3329 0d0a 2020 2020 2020 2020 2020  d(3)..          
+000205d0: 2020 6966 206c 656e 2864 6174 6129 203c    if len(data) <
+000205e0: 2033 3a0d 0a20 2020 2020 2020 2020 2020   3:..           
+000205f0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+00020600: 650d 0a20 2020 2020 2020 2020 2020 2066  e..            f
+00020610: 6f72 2072 6f77 2069 6e20 6461 7461 2e69  or row in data.i
+00020620: 7465 7272 6f77 7328 293a 0d0a 2020 2020  terrows():..    
+00020630: 2020 2020 2020 2020 2020 2020 2320 416c              # Al
+00020640: 6c20 3320 6361 6e64 6c65 7320 7368 6f75  l 3 candles shou
+00020650: 6c64 2062 6520 4772 6565 6e20 616e 6420  ld be Green and 
+00020660: 4e4f 5420 4369 7263 7569 7473 0d0a 2020  NOT Circuits..  
+00020670: 2020 2020 2020 2020 2020 2020 2020 7963                yc
+00020680: 203d 2072 6f77 5b31 5d5b 2243 6c6f 7365   = row[1]["Close
+00020690: 225d 0d0a 2020 2020 2020 2020 2020 2020  "]..            
+000206a0: 2020 2020 796f 203d 2072 6f77 5b31 5d5b      yo = row[1][
+000206b0: 224f 7065 6e22 5d0d 0a20 2020 2020 2020  "Open"]..       
+000206c0: 2020 2020 2020 2020 2069 6620 7963 203c           if yc <
+000206d0: 3d20 796f 3a0d 0a20 2020 2020 2020 2020  = yo:..         
+000206e0: 2020 2020 2020 2020 2020 2023 2073 656c             # sel
+000206f0: 662e 6465 6661 756c 745f 6c6f 6767 6572  f.default_logger
+00020700: 2e69 6e66 6f28 0d0a 2020 2020 2020 2020  .info(..        
+00020710: 2020 2020 2020 2020 2020 2020 2320 2020              #   
+00020720: 2020 6627 5374 6f63 6b3a 7b73 6176 6544    f'Stock:{saveD
+00020730: 6963 745b 2253 746f 636b 225d 7d2c 2069  ict["Stock"]}, i
+00020740: 7320 6e6f 7420 6120 6d6f 6d65 6e74 756d  s not a momentum
+00020750: 2d67 6169 6e65 7220 6265 6361 7573 6520  -gainer because 
+00020760: 7965 7374 6572 6461 792d 636c 6f73 6520  yesterday-close 
+00020770: 287b 7963 7d29 203c 3d20 7965 7374 6572  ({yc}) <= yester
+00020780: 6461 792d 6f70 656e 2028 7b79 6f7d 2927  day-open ({yo})'
+00020790: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000207a0: 2020 2020 2020 2320 290d 0a20 2020 2020        # )..     
+000207b0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+000207c0: 6574 7572 6e20 4661 6c73 650d 0a20 2020  eturn False..   
+000207d0: 2020 2020 2020 2020 206f 7065 6e44 6573           openDes
+000207e0: 6320 3d20 6461 7461 2e73 6f72 745f 7661  c = data.sort_va
+000207f0: 6c75 6573 2862 793d 5b22 4f70 656e 225d  lues(by=["Open"]
+00020800: 2c20 6173 6365 6e64 696e 673d 4661 6c73  , ascending=Fals
+00020810: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
+00020820: 636c 6f73 6544 6573 6320 3d20 6461 7461  closeDesc = data
+00020830: 2e73 6f72 745f 7661 6c75 6573 2862 793d  .sort_values(by=
+00020840: 5b22 436c 6f73 6522 5d2c 2061 7363 656e  ["Close"], ascen
+00020850: 6469 6e67 3d46 616c 7365 290d 0a20 2020  ding=False)..   
+00020860: 2020 2020 2020 2020 2076 6f6c 4465 7363           volDesc
+00020870: 203d 2064 6174 612e 736f 7274 5f76 616c   = data.sort_val
+00020880: 7565 7328 6279 3d5b 2256 6f6c 756d 6522  ues(by=["Volume"
+00020890: 5d2c 2061 7363 656e 6469 6e67 3d46 616c  ], ascending=Fal
+000208a0: 7365 290d 0a20 2020 2020 2020 2020 2020  se)..           
+000208b0: 2074 7279 3a0d 0a20 2020 2020 2020 2020   try:..         
+000208c0: 2020 2020 2020 2069 6620 280d 0a20 2020         if (..   
+000208d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000208e0: 2064 6174 612e 6571 7561 6c73 286f 7065   data.equals(ope
+000208f0: 6e44 6573 6329 0d0a 2020 2020 2020 2020  nDesc)..        
+00020900: 2020 2020 2020 2020 2020 2020 616e 6420              and 
+00020910: 6461 7461 2e65 7175 616c 7328 636c 6f73  data.equals(clos
+00020920: 6544 6573 6329 0d0a 2020 2020 2020 2020  eDesc)..        
+00020930: 2020 2020 2020 2020 2020 2020 616e 6420              and 
+00020940: 6461 7461 2e65 7175 616c 7328 766f 6c44  data.equals(volD
+00020950: 6573 6329 0d0a 2020 2020 2020 2020 2020  esc)..          
+00020960: 2020 2020 2020 293a 0d0a 2020 2020 2020        ):..      
+00020970: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00020980: 7365 6c66 2e64 6566 6175 6c74 5f6c 6f67  self.default_log
+00020990: 6765 722e 696e 666f 280d 0a20 2020 2020  ger.info(..     
+000209a0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+000209b0: 2020 2020 2066 2753 746f 636b 3a7b 7361       f'Stock:{sa
+000209c0: 7665 4469 6374 5b22 5374 6f63 6b22 5d7d  veDict["Stock"]}
+000209d0: 2c20 6f70 656e 2c63 6c6f 7365 2061 6e64  , open,close and
+000209e0: 2076 6f6c 756d 6520 6571 7561 6c20 6672   volume equal fr
+000209f0: 6f6d 2064 6179 2062 6566 6f72 6520 7965  om day before ye
+00020a00: 7374 6572 6461 792e 2041 2070 6f74 656e  sterday. A poten
+00020a10: 7469 616c 206d 6f6d 656e 7475 6d2d 6761  tial momentum-ga
+00020a20: 696e 6572 2127 0d0a 2020 2020 2020 2020  iner!'..        
+00020a30: 2020 2020 2020 2020 2020 2020 2320 290d              # ).
+00020a40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00020a50: 2020 2020 2074 6f20 3d20 6461 7461 5b22       to = data["
+00020a60: 4f70 656e 225d 2e69 6c6f 635b 305d 0d0a  Open"].iloc[0]..
 00020a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020a80: 2020 2020 2b20 636f 6c6f 7254 6578 742e      + colorText.
-00020a90: 424f 4c44 0d0a 2020 2020 2020 2020 2020  BOLD..          
+00020a80: 2020 2020 7963 203d 2064 6174 615b 2243      yc = data["C
+00020a90: 6c6f 7365 225d 2e69 6c6f 635b 315d 0d0a  lose"].iloc[1]..
 00020aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020ab0: 2020 2b20 636f 6c6f 7254 6578 742e 4752    + colorText.GR
-00020ac0: 4545 4e0d 0a20 2020 2020 2020 2020 2020  EEN..           
+00020ab0: 2020 2020 796f 203d 2064 6174 615b 224f      yo = data["O
+00020ac0: 7065 6e22 5d2e 696c 6f63 5b31 5d0d 0a20  pen"].iloc[1].. 
 00020ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020ae0: 202b 2022 4d6f 6d65 6e74 756d 2047 6169   + "Momentum Gai
-00020af0: 6e65 7222 0d0a 2020 2020 2020 2020 2020  ner"..          
+00020ae0: 2020 2064 7963 203d 2064 6174 615b 2243     dyc = data["C
+00020af0: 6c6f 7365 225d 2e69 6c6f 635b 325d 0d0a  lose"].iloc[2]..
 00020b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020b10: 2020 2b20 636f 6c6f 7254 6578 742e 454e    + colorText.EN
-00020b20: 440d 0a20 2020 2020 2020 2020 2020 2020  D..             
-00020b30: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
-00020b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020b50: 2020 2020 2020 7361 7665 4469 6374 5b22        saveDict["
-00020b60: 5061 7474 6572 6e22 5d20 3d20 7361 7665  Pattern"] = save
-00020b70: 645b 315d 202b 2022 4d6f 6d65 6e74 756d  d[1] + "Momentum
-00020b80: 2047 6169 6e65 7222 0d0a 2020 2020 2020   Gainer"..      
-00020b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020ba0: 2020 7265 7475 726e 2054 7275 650d 0a20    return True.. 
-00020bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020bc0: 2020 2023 2073 656c 662e 6465 6661 756c     # self.defaul
-00020bd0: 745f 6c6f 6767 6572 2e69 6e66 6f28 0d0a  t_logger.info(..
-00020be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020bf0: 2020 2020 2320 2020 2020 6627 5374 6f63      #     f'Stoc
-00020c00: 6b3a 7b73 6176 6544 6963 745b 2253 746f  k:{saveDict["Sto
-00020c10: 636b 225d 7d2c 2069 7320 6e6f 7420 6120  ck"]}, is not a 
-00020c20: 6d6f 6d65 6e74 756d 2d67 6169 6e65 7220  momentum-gainer 
-00020c30: 6265 6361 7573 6520 6569 7468 6572 2074  because either t
-00020c40: 6f64 6179 2d6f 7065 6e20 287b 746f 7d29  oday-open ({to})
-00020c50: 203c 2079 6573 7465 7264 6179 2d63 6c6f   < yesterday-clo
-00020c60: 7365 2028 7b79 637d 2920 6f72 2079 6573  se ({yc}) or yes
-00020c70: 7465 7264 6179 2d6f 7065 6e28 7b79 6f7d  terday-open({yo}
-00020c80: 2920 3c20 6461 792d 6265 666f 7265 2d63  ) < day-before-c
-00020c90: 6c6f 7365 287b 6479 637d 2927 0d0a 2020  lose({dyc})'..  
+00020b10: 2020 2020 6966 2028 746f 203e 3d20 7963      if (to >= yc
+00020b20: 2920 616e 6420 2879 6f20 3e3d 2064 7963  ) and (yo >= dyc
+00020b30: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00020b40: 2020 2020 2020 2020 2020 2020 2320 7365              # se
+00020b50: 6c66 2e64 6566 6175 6c74 5f6c 6f67 6765  lf.default_logge
+00020b60: 722e 696e 666f 280d 0a20 2020 2020 2020  r.info(..       
+00020b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020b80: 2023 2020 2020 2066 2753 746f 636b 3a7b   #     f'Stock:{
+00020b90: 7361 7665 4469 6374 5b22 5374 6f63 6b22  saveDict["Stock"
+00020ba0: 5d7d 2c20 6973 2061 206d 6f6d 656e 7475  ]}, is a momentu
+00020bb0: 6d2d 6761 696e 6572 2062 6563 6175 7365  m-gainer because
+00020bc0: 2074 6f64 6179 2d6f 7065 6e20 287b 746f   today-open ({to
+00020bd0: 7d29 203e 3d20 7965 7374 6572 6461 792d  }) >= yesterday-
+00020be0: 636c 6f73 6520 287b 7963 7d29 2061 6e64  close ({yc}) and
+00020bf0: 2079 6573 7465 7264 6179 2d6f 7065 6e28   yesterday-open(
+00020c00: 7b79 6f7d 2920 3e3d 2064 6179 2d62 6566  {yo}) >= day-bef
+00020c10: 6f72 652d 636c 6f73 6528 7b64 7963 7d29  ore-close({dyc})
+00020c20: 270d 0a20 2020 2020 2020 2020 2020 2020  '..             
+00020c30: 2020 2020 2020 2020 2020 2023 2029 0d0a             # )..
+00020c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020c50: 2020 2020 2020 2020 7361 7665 6420 3d20          saved = 
+00020c60: 7365 6c66 2e66 696e 6443 7572 7265 6e74  self.findCurrent
+00020c70: 5361 7665 6456 616c 7565 2873 6372 6565  SavedValue(scree
+00020c80: 6e44 6963 742c 2073 6176 6544 6963 742c  nDict, saveDict,
+00020c90: 2022 5061 7474 6572 6e22 290d 0a20 2020   "Pattern")..   
 00020ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020cb0: 2020 2320 290d 0a20 2020 2020 2020 2020    # )..         
-00020cc0: 2020 2065 7863 6570 7420 496e 6465 7845     except IndexE
-00020cd0: 7272 6f72 2061 7320 653a 2023 2070 7261  rror as e: # pra
-00020ce0: 676d 613a 206e 6f20 636f 7665 720d 0a20  gma: no cover.. 
-00020cf0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00020d00: 656c 662e 6465 6661 756c 745f 6c6f 6767  elf.default_logg
-00020d10: 6572 2e64 6562 7567 2865 2c20 6578 635f  er.debug(e, exc_
-00020d20: 696e 666f 3d54 7275 6529 0d0a 2020 2020  info=True)..    
-00020d30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00020d40: 2e64 6566 6175 6c74 5f6c 6f67 6765 722e  .default_logger.
-00020d50: 6465 6275 6728 6461 7461 290d 0a20 2020  debug(data)..   
-00020d60: 2020 2020 2020 2020 2020 2020 2070 6173               pas
-00020d70: 730d 0a20 2020 2020 2020 2020 2020 2072  s..            r
-00020d80: 6574 7572 6e20 4661 6c73 650d 0a20 2020  eturn False..   
-00020d90: 2020 2020 2065 7863 6570 7420 4578 6365       except Exce
-00020da0: 7074 696f 6e20 6173 2065 3a20 2023 2070  ption as e:  # p
-00020db0: 7261 676d 613a 206e 6f20 636f 7665 720d  ragma: no cover.
-00020dc0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00020dd0: 662e 6465 6661 756c 745f 6c6f 6767 6572  f.default_logger
-00020de0: 2e64 6562 7567 2865 2c20 6578 635f 696e  .debug(e, exc_in
-00020df0: 666f 3d54 7275 6529 0d0a 2020 2020 2020  fo=True)..      
-00020e00: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-00020e10: 7365 0d0a 0d0a 2020 2020 2340 6d65 6173  se....    #@meas
-00020e20: 7572 655f 7469 6d65 0d0a 2020 2020 2320  ure_time..    # 
-00020e30: 5661 6c69 6461 7465 204d 6f76 696e 6720  Validate Moving 
-00020e40: 6176 6572 6167 6573 2061 6e64 206c 6f6f  averages and loo
-00020e50: 6b20 666f 7220 6275 792f 7365 6c6c 2073  k for buy/sell s
-00020e60: 6967 6e61 6c73 0d0a 2020 2020 6465 6620  ignals..    def 
-00020e70: 7661 6c69 6461 7465 4d6f 7669 6e67 4176  validateMovingAv
-00020e80: 6572 6167 6573 2873 656c 662c 2064 662c  erages(self, df,
-00020e90: 2073 6372 6565 6e44 6963 742c 2073 6176   screenDict, sav
-00020ea0: 6544 6963 742c 206d 6152 616e 6765 3d32  eDict, maRange=2
-00020eb0: 2e35 293a 0d0a 2020 2020 2020 2020 6461  .5):..        da
-00020ec0: 7461 203d 2064 662e 636f 7079 2829 0d0a  ta = df.copy()..
-00020ed0: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
-00020ee0: 6174 612e 6669 6c6c 6e61 2830 290d 0a20  ata.fillna(0).. 
-00020ef0: 2020 2020 2020 2064 6174 6120 3d20 6461         data = da
-00020f00: 7461 2e72 6570 6c61 6365 285b 6e70 2e69  ta.replace([np.i
-00020f10: 6e66 2c20 2d6e 702e 696e 665d 2c20 3029  nf, -np.inf], 0)
-00020f20: 0d0a 2020 2020 2020 2020 7265 6365 6e74  ..        recent
-00020f30: 203d 2064 6174 612e 6865 6164 2831 290d   = data.head(1).
-00020f40: 0a20 2020 2020 2020 2073 6176 6564 203d  .        saved =
-00020f50: 2073 656c 662e 6669 6e64 4375 7272 656e   self.findCurren
-00020f60: 7453 6176 6564 5661 6c75 6528 7363 7265  tSavedValue(scre
-00020f70: 656e 4469 6374 2c73 6176 6544 6963 742c  enDict,saveDict,
-00020f80: 224d 412d 5369 676e 616c 2229 0d0a 2020  "MA-Signal")..  
-00020f90: 2020 2020 2020 6966 2028 0d0a 2020 2020        if (..    
-00020fa0: 2020 2020 2020 2020 7265 6365 6e74 5b22          recent["
-00020fb0: 534d 4122 5d2e 696c 6f63 5b30 5d20 3e20  SMA"].iloc[0] > 
-00020fc0: 7265 6365 6e74 5b22 4c4d 4122 5d2e 696c  recent["LMA"].il
-00020fd0: 6f63 5b30 5d0d 0a20 2020 2020 2020 2020  oc[0]..         
-00020fe0: 2020 2061 6e64 2072 6563 656e 745b 2243     and recent["C
-00020ff0: 6c6f 7365 225d 2e69 6c6f 635b 305d 203e  lose"].iloc[0] >
-00021000: 2072 6563 656e 745b 2253 4d41 225d 2e69   recent["SMA"].i
-00021010: 6c6f 635b 305d 0d0a 2020 2020 2020 2020  loc[0]..        
-00021020: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00021030: 7363 7265 656e 4469 6374 5b22 4d41 2d53  screenDict["MA-S
-00021040: 6967 6e61 6c22 5d20 3d20 280d 0a20 2020  ignal"] = (..   
-00021050: 2020 2020 2020 2020 2020 2020 2073 6176               sav
-00021060: 6564 5b30 5d20 2b20 636f 6c6f 7254 6578  ed[0] + colorTex
-00021070: 742e 424f 4c44 202b 2063 6f6c 6f72 5465  t.BOLD + colorTe
-00021080: 7874 2e47 5245 454e 202b 2022 4275 6c6c  xt.GREEN + "Bull
-00021090: 6973 6822 202b 2063 6f6c 6f72 5465 7874  ish" + colorText
-000210a0: 2e45 4e44 0d0a 2020 2020 2020 2020 2020  .END..          
-000210b0: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
-000210c0: 2073 6176 6544 6963 745b 224d 412d 5369   saveDict["MA-Si
-000210d0: 676e 616c 225d 203d 2073 6176 6564 5b31  gnal"] = saved[1
-000210e0: 5d20 2b20 2242 756c 6c69 7368 220d 0a20  ] + "Bullish".. 
-000210f0: 2020 2020 2020 2065 6c69 6620 7265 6365         elif rece
-00021100: 6e74 5b22 534d 4122 5d2e 696c 6f63 5b30  nt["SMA"].iloc[0
-00021110: 5d20 3c20 7265 6365 6e74 5b22 4c4d 4122  ] < recent["LMA"
-00021120: 5d2e 696c 6f63 5b30 5d3a 0d0a 2020 2020  ].iloc[0]:..    
-00021130: 2020 2020 2020 2020 7363 7265 656e 4469          screenDi
-00021140: 6374 5b22 4d41 2d53 6967 6e61 6c22 5d20  ct["MA-Signal"] 
-00021150: 3d20 280d 0a20 2020 2020 2020 2020 2020  = (..           
-00021160: 2020 2020 2073 6176 6564 5b30 5d20 2b20       saved[0] + 
-00021170: 636f 6c6f 7254 6578 742e 424f 4c44 202b  colorText.BOLD +
-00021180: 2063 6f6c 6f72 5465 7874 2e46 4149 4c20   colorText.FAIL 
-00021190: 2b20 2242 6561 7269 7368 2220 2b20 636f  + "Bearish" + co
-000211a0: 6c6f 7254 6578 742e 454e 440d 0a20 2020  lorText.END..   
-000211b0: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
-000211c0: 2020 2020 2020 2020 7361 7665 4469 6374          saveDict
-000211d0: 5b22 4d41 2d53 6967 6e61 6c22 5d20 3d20  ["MA-Signal"] = 
-000211e0: 7361 7665 645b 315d 202b 2022 4265 6172  saved[1] + "Bear
-000211f0: 6973 6822 0d0a 2020 2020 2020 2020 656c  ish"..        el
-00021200: 6966 2072 6563 656e 745b 2253 4d41 225d  if recent["SMA"]
-00021210: 2e69 6c6f 635b 305d 203d 3d20 303a 0d0a  .iloc[0] == 0:..
-00021220: 2020 2020 2020 2020 2020 2020 7363 7265              scre
-00021230: 656e 4469 6374 5b22 4d41 2d53 6967 6e61  enDict["MA-Signa
-00021240: 6c22 5d20 3d20 280d 0a20 2020 2020 2020  l"] = (..       
-00021250: 2020 2020 2020 2020 2073 6176 6564 5b30           saved[0
-00021260: 5d20 2b20 636f 6c6f 7254 6578 742e 424f  ] + colorText.BO
-00021270: 4c44 202b 2063 6f6c 6f72 5465 7874 2e57  LD + colorText.W
-00021280: 4152 4e20 2b20 2255 6e6b 6e6f 776e 2220  ARN + "Unknown" 
-00021290: 2b20 636f 6c6f 7254 6578 742e 454e 440d  + colorText.END.
-000212a0: 0a20 2020 2020 2020 2020 2020 2029 0d0a  .            )..
-000212b0: 2020 2020 2020 2020 2020 2020 7361 7665              save
-000212c0: 4469 6374 5b22 4d41 2d53 6967 6e61 6c22  Dict["MA-Signal"
-000212d0: 5d20 3d20 7361 7665 645b 315d 202b 2022  ] = saved[1] + "
-000212e0: 556e 6b6e 6f77 6e22 0d0a 2020 2020 2020  Unknown"..      
-000212f0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-00021300: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
-00021310: 224d 412d 5369 676e 616c 225d 203d 2028  "MA-Signal"] = (
-00021320: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00021330: 2020 7361 7665 645b 305d 202b 2063 6f6c    saved[0] + col
-00021340: 6f72 5465 7874 2e42 4f4c 4420 2b20 636f  orText.BOLD + co
-00021350: 6c6f 7254 6578 742e 5741 524e 202b 2022  lorText.WARN + "
-00021360: 4e65 7574 7261 6c22 202b 2063 6f6c 6f72  Neutral" + color
-00021370: 5465 7874 2e45 4e44 0d0a 2020 2020 2020  Text.END..      
-00021380: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-00021390: 2020 2020 2073 6176 6544 6963 745b 224d       saveDict["M
-000213a0: 412d 5369 676e 616c 225d 203d 2073 6176  A-Signal"] = sav
-000213b0: 6564 5b31 5d20 2b20 224e 6575 7472 616c  ed[1] + "Neutral
-000213c0: 220d 0a0d 0a20 2020 2020 2020 2073 6d61  "....        sma
-000213d0: 4465 7620 3d20 6461 7461 5b22 534d 4122  Dev = data["SMA"
-000213e0: 5d2e 696c 6f63 5b30 5d20 2a20 6d61 5261  ].iloc[0] * maRa
-000213f0: 6e67 6520 2f20 3130 300d 0a20 2020 2020  nge / 100..     
-00021400: 2020 206c 6d61 4465 7620 3d20 6461 7461     lmaDev = data
-00021410: 5b22 4c4d 4122 5d2e 696c 6f63 5b30 5d20  ["LMA"].iloc[0] 
-00021420: 2a20 6d61 5261 6e67 6520 2f20 3130 300d  * maRange / 100.
-00021430: 0a20 2020 2020 2020 206f 7065 6e2c 2068  .        open, h
-00021440: 6967 682c 206c 6f77 2c20 636c 6f73 652c  igh, low, close,
-00021450: 2073 6d61 2c20 6c6d 6120 3d20 280d 0a20   sma, lma = (.. 
-00021460: 2020 2020 2020 2020 2020 2064 6174 615b             data[
-00021470: 224f 7065 6e22 5d2e 696c 6f63 5b30 5d2c  "Open"].iloc[0],
-00021480: 0d0a 2020 2020 2020 2020 2020 2020 6461  ..            da
-00021490: 7461 5b22 4869 6768 225d 2e69 6c6f 635b  ta["High"].iloc[
-000214a0: 305d 2c0d 0a20 2020 2020 2020 2020 2020  0],..           
-000214b0: 2064 6174 615b 224c 6f77 225d 2e69 6c6f   data["Low"].ilo
-000214c0: 635b 305d 2c0d 0a20 2020 2020 2020 2020  c[0],..         
-000214d0: 2020 2064 6174 615b 2243 6c6f 7365 225d     data["Close"]
-000214e0: 2e69 6c6f 635b 305d 2c0d 0a20 2020 2020  .iloc[0],..     
-000214f0: 2020 2020 2020 2064 6174 615b 2253 4d41         data["SMA
-00021500: 225d 2e69 6c6f 635b 305d 2c0d 0a20 2020  "].iloc[0],..   
-00021510: 2020 2020 2020 2020 2064 6174 615b 224c           data["L
-00021520: 4d41 225d 2e69 6c6f 635b 305d 2c0d 0a20  MA"].iloc[0],.. 
-00021530: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-00021540: 2020 6d61 5265 7665 7273 616c 203d 2030    maReversal = 0
-00021550: 0d0a 2020 2020 2020 2020 2320 5461 6b69  ..        # Taki
-00021560: 6e67 2053 7570 706f 7274 2035 300d 0a20  ng Support 50.. 
-00021570: 2020 2020 2020 2069 6620 636c 6f73 6520         if close 
-00021580: 3e20 736d 6120 616e 6420 6c6f 7720 3c3d  > sma and low <=
-00021590: 2028 736d 6120 2b20 736d 6144 6576 293a   (sma + smaDev):
-000215a0: 0d0a 2020 2020 2020 2020 2020 2020 7363  ..            sc
-000215b0: 7265 656e 4469 6374 5b22 4d41 2d53 6967  reenDict["MA-Sig
-000215c0: 6e61 6c22 5d20 3d20 280d 0a20 2020 2020  nal"] = (..     
-000215d0: 2020 2020 2020 2020 2020 2073 6176 6564             saved
-000215e0: 5b30 5d20 2b20 636f 6c6f 7254 6578 742e  [0] + colorText.
-000215f0: 424f 4c44 202b 2063 6f6c 6f72 5465 7874  BOLD + colorText
-00021600: 2e47 5245 454e 202b 2022 3530 4d41 2d53  .GREEN + "50MA-S
-00021610: 7570 706f 7274 2220 2b20 636f 6c6f 7254  upport" + colorT
-00021620: 6578 742e 454e 440d 0a20 2020 2020 2020  ext.END..       
-00021630: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
-00021640: 2020 2020 7361 7665 4469 6374 5b22 4d41      saveDict["MA
-00021650: 2d53 6967 6e61 6c22 5d20 3d20 7361 7665  -Signal"] = save
-00021660: 645b 315d 202b 2022 3530 4d41 2d53 7570  d[1] + "50MA-Sup
-00021670: 706f 7274 220d 0a20 2020 2020 2020 2020  port"..         
-00021680: 2020 206d 6152 6576 6572 7361 6c20 3d20     maReversal = 
-00021690: 310d 0a20 2020 2020 2020 2023 2056 616c  1..        # Val
-000216a0: 6964 6174 696e 6720 5265 7369 7374 616e  idating Resistan
-000216b0: 6365 2035 300d 0a20 2020 2020 2020 2065  ce 50..        e
-000216c0: 6c69 6620 636c 6f73 6520 3c20 736d 6120  lif close < sma 
-000216d0: 616e 6420 6869 6768 203e 3d20 2873 6d61  and high >= (sma
-000216e0: 202d 2073 6d61 4465 7629 3a0d 0a20 2020   - smaDev):..   
-000216f0: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
-00021700: 6963 745b 224d 412d 5369 676e 616c 225d  ict["MA-Signal"]
-00021710: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
-00021720: 2020 2020 2020 7361 7665 645b 305d 202b        saved[0] +
-00021730: 2063 6f6c 6f72 5465 7874 2e42 4f4c 4420   colorText.BOLD 
-00021740: 2b20 636f 6c6f 7254 6578 742e 4641 494c  + colorText.FAIL
-00021750: 202b 2022 3530 4d41 2d52 6573 6973 7422   + "50MA-Resist"
-00021760: 202b 2063 6f6c 6f72 5465 7874 2e45 4e44   + colorText.END
-00021770: 0d0a 2020 2020 2020 2020 2020 2020 290d  ..            ).
-00021780: 0a20 2020 2020 2020 2020 2020 2073 6176  .            sav
-00021790: 6544 6963 745b 224d 412d 5369 676e 616c  eDict["MA-Signal
-000217a0: 225d 203d 2073 6176 6564 5b31 5d20 2b20  "] = saved[1] + 
-000217b0: 2235 304d 412d 5265 7369 7374 220d 0a20  "50MA-Resist".. 
-000217c0: 2020 2020 2020 2020 2020 206d 6152 6576             maRev
-000217d0: 6572 7361 6c20 3d20 2d31 0d0a 2020 2020  ersal = -1..    
-000217e0: 2020 2020 2320 5461 6b69 6e67 2053 7570      # Taking Sup
-000217f0: 706f 7274 2032 3030 0d0a 2020 2020 2020  port 200..      
-00021800: 2020 656c 6966 2063 6c6f 7365 203e 206c    elif close > l
-00021810: 6d61 2061 6e64 206c 6f77 203c 3d20 286c  ma and low <= (l
-00021820: 6d61 202b 206c 6d61 4465 7629 3a0d 0a20  ma + lmaDev):.. 
-00021830: 2020 2020 2020 2020 2020 2073 6372 6565             scree
-00021840: 6e44 6963 745b 224d 412d 5369 676e 616c  nDict["MA-Signal
-00021850: 225d 203d 2028 0d0a 2020 2020 2020 2020  "] = (..        
-00021860: 2020 2020 2020 2020 7361 7665 645b 305d          saved[0]
-00021870: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
-00021880: 4420 2b20 636f 6c6f 7254 6578 742e 4752  D + colorText.GR
-00021890: 4545 4e20 2b20 2232 3030 4d41 2d53 7570  EEN + "200MA-Sup
+00020cb0: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
+00020cc0: 2250 6174 7465 726e 225d 203d 2028 0d0a  "Pattern"] = (..
+00020cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020ce0: 2020 2020 2020 2020 2020 2020 7361 7665              save
+00020cf0: 645b 305d 0d0a 2020 2020 2020 2020 2020  d[0]..          
+00020d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020d10: 2020 2b20 636f 6c6f 7254 6578 742e 424f    + colorText.BO
+00020d20: 4c44 0d0a 2020 2020 2020 2020 2020 2020  LD..            
+00020d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020d40: 2b20 636f 6c6f 7254 6578 742e 4752 4545  + colorText.GREE
+00020d50: 4e0d 0a20 2020 2020 2020 2020 2020 2020  N..             
+00020d60: 2020 2020 2020 2020 2020 2020 2020 202b                 +
+00020d70: 2022 4d6f 6d65 6e74 756d 2047 6169 6e65   "Momentum Gaine
+00020d80: 7222 0d0a 2020 2020 2020 2020 2020 2020  r"..            
+00020d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020da0: 2b20 636f 6c6f 7254 6578 742e 454e 440d  + colorText.END.
+00020db0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00020dc0: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
+00020dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020de0: 2020 2020 7361 7665 4469 6374 5b22 5061      saveDict["Pa
+00020df0: 7474 6572 6e22 5d20 3d20 7361 7665 645b  ttern"] = saved[
+00020e00: 315d 202b 2022 4d6f 6d65 6e74 756d 2047  1] + "Momentum G
+00020e10: 6169 6e65 7222 0d0a 2020 2020 2020 2020  ainer"..        
+00020e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020e30: 7265 7475 726e 2054 7275 650d 0a20 2020  return True..   
+00020e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020e50: 2023 2073 656c 662e 6465 6661 756c 745f   # self.default_
+00020e60: 6c6f 6767 6572 2e69 6e66 6f28 0d0a 2020  logger.info(..  
+00020e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020e80: 2020 2320 2020 2020 6627 5374 6f63 6b3a    #     f'Stock:
+00020e90: 7b73 6176 6544 6963 745b 2253 746f 636b  {saveDict["Stock
+00020ea0: 225d 7d2c 2069 7320 6e6f 7420 6120 6d6f  "]}, is not a mo
+00020eb0: 6d65 6e74 756d 2d67 6169 6e65 7220 6265  mentum-gainer be
+00020ec0: 6361 7573 6520 6569 7468 6572 2074 6f64  cause either tod
+00020ed0: 6179 2d6f 7065 6e20 287b 746f 7d29 203c  ay-open ({to}) <
+00020ee0: 2079 6573 7465 7264 6179 2d63 6c6f 7365   yesterday-close
+00020ef0: 2028 7b79 637d 2920 6f72 2079 6573 7465   ({yc}) or yeste
+00020f00: 7264 6179 2d6f 7065 6e28 7b79 6f7d 2920  rday-open({yo}) 
+00020f10: 3c20 6461 792d 6265 666f 7265 2d63 6c6f  < day-before-clo
+00020f20: 7365 287b 6479 637d 2927 0d0a 2020 2020  se({dyc})'..    
+00020f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020f40: 2320 290d 0a20 2020 2020 2020 2020 2020  # )..           
+00020f50: 2065 7863 6570 7420 496e 6465 7845 7272   except IndexErr
+00020f60: 6f72 2061 7320 653a 2023 2070 7261 676d  or as e: # pragm
+00020f70: 613a 206e 6f20 636f 7665 720d 0a20 2020  a: no cover..   
+00020f80: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00020f90: 662e 6465 6661 756c 745f 6c6f 6767 6572  f.default_logger
+00020fa0: 2e64 6562 7567 2865 2c20 6578 635f 696e  .debug(e, exc_in
+00020fb0: 666f 3d54 7275 6529 0d0a 2020 2020 2020  fo=True)..      
+00020fc0: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+00020fd0: 6566 6175 6c74 5f6c 6f67 6765 722e 6465  efault_logger.de
+00020fe0: 6275 6728 6461 7461 290d 0a20 2020 2020  bug(data)..     
+00020ff0: 2020 2020 2020 2020 2020 2070 6173 730d             pass.
+00021000: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00021010: 7572 6e20 4661 6c73 650d 0a20 2020 2020  urn False..     
+00021020: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
+00021030: 696f 6e20 6173 2065 3a20 2023 2070 7261  ion as e:  # pra
+00021040: 676d 613a 206e 6f20 636f 7665 720d 0a20  gma: no cover.. 
+00021050: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00021060: 6465 6661 756c 745f 6c6f 6767 6572 2e64  default_logger.d
+00021070: 6562 7567 2865 2c20 6578 635f 696e 666f  ebug(e, exc_info
+00021080: 3d54 7275 6529 0d0a 2020 2020 2020 2020  =True)..        
+00021090: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+000210a0: 0d0a 0d0a 2020 2020 2340 6d65 6173 7572  ....    #@measur
+000210b0: 655f 7469 6d65 0d0a 2020 2020 2320 5661  e_time..    # Va
+000210c0: 6c69 6461 7465 204d 6f76 696e 6720 6176  lidate Moving av
+000210d0: 6572 6167 6573 2061 6e64 206c 6f6f 6b20  erages and look 
+000210e0: 666f 7220 6275 792f 7365 6c6c 2073 6967  for buy/sell sig
+000210f0: 6e61 6c73 0d0a 2020 2020 6465 6620 7661  nals..    def va
+00021100: 6c69 6461 7465 4d6f 7669 6e67 4176 6572  lidateMovingAver
+00021110: 6167 6573 2873 656c 662c 2064 662c 2073  ages(self, df, s
+00021120: 6372 6565 6e44 6963 742c 2073 6176 6544  creenDict, saveD
+00021130: 6963 742c 206d 6152 616e 6765 3d32 2e35  ict, maRange=2.5
+00021140: 293a 0d0a 2020 2020 2020 2020 6461 7461  ):..        data
+00021150: 203d 2064 662e 636f 7079 2829 0d0a 2020   = df.copy()..  
+00021160: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
+00021170: 612e 6669 6c6c 6e61 2830 290d 0a20 2020  a.fillna(0)..   
+00021180: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
+00021190: 2e72 6570 6c61 6365 285b 6e70 2e69 6e66  .replace([np.inf
+000211a0: 2c20 2d6e 702e 696e 665d 2c20 3029 0d0a  , -np.inf], 0)..
+000211b0: 2020 2020 2020 2020 7265 6365 6e74 203d          recent =
+000211c0: 2064 6174 612e 6865 6164 2831 290d 0a20   data.head(1).. 
+000211d0: 2020 2020 2020 2073 6176 6564 203d 2073         saved = s
+000211e0: 656c 662e 6669 6e64 4375 7272 656e 7453  elf.findCurrentS
+000211f0: 6176 6564 5661 6c75 6528 7363 7265 656e  avedValue(screen
+00021200: 4469 6374 2c73 6176 6544 6963 742c 224d  Dict,saveDict,"M
+00021210: 412d 5369 676e 616c 2229 0d0a 2020 2020  A-Signal")..    
+00021220: 2020 2020 6966 2028 0d0a 2020 2020 2020      if (..      
+00021230: 2020 2020 2020 7265 6365 6e74 5b22 534d        recent["SM
+00021240: 4122 5d2e 696c 6f63 5b30 5d20 3e20 7265  A"].iloc[0] > re
+00021250: 6365 6e74 5b22 4c4d 4122 5d2e 696c 6f63  cent["LMA"].iloc
+00021260: 5b30 5d0d 0a20 2020 2020 2020 2020 2020  [0]..           
+00021270: 2061 6e64 2072 6563 656e 745b 2243 6c6f   and recent["Clo
+00021280: 7365 225d 2e69 6c6f 635b 305d 203e 2072  se"].iloc[0] > r
+00021290: 6563 656e 745b 2253 4d41 225d 2e69 6c6f  ecent["SMA"].ilo
+000212a0: 635b 305d 0d0a 2020 2020 2020 2020 293a  c[0]..        ):
+000212b0: 0d0a 2020 2020 2020 2020 2020 2020 7363  ..            sc
+000212c0: 7265 656e 4469 6374 5b22 4d41 2d53 6967  reenDict["MA-Sig
+000212d0: 6e61 6c22 5d20 3d20 280d 0a20 2020 2020  nal"] = (..     
+000212e0: 2020 2020 2020 2020 2020 2073 6176 6564             saved
+000212f0: 5b30 5d20 2b20 636f 6c6f 7254 6578 742e  [0] + colorText.
+00021300: 424f 4c44 202b 2063 6f6c 6f72 5465 7874  BOLD + colorText
+00021310: 2e47 5245 454e 202b 2022 4275 6c6c 6973  .GREEN + "Bullis
+00021320: 6822 202b 2063 6f6c 6f72 5465 7874 2e45  h" + colorText.E
+00021330: 4e44 0d0a 2020 2020 2020 2020 2020 2020  ND..            
+00021340: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
+00021350: 6176 6544 6963 745b 224d 412d 5369 676e  aveDict["MA-Sign
+00021360: 616c 225d 203d 2073 6176 6564 5b31 5d20  al"] = saved[1] 
+00021370: 2b20 2242 756c 6c69 7368 220d 0a20 2020  + "Bullish"..   
+00021380: 2020 2020 2065 6c69 6620 7265 6365 6e74       elif recent
+00021390: 5b22 534d 4122 5d2e 696c 6f63 5b30 5d20  ["SMA"].iloc[0] 
+000213a0: 3c20 7265 6365 6e74 5b22 4c4d 4122 5d2e  < recent["LMA"].
+000213b0: 696c 6f63 5b30 5d3a 0d0a 2020 2020 2020  iloc[0]:..      
+000213c0: 2020 2020 2020 7363 7265 656e 4469 6374        screenDict
+000213d0: 5b22 4d41 2d53 6967 6e61 6c22 5d20 3d20  ["MA-Signal"] = 
+000213e0: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+000213f0: 2020 2073 6176 6564 5b30 5d20 2b20 636f     saved[0] + co
+00021400: 6c6f 7254 6578 742e 424f 4c44 202b 2063  lorText.BOLD + c
+00021410: 6f6c 6f72 5465 7874 2e46 4149 4c20 2b20  olorText.FAIL + 
+00021420: 2242 6561 7269 7368 2220 2b20 636f 6c6f  "Bearish" + colo
+00021430: 7254 6578 742e 454e 440d 0a20 2020 2020  rText.END..     
+00021440: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+00021450: 2020 2020 2020 7361 7665 4469 6374 5b22        saveDict["
+00021460: 4d41 2d53 6967 6e61 6c22 5d20 3d20 7361  MA-Signal"] = sa
+00021470: 7665 645b 315d 202b 2022 4265 6172 6973  ved[1] + "Bearis
+00021480: 6822 0d0a 2020 2020 2020 2020 656c 6966  h"..        elif
+00021490: 2072 6563 656e 745b 2253 4d41 225d 2e69   recent["SMA"].i
+000214a0: 6c6f 635b 305d 203d 3d20 303a 0d0a 2020  loc[0] == 0:..  
+000214b0: 2020 2020 2020 2020 2020 7363 7265 656e            screen
+000214c0: 4469 6374 5b22 4d41 2d53 6967 6e61 6c22  Dict["MA-Signal"
+000214d0: 5d20 3d20 280d 0a20 2020 2020 2020 2020  ] = (..         
+000214e0: 2020 2020 2020 2073 6176 6564 5b30 5d20         saved[0] 
+000214f0: 2b20 636f 6c6f 7254 6578 742e 424f 4c44  + colorText.BOLD
+00021500: 202b 2063 6f6c 6f72 5465 7874 2e57 4152   + colorText.WAR
+00021510: 4e20 2b20 2255 6e6b 6e6f 776e 2220 2b20  N + "Unknown" + 
+00021520: 636f 6c6f 7254 6578 742e 454e 440d 0a20  colorText.END.. 
+00021530: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
+00021540: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
+00021550: 6374 5b22 4d41 2d53 6967 6e61 6c22 5d20  ct["MA-Signal"] 
+00021560: 3d20 7361 7665 645b 315d 202b 2022 556e  = saved[1] + "Un
+00021570: 6b6e 6f77 6e22 0d0a 2020 2020 2020 2020  known"..        
+00021580: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00021590: 2020 2073 6372 6565 6e44 6963 745b 224d     screenDict["M
+000215a0: 412d 5369 676e 616c 225d 203d 2028 0d0a  A-Signal"] = (..
+000215b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000215c0: 7361 7665 645b 305d 202b 2063 6f6c 6f72  saved[0] + color
+000215d0: 5465 7874 2e42 4f4c 4420 2b20 636f 6c6f  Text.BOLD + colo
+000215e0: 7254 6578 742e 5741 524e 202b 2022 4e65  rText.WARN + "Ne
+000215f0: 7574 7261 6c22 202b 2063 6f6c 6f72 5465  utral" + colorTe
+00021600: 7874 2e45 4e44 0d0a 2020 2020 2020 2020  xt.END..        
+00021610: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
+00021620: 2020 2073 6176 6544 6963 745b 224d 412d     saveDict["MA-
+00021630: 5369 676e 616c 225d 203d 2073 6176 6564  Signal"] = saved
+00021640: 5b31 5d20 2b20 224e 6575 7472 616c 220d  [1] + "Neutral".
+00021650: 0a0d 0a20 2020 2020 2020 2073 6d61 4465  ...        smaDe
+00021660: 7620 3d20 6461 7461 5b22 534d 4122 5d2e  v = data["SMA"].
+00021670: 696c 6f63 5b30 5d20 2a20 6d61 5261 6e67  iloc[0] * maRang
+00021680: 6520 2f20 3130 300d 0a20 2020 2020 2020  e / 100..       
+00021690: 206c 6d61 4465 7620 3d20 6461 7461 5b22   lmaDev = data["
+000216a0: 4c4d 4122 5d2e 696c 6f63 5b30 5d20 2a20  LMA"].iloc[0] * 
+000216b0: 6d61 5261 6e67 6520 2f20 3130 300d 0a20  maRange / 100.. 
+000216c0: 2020 2020 2020 206f 7065 6e2c 2068 6967         open, hig
+000216d0: 682c 206c 6f77 2c20 636c 6f73 652c 2073  h, low, close, s
+000216e0: 6d61 2c20 6c6d 6120 3d20 280d 0a20 2020  ma, lma = (..   
+000216f0: 2020 2020 2020 2020 2064 6174 615b 224f           data["O
+00021700: 7065 6e22 5d2e 696c 6f63 5b30 5d2c 0d0a  pen"].iloc[0],..
+00021710: 2020 2020 2020 2020 2020 2020 6461 7461              data
+00021720: 5b22 4869 6768 225d 2e69 6c6f 635b 305d  ["High"].iloc[0]
+00021730: 2c0d 0a20 2020 2020 2020 2020 2020 2064  ,..            d
+00021740: 6174 615b 224c 6f77 225d 2e69 6c6f 635b  ata["Low"].iloc[
+00021750: 305d 2c0d 0a20 2020 2020 2020 2020 2020  0],..           
+00021760: 2064 6174 615b 2243 6c6f 7365 225d 2e69   data["Close"].i
+00021770: 6c6f 635b 305d 2c0d 0a20 2020 2020 2020  loc[0],..       
+00021780: 2020 2020 2064 6174 615b 2253 4d41 225d       data["SMA"]
+00021790: 2e69 6c6f 635b 305d 2c0d 0a20 2020 2020  .iloc[0],..     
+000217a0: 2020 2020 2020 2064 6174 615b 224c 4d41         data["LMA
+000217b0: 225d 2e69 6c6f 635b 305d 2c0d 0a20 2020  "].iloc[0],..   
+000217c0: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+000217d0: 6d61 5265 7665 7273 616c 203d 2030 0d0a  maReversal = 0..
+000217e0: 2020 2020 2020 2020 2320 5461 6b69 6e67          # Taking
+000217f0: 2053 7570 706f 7274 2035 300d 0a20 2020   Support 50..   
+00021800: 2020 2020 2069 6620 636c 6f73 6520 3e20       if close > 
+00021810: 736d 6120 616e 6420 6c6f 7720 3c3d 2028  sma and low <= (
+00021820: 736d 6120 2b20 736d 6144 6576 293a 0d0a  sma + smaDev):..
+00021830: 2020 2020 2020 2020 2020 2020 7363 7265              scre
+00021840: 656e 4469 6374 5b22 4d41 2d53 6967 6e61  enDict["MA-Signa
+00021850: 6c22 5d20 3d20 280d 0a20 2020 2020 2020  l"] = (..       
+00021860: 2020 2020 2020 2020 2073 6176 6564 5b30           saved[0
+00021870: 5d20 2b20 636f 6c6f 7254 6578 742e 424f  ] + colorText.BO
+00021880: 4c44 202b 2063 6f6c 6f72 5465 7874 2e47  LD + colorText.G
+00021890: 5245 454e 202b 2022 3530 4d41 2d53 7570  REEN + "50MA-Sup
 000218a0: 706f 7274 2220 2b20 636f 6c6f 7254 6578  port" + colorTex
 000218b0: 742e 454e 440d 0a20 2020 2020 2020 2020  t.END..         
 000218c0: 2020 2029 0d0a 2020 2020 2020 2020 2020     )..          
 000218d0: 2020 7361 7665 4469 6374 5b22 4d41 2d53    saveDict["MA-S
 000218e0: 6967 6e61 6c22 5d20 3d20 7361 7665 645b  ignal"] = saved[
-000218f0: 315d 202b 2022 3230 304d 412d 5375 7070  1] + "200MA-Supp
-00021900: 6f72 7422 0d0a 2020 2020 2020 2020 2020  ort"..          
-00021910: 2020 6d61 5265 7665 7273 616c 203d 2031    maReversal = 1
-00021920: 0d0a 2020 2020 2020 2020 2320 5661 6c69  ..        # Vali
-00021930: 6461 7469 6e67 2052 6573 6973 7461 6e63  dating Resistanc
-00021940: 6520 3230 300d 0a20 2020 2020 2020 2065  e 200..        e
-00021950: 6c69 6620 636c 6f73 6520 3c20 6c6d 6120  lif close < lma 
-00021960: 616e 6420 6869 6768 203e 3d20 286c 6d61  and high >= (lma
-00021970: 202d 206c 6d61 4465 7629 3a0d 0a20 2020   - lmaDev):..   
-00021980: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
-00021990: 6963 745b 224d 412d 5369 676e 616c 225d  ict["MA-Signal"]
-000219a0: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
-000219b0: 2020 2020 2020 7361 7665 645b 305d 202b        saved[0] +
-000219c0: 2063 6f6c 6f72 5465 7874 2e42 4f4c 4420   colorText.BOLD 
-000219d0: 2b20 636f 6c6f 7254 6578 742e 4641 494c  + colorText.FAIL
-000219e0: 202b 2022 3230 304d 412d 5265 7369 7374   + "200MA-Resist
-000219f0: 2220 2b20 636f 6c6f 7254 6578 742e 454e  " + colorText.EN
-00021a00: 440d 0a20 2020 2020 2020 2020 2020 2029  D..            )
-00021a10: 0d0a 2020 2020 2020 2020 2020 2020 7361  ..            sa
-00021a20: 7665 4469 6374 5b22 4d41 2d53 6967 6e61  veDict["MA-Signa
-00021a30: 6c22 5d20 3d20 7361 7665 645b 315d 202b  l"] = saved[1] +
-00021a40: 2022 3230 304d 412d 5265 7369 7374 220d   "200MA-Resist".
-00021a50: 0a20 2020 2020 2020 2020 2020 206d 6152  .            maR
-00021a60: 6576 6572 7361 6c20 3d20 2d31 0d0a 2020  eversal = -1..  
-00021a70: 2020 2020 2020 2320 466f 7220 6120 4275        # For a Bu
-00021a80: 6c6c 6973 6820 4361 6e64 6c65 0d0a 2020  llish Candle..  
-00021a90: 2020 2020 2020 6966 2073 656c 662e 6765        if self.ge
-00021aa0: 7443 616e 646c 6554 7970 6528 6461 7461  tCandleType(data
-00021ab0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00021ac0: 2320 4372 6f73 7369 6e67 2075 7020 3530  # Crossing up 50
-00021ad0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00021ae0: 206f 7065 6e20 3c20 736d 6120 616e 6420   open < sma and 
-00021af0: 636c 6f73 6520 3e20 736d 613a 0d0a 2020  close > sma:..  
-00021b00: 2020 2020 2020 2020 2020 2020 2020 7363                sc
-00021b10: 7265 656e 4469 6374 5b22 4d41 2d53 6967  reenDict["MA-Sig
-00021b20: 6e61 6c22 5d20 3d20 280d 0a20 2020 2020  nal"] = (..     
-00021b30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00021b40: 6176 6564 5b30 5d20 2b20 636f 6c6f 7254  aved[0] + colorT
-00021b50: 6578 742e 424f 4c44 202b 2063 6f6c 6f72  ext.BOLD + color
-00021b60: 5465 7874 2e47 5245 454e 202b 2022 4275  Text.GREEN + "Bu
-00021b70: 6c6c 4372 6f73 732d 3530 4d41 2220 2b20  llCross-50MA" + 
-00021b80: 636f 6c6f 7254 6578 742e 454e 440d 0a20  colorText.END.. 
-00021b90: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00021ba0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00021bb0: 2020 7361 7665 4469 6374 5b22 4d41 2d53    saveDict["MA-S
-00021bc0: 6967 6e61 6c22 5d20 3d20 7361 7665 645b  ignal"] = saved[
-00021bd0: 315d 202b 2022 4275 6c6c 4372 6f73 732d  1] + "BullCross-
-00021be0: 3530 4d41 220d 0a20 2020 2020 2020 2020  50MA"..         
-00021bf0: 2020 2020 2020 206d 6152 6576 6572 7361         maReversa
-00021c00: 6c20 3d20 310d 0a20 2020 2020 2020 2020  l = 1..         
-00021c10: 2020 2023 2043 726f 7373 696e 6720 7570     # Crossing up
-00021c20: 2032 3030 0d0a 2020 2020 2020 2020 2020   200..          
-00021c30: 2020 656c 6966 206f 7065 6e20 3c20 6c6d    elif open < lm
-00021c40: 6120 616e 6420 636c 6f73 6520 3e20 6c6d  a and close > lm
-00021c50: 613a 0d0a 2020 2020 2020 2020 2020 2020  a:..            
-00021c60: 2020 2020 7363 7265 656e 4469 6374 5b22      screenDict["
-00021c70: 4d41 2d53 6967 6e61 6c22 5d20 3d20 280d  MA-Signal"] = (.
-00021c80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00021c90: 2020 2020 2073 6176 6564 5b30 5d20 2b20       saved[0] + 
-00021ca0: 636f 6c6f 7254 6578 742e 424f 4c44 202b  colorText.BOLD +
-00021cb0: 2063 6f6c 6f72 5465 7874 2e47 5245 454e   colorText.GREEN
-00021cc0: 202b 2022 4275 6c6c 4372 6f73 732d 3230   + "BullCross-20
-00021cd0: 304d 4122 202b 2063 6f6c 6f72 5465 7874  0MA" + colorText
-00021ce0: 2e45 4e44 0d0a 2020 2020 2020 2020 2020  .END..          
-00021cf0: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-00021d00: 2020 2020 2020 2020 2073 6176 6544 6963           saveDic
-00021d10: 745b 224d 412d 5369 676e 616c 225d 203d  t["MA-Signal"] =
-00021d20: 2073 6176 6564 5b31 5d20 2b20 2242 756c   saved[1] + "Bul
-00021d30: 6c43 726f 7373 2d32 3030 4d41 220d 0a20  lCross-200MA".. 
-00021d40: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00021d50: 6152 6576 6572 7361 6c20 3d20 310d 0a20  aReversal = 1.. 
-00021d60: 2020 2020 2020 2023 2046 6f72 2061 2042         # For a B
-00021d70: 6561 7269 7368 2043 616e 646c 650d 0a20  earish Candle.. 
-00021d80: 2020 2020 2020 2065 6c69 6620 6e6f 7420         elif not 
-00021d90: 7365 6c66 2e67 6574 4361 6e64 6c65 5479  self.getCandleTy
-00021da0: 7065 2864 6174 6129 3a0d 0a20 2020 2020  pe(data):..     
-00021db0: 2020 2020 2020 2023 2043 726f 7373 696e         # Crossin
-00021dc0: 6720 646f 776e 2035 300d 0a20 2020 2020  g down 50..     
-00021dd0: 2020 2020 2020 2069 6620 6f70 656e 203e         if open >
-00021de0: 2073 6d61 2061 6e64 2063 6c6f 7365 203c   sma and close <
-00021df0: 2073 6d61 3a0d 0a20 2020 2020 2020 2020   sma:..         
-00021e00: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
-00021e10: 745b 224d 412d 5369 676e 616c 225d 203d  t["MA-Signal"] =
-00021e20: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
-00021e30: 2020 2020 2020 2020 7361 7665 645b 305d          saved[0]
-00021e40: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
-00021e50: 4420 2b20 636f 6c6f 7254 6578 742e 4641  D + colorText.FA
-00021e60: 494c 202b 2022 4265 6172 4372 6f73 732d  IL + "BearCross-
-00021e70: 3530 4d41 2220 2b20 636f 6c6f 7254 6578  50MA" + colorTex
-00021e80: 742e 454e 440d 0a20 2020 2020 2020 2020  t.END..         
-00021e90: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-00021ea0: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
-00021eb0: 6374 5b22 4d41 2d53 6967 6e61 6c22 5d20  ct["MA-Signal"] 
-00021ec0: 3d20 7361 7665 645b 315d 202b 2022 4265  = saved[1] + "Be
-00021ed0: 6172 4372 6f73 732d 3530 4d41 220d 0a20  arCross-50MA".. 
-00021ee0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00021ef0: 6152 6576 6572 7361 6c20 3d20 2d31 0d0a  aReversal = -1..
-00021f00: 2020 2020 2020 2020 2020 2020 2320 4372              # Cr
-00021f10: 6f73 7369 6e67 2075 7020 3230 300d 0a20  ossing up 200.. 
-00021f20: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-00021f30: 6f70 656e 203e 206c 6d61 2061 6e64 2063  open > lma and c
-00021f40: 6c6f 7365 203c 206c 6d61 3a0d 0a20 2020  lose < lma:..   
-00021f50: 2020 2020 2020 2020 2020 2020 2073 6372               scr
-00021f60: 6565 6e44 6963 745b 224d 412d 5369 676e  eenDict["MA-Sign
-00021f70: 616c 225d 203d 2028 0d0a 2020 2020 2020  al"] = (..      
-00021f80: 2020 2020 2020 2020 2020 2020 2020 7361                sa
-00021f90: 7665 645b 305d 202b 2063 6f6c 6f72 5465  ved[0] + colorTe
-00021fa0: 7874 2e42 4f4c 4420 2b20 636f 6c6f 7254  xt.BOLD + colorT
-00021fb0: 6578 742e 4641 494c 202b 2022 4265 6172  ext.FAIL + "Bear
-00021fc0: 4372 6f73 732d 3230 304d 4122 202b 2063  Cross-200MA" + c
-00021fd0: 6f6c 6f72 5465 7874 2e45 4e44 0d0a 2020  olorText.END..  
-00021fe0: 2020 2020 2020 2020 2020 2020 2020 290d                ).
-00021ff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00022000: 2073 6176 6544 6963 745b 224d 412d 5369   saveDict["MA-Si
-00022010: 676e 616c 225d 203d 2073 6176 6564 5b31  gnal"] = saved[1
-00022020: 5d20 2b20 2242 6561 7243 726f 7373 2d32  ] + "BearCross-2
-00022030: 3030 4d41 220d 0a20 2020 2020 2020 2020  00MA"..         
-00022040: 2020 2020 2020 206d 6152 6576 6572 7361         maReversa
-00022050: 6c20 3d20 2d31 0d0a 2020 2020 2020 2020  l = -1..        
-00022060: 7265 7475 726e 206d 6152 6576 6572 7361  return maReversa
-00022070: 6c0d 0a0d 0a20 2020 2023 2046 696e 6420  l....    # Find 
-00022080: 4e52 7820 7261 6e67 6520 666f 7220 5265  NRx range for Re
-00022090: 7665 7273 616c 0d0a 2020 2020 6465 6620  versal..    def 
-000220a0: 7661 6c69 6461 7465 4e61 7272 6f77 5261  validateNarrowRa
-000220b0: 6e67 6528 7365 6c66 2c20 6466 2c20 7363  nge(self, df, sc
-000220c0: 7265 656e 4469 6374 2c20 7361 7665 4469  reenDict, saveDi
-000220d0: 6374 2c20 6e72 3d34 293a 0d0a 2020 2020  ct, nr=4):..    
-000220e0: 2020 2020 6966 2064 6620 6973 204e 6f6e      if df is Non
-000220f0: 6520 6f72 206c 656e 2864 6629 203d 3d20  e or len(df) == 
-00022100: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
-00022110: 7265 7475 726e 2046 616c 7365 0d0a 2020  return False..  
-00022120: 2020 2020 2020 6461 7461 203d 2064 662e        data = df.
-00022130: 636f 7079 2829 0d0a 2020 2020 2020 2020  copy()..        
-00022140: 7361 7665 6420 3d20 7365 6c66 2e66 696e  saved = self.fin
-00022150: 6443 7572 7265 6e74 5361 7665 6456 616c  dCurrentSavedVal
-00022160: 7565 2873 6372 6565 6e44 6963 742c 2073  ue(screenDict, s
-00022170: 6176 6544 6963 742c 2022 5061 7474 6572  aveDict, "Patter
-00022180: 6e22 290d 0a20 2020 2020 2020 2069 6620  n")..        if 
-00022190: 504b 4461 7465 5574 696c 6974 6965 732e  PKDateUtilities.
-000221a0: 6973 5472 6164 696e 6754 696d 6528 293a  isTradingTime():
-000221b0: 0d0a 2020 2020 2020 2020 2020 2020 7261  ..            ra
-000221c0: 6e67 6544 6174 6120 3d20 6461 7461 2e68  ngeData = data.h
-000221d0: 6561 6428 6e72 202b 2031 295b 313a 5d0d  ead(nr + 1)[1:].
-000221e0: 0a20 2020 2020 2020 2020 2020 206e 6f77  .            now
-000221f0: 5f63 616e 646c 6520 3d20 6461 7461 2e68  _candle = data.h
-00022200: 6561 6428 3129 0d0a 2020 2020 2020 2020  ead(1)..        
-00022210: 2020 2020 7261 6e67 6544 6174 615b 2252      rangeData["R
-00022220: 616e 6765 225d 203d 2061 6273 2872 616e  ange"] = abs(ran
-00022230: 6765 4461 7461 5b22 436c 6f73 6522 5d20  geData["Close"] 
-00022240: 2d20 7261 6e67 6544 6174 615b 224f 7065  - rangeData["Ope
-00022250: 6e22 5d29 0d0a 2020 2020 2020 2020 2020  n"])..          
-00022260: 2020 7265 6365 6e74 203d 2072 616e 6765    recent = range
-00022270: 4461 7461 2e68 6561 6428 3129 0d0a 2020  Data.head(1)..  
-00022280: 2020 2020 2020 2020 2020 6966 2028 0d0a            if (..
-00022290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000222a0: 6c65 6e28 7265 6365 6e74 2920 3d3d 2031  len(recent) == 1
-000222b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000222c0: 2020 616e 6420 7265 6365 6e74 5b22 5261    and recent["Ra
-000222d0: 6e67 6522 5d2e 696c 6f63 5b30 5d20 3d3d  nge"].iloc[0] ==
-000222e0: 2072 616e 6765 4461 7461 2e64 6573 6372   rangeData.descr
-000222f0: 6962 6528 295b 2252 616e 6765 225d 5b22  ibe()["Range"]["
-00022300: 6d69 6e22 5d0d 0a20 2020 2020 2020 2020  min"]..         
-00022310: 2020 2029 3a0d 0a20 2020 2020 2020 2020     ):..         
-00022320: 2020 2020 2020 2069 6620 280d 0a20 2020         if (..   
-00022330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022340: 2073 656c 662e 6765 7443 616e 646c 6554   self.getCandleT
-00022350: 7970 6528 7265 6365 6e74 290d 0a20 2020  ype(recent)..   
-00022360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022370: 2061 6e64 206e 6f77 5f63 616e 646c 655b   and now_candle[
-00022380: 2243 6c6f 7365 225d 2e69 6c6f 635b 305d  "Close"].iloc[0]
-00022390: 203e 3d20 7265 6365 6e74 5b22 436c 6f73   >= recent["Clos
-000223a0: 6522 5d2e 696c 6f63 5b30 5d0d 0a20 2020  e"].iloc[0]..   
-000223b0: 2020 2020 2020 2020 2020 2020 2029 3a0d               ):.
-000223c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000223d0: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
-000223e0: 2250 6174 7465 726e 225d 203d 2028 0d0a  "Pattern"] = (..
-000223f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022400: 2020 2020 2020 2020 7361 7665 645b 305d          saved[0]
-00022410: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
-00022420: 4420 2b20 636f 6c6f 7254 6578 742e 4752  D + colorText.GR
-00022430: 4545 4e20 2b20 6622 4275 792d 4e52 7b6e  EEN + f"Buy-NR{n
-00022440: 727d 2220 2b20 636f 6c6f 7254 6578 742e  r}" + colorText.
-00022450: 454e 440d 0a20 2020 2020 2020 2020 2020  END..           
-00022460: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
-00022470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022480: 7361 7665 4469 6374 5b22 5061 7474 6572  saveDict["Patter
-00022490: 6e22 5d20 3d20 7361 7665 645b 315d 202b  n"] = saved[1] +
-000224a0: 2066 2242 7579 2d4e 527b 6e72 7d22 0d0a   f"Buy-NR{nr}"..
-000224b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000224c0: 2020 2020 7265 7475 726e 2054 7275 650d      return True.
-000224d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000224e0: 2065 6c69 6620 280d 0a20 2020 2020 2020   elif (..       
-000224f0: 2020 2020 2020 2020 2020 2020 206e 6f74               not
-00022500: 2073 656c 662e 6765 7443 616e 646c 6554   self.getCandleT
-00022510: 7970 6528 7265 6365 6e74 290d 0a20 2020  ype(recent)..   
-00022520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022530: 2061 6e64 206e 6f77 5f63 616e 646c 655b   and now_candle[
-00022540: 2243 6c6f 7365 225d 2e69 6c6f 635b 305d  "Close"].iloc[0]
-00022550: 203c 3d20 7265 6365 6e74 5b22 436c 6f73   <= recent["Clos
-00022560: 6522 5d2e 696c 6f63 5b30 5d0d 0a20 2020  e"].iloc[0]..   
-00022570: 2020 2020 2020 2020 2020 2020 2029 3a0d               ):.
-00022580: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00022590: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
-000225a0: 2250 6174 7465 726e 225d 203d 2028 0d0a  "Pattern"] = (..
-000225b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000225c0: 2020 2020 2020 2020 7361 7665 645b 305d          saved[0]
-000225d0: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
-000225e0: 4420 2b20 636f 6c6f 7254 6578 742e 4641  D + colorText.FA
-000225f0: 494c 202b 2066 2253 656c 6c2d 4e52 7b6e  IL + f"Sell-NR{n
-00022600: 727d 2220 2b20 636f 6c6f 7254 6578 742e  r}" + colorText.
-00022610: 454e 440d 0a20 2020 2020 2020 2020 2020  END..           
-00022620: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
-00022630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022640: 7361 7665 4469 6374 5b22 5061 7474 6572  saveDict["Patter
-00022650: 6e22 5d20 3d20 7361 7665 645b 315d 202b  n"] = saved[1] +
-00022660: 2066 2253 656c 6c2d 4e52 7b6e 727d 220d   f"Sell-NR{nr}".
-00022670: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00022680: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
-00022690: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-000226a0: 7475 726e 2046 616c 7365 0d0a 2020 2020  turn False..    
-000226b0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-000226c0: 2020 2020 2020 2072 616e 6765 4461 7461         rangeData
-000226d0: 203d 2064 6174 612e 6865 6164 286e 7229   = data.head(nr)
-000226e0: 0d0a 2020 2020 2020 2020 2020 2020 7261  ..            ra
-000226f0: 6e67 6544 6174 612e 6c6f 635b 3a2c 2752  ngeData.loc[:,'R
-00022700: 616e 6765 275d 203d 2061 6273 2872 616e  ange'] = abs(ran
-00022710: 6765 4461 7461 5b22 436c 6f73 6522 5d20  geData["Close"] 
-00022720: 2d20 7261 6e67 6544 6174 615b 224f 7065  - rangeData["Ope
-00022730: 6e22 5d29 0d0a 2020 2020 2020 2020 2020  n"])..          
-00022740: 2020 7265 6365 6e74 203d 2072 616e 6765    recent = range
-00022750: 4461 7461 2e68 6561 6428 3129 0d0a 2020  Data.head(1)..  
-00022760: 2020 2020 2020 2020 2020 6966 2072 6563            if rec
-00022770: 656e 745b 2252 616e 6765 225d 2e69 6c6f  ent["Range"].ilo
-00022780: 635b 305d 203d 3d20 7261 6e67 6544 6174  c[0] == rangeDat
-00022790: 612e 6465 7363 7269 6265 2829 5b22 5261  a.describe()["Ra
-000227a0: 6e67 6522 5d5b 226d 696e 225d 3a0d 0a20  nge"]["min"]:.. 
-000227b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000227c0: 6372 6565 6e44 6963 745b 2250 6174 7465  creenDict["Patte
-000227d0: 726e 225d 203d 2028 0d0a 2020 2020 2020  rn"] = (..      
-000227e0: 2020 2020 2020 2020 2020 2020 2020 7361                sa
-000227f0: 7665 645b 305d 202b 2063 6f6c 6f72 5465  ved[0] + colorTe
-00022800: 7874 2e42 4f4c 4420 2b20 636f 6c6f 7254  xt.BOLD + colorT
-00022810: 6578 742e 4752 4545 4e20 2b20 6622 4e52  ext.GREEN + f"NR
-00022820: 7b6e 727d 2220 2b20 636f 6c6f 7254 6578  {nr}" + colorTex
-00022830: 742e 454e 440d 0a20 2020 2020 2020 2020  t.END..         
-00022840: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-00022850: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
-00022860: 6374 5b22 5061 7474 6572 6e22 5d20 3d20  ct["Pattern"] = 
-00022870: 7361 7665 645b 315d 202b 2066 224e 527b  saved[1] + f"NR{
-00022880: 6e72 7d22 0d0a 2020 2020 2020 2020 2020  nr}"..          
-00022890: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
-000228a0: 650d 0a20 2020 2020 2020 2020 2020 2072  e..            r
-000228b0: 6574 7572 6e20 4661 6c73 650d 0a0d 0a20  eturn False.... 
-000228c0: 2020 2023 2046 696e 6420 6966 2073 746f     # Find if sto
-000228d0: 636b 2069 7320 6e65 776c 7920 6c69 7374  ck is newly list
-000228e0: 6564 0d0a 2020 2020 6465 6620 7661 6c69  ed..    def vali
-000228f0: 6461 7465 4e65 776c 794c 6973 7465 6428  dateNewlyListed(
-00022900: 7365 6c66 2c20 6466 2c20 6461 7973 546f  self, df, daysTo
-00022910: 4c6f 6f6b 6261 636b 293a 0d0a 2020 2020  Lookback):..    
-00022920: 2020 2020 6966 2064 6620 6973 204e 6f6e      if df is Non
-00022930: 6520 6f72 206c 656e 2864 6629 203d 3d20  e or len(df) == 
-00022940: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
-00022950: 7265 7475 726e 2046 616c 7365 0d0a 2020  return False..  
-00022960: 2020 2020 2020 6461 7461 203d 2064 662e        data = df.
-00022970: 636f 7079 2829 0d0a 2020 2020 2020 2020  copy()..        
-00022980: 6461 7973 546f 4c6f 6f6b 6261 636b 203d  daysToLookback =
-00022990: 2069 6e74 2864 6179 7354 6f4c 6f6f 6b62   int(daysToLookb
-000229a0: 6163 6b5b 3a2d 315d 290d 0a20 2020 2020  ack[:-1])..     
-000229b0: 2020 2072 6563 656e 7420 3d20 6461 7461     recent = data
-000229c0: 2e68 6561 6428 3129 0d0a 2020 2020 2020  .head(1)..      
-000229d0: 2020 6966 206c 656e 2872 6563 656e 7429    if len(recent)
-000229e0: 203c 2031 3a0d 0a20 2020 2020 2020 2020   < 1:..         
-000229f0: 2020 2072 6574 7572 6e20 4661 6c73 650d     return False.
-00022a00: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
-00022a10: 6461 7461 2920 3c20 6461 7973 546f 4c6f  data) < daysToLo
-00022a20: 6f6b 6261 636b 2061 6e64 2028 0d0a 2020  okback and (..  
-00022a30: 2020 2020 2020 2020 2020 7265 6365 6e74            recent
-00022a40: 5b22 436c 6f73 6522 5d2e 696c 6f63 5b30  ["Close"].iloc[0
-00022a50: 5d20 213d 206e 702e 6e61 6e20 616e 6420  ] != np.nan and 
-00022a60: 7265 6365 6e74 5b22 436c 6f73 6522 5d2e  recent["Close"].
-00022a70: 696c 6f63 5b30 5d20 3e20 300d 0a20 2020  iloc[0] > 0..   
-00022a80: 2020 2020 2029 3a0d 0a20 2020 2020 2020       ):..       
-00022a90: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
-00022aa0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00022ab0: 2046 616c 7365 0d0a 0d0a 2020 2020 2320   False....    # 
-00022ac0: 5661 6c69 6461 7465 2069 6620 7468 6520  Validate if the 
-00022ad0: 7374 6f63 6b20 7072 6963 6573 2061 7265  stock prices are
-00022ae0: 2061 7420 6c65 6173 7420 7269 7369 6e67   at least rising
-00022af0: 2062 7920 3225 2066 6f72 2074 6865 206c   by 2% for the l
-00022b00: 6173 7420 3320 7365 7373 696f 6e73 0d0a  ast 3 sessions..
-00022b10: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
-00022b20: 5072 6963 6552 6973 696e 6742 7941 744c  PriceRisingByAtL
-00022b30: 6561 7374 3250 6572 6365 6e74 2873 656c  east2Percent(sel
-00022b40: 662c 2064 662c 2073 6372 6565 6e44 6963  f, df, screenDic
-00022b50: 742c 2073 6176 6544 6963 7429 3a0d 0a20  t, saveDict):.. 
-00022b60: 2020 2020 2020 2069 6620 6466 2069 7320         if df is 
-00022b70: 4e6f 6e65 206f 7220 6c65 6e28 6466 2920  None or len(df) 
-00022b80: 3d3d 2030 3a0d 0a20 2020 2020 2020 2020  == 0:..         
-00022b90: 2020 2072 6574 7572 6e20 4661 6c73 650d     return False.
-00022ba0: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
-00022bb0: 6466 2e63 6f70 7928 290d 0a20 2020 2020  df.copy()..     
-00022bc0: 2020 2064 6174 6120 3d20 6461 7461 2e66     data = data.f
-00022bd0: 696c 6c6e 6128 3029 0d0a 2020 2020 2020  illna(0)..      
-00022be0: 2020 6461 7461 203d 2064 6174 612e 7265    data = data.re
-00022bf0: 706c 6163 6528 5b6e 702e 696e 662c 202d  place([np.inf, -
-00022c00: 6e70 2e69 6e66 5d2c 2030 290d 0a20 2020  np.inf], 0)..   
-00022c10: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
-00022c20: 2e68 6561 6428 3429 0d0a 2020 2020 2020  .head(4)..      
-00022c30: 2020 6966 206c 656e 2864 6174 6129 203c    if len(data) <
-00022c40: 2034 3a0d 0a20 2020 2020 2020 2020 2020   4:..           
-00022c50: 2072 6574 7572 6e20 4661 6c73 650d 0a20   return False.. 
-00022c60: 2020 2020 2020 2064 6179 3020 3d20 6461         day0 = da
-00022c70: 7461 2e69 6c6f 635b 305d 5b22 436c 6f73  ta.iloc[0]["Clos
-00022c80: 6522 5d2e 6974 656d 2829 0d0a 2020 2020  e"].item()..    
-00022c90: 2020 2020 6461 794d 696e 7573 3120 3d20      dayMinus1 = 
-00022ca0: 6461 7461 2e69 6c6f 635b 315d 5b22 436c  data.iloc[1]["Cl
-00022cb0: 6f73 6522 5d2e 6974 656d 2829 0d0a 2020  ose"].item()..  
-00022cc0: 2020 2020 2020 6461 794d 696e 7573 3220        dayMinus2 
-00022cd0: 3d20 6461 7461 2e69 6c6f 635b 325d 5b22  = data.iloc[2]["
-00022ce0: 436c 6f73 6522 5d2e 6974 656d 2829 0d0a  Close"].item()..
-00022cf0: 2020 2020 2020 2020 6461 794d 696e 7573          dayMinus
-00022d00: 3320 3d20 6461 7461 2e69 6c6f 635b 335d  3 = data.iloc[3]
-00022d10: 5b22 436c 6f73 6522 5d2e 6974 656d 2829  ["Close"].item()
-00022d20: 0d0a 2020 2020 2020 2020 7065 7263 656e  ..        percen
-00022d30: 7433 203d 2072 6f75 6e64 2828 6461 794d  t3 = round((dayM
-00022d40: 696e 7573 3220 2d20 6461 794d 696e 7573  inus2 - dayMinus
-00022d50: 3329 202a 2031 3030 202f 2064 6179 4d69  3) * 100 / dayMi
-00022d60: 6e75 7333 2c20 3229 0d0a 2020 2020 2020  nus3, 2)..      
-00022d70: 2020 7065 7263 656e 7432 203d 2072 6f75    percent2 = rou
-00022d80: 6e64 2828 6461 794d 696e 7573 3120 2d20  nd((dayMinus1 - 
-00022d90: 6461 794d 696e 7573 3229 202a 2031 3030  dayMinus2) * 100
-00022da0: 202f 2064 6179 4d69 6e75 7332 2c20 3229   / dayMinus2, 2)
-00022db0: 0d0a 2020 2020 2020 2020 7065 7263 656e  ..        percen
-00022dc0: 7431 203d 2072 6f75 6e64 2828 6461 7930  t1 = round((day0
-00022dd0: 202d 2064 6179 4d69 6e75 7331 2920 2a20   - dayMinus1) * 
-00022de0: 3130 3020 2f20 6461 794d 696e 7573 312c  100 / dayMinus1,
-00022df0: 2032 290d 0a0d 0a20 2020 2020 2020 2069   2)....        i
-00022e00: 6620 7065 7263 656e 7431 203e 3d20 3220  f percent1 >= 2 
-00022e10: 616e 6420 7065 7263 656e 7432 203e 3d20  and percent2 >= 
-00022e20: 3220 616e 6420 7065 7263 656e 7433 203e  2 and percent3 >
-00022e30: 3d20 323a 0d0a 2020 2020 2020 2020 2020  = 2:..          
-00022e40: 2020 7063 745f 6368 616e 6765 5f74 6578    pct_change_tex
-00022e50: 7420 3d20 280d 0a20 2020 2020 2020 2020  t = (..         
-00022e60: 2020 2020 2020 2028 2225 2e31 6625 2522         ("%.1f%%"
-00022e70: 2025 2070 6572 6365 6e74 3129 0d0a 2020   % percent1)..  
-00022e80: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-00022e90: 2822 2028 252e 3166 2525 2c22 2025 2070  (" (%.1f%%," % p
-00022ea0: 6572 6365 6e74 3229 0d0a 2020 2020 2020  ercent2)..      
-00022eb0: 2020 2020 2020 2020 2020 2b20 2822 2025            + (" %
-00022ec0: 2e31 6625 2529 2220 2520 7065 7263 656e  .1f%%)" % percen
-00022ed0: 7433 290d 0a20 2020 2020 2020 2020 2020  t3)..           
-00022ee0: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
-00022ef0: 7361 7665 4469 6374 5b22 2543 686e 6722  saveDict["%Chng"
-00022f00: 5d20 3d20 7063 745f 6368 616e 6765 5f74  ] = pct_change_t
-00022f10: 6578 740d 0a20 2020 2020 2020 2020 2020  ext..           
-00022f20: 2073 6372 6565 6e44 6963 745b 2225 4368   screenDict["%Ch
-00022f30: 6e67 225d 203d 2063 6f6c 6f72 5465 7874  ng"] = colorText
-00022f40: 2e47 5245 454e 202b 2070 6374 5f63 6861  .GREEN + pct_cha
-00022f50: 6e67 655f 7465 7874 202b 2063 6f6c 6f72  nge_text + color
-00022f60: 5465 7874 2e45 4e44 0d0a 2020 2020 2020  Text.END..      
-00022f70: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
-00022f80: 6520 616e 6420 7365 6c66 2e67 6574 4361  e and self.getCa
-00022f90: 6e64 6c65 5479 7065 2864 6174 612e 6865  ndleType(data.he
-00022fa0: 6164 2831 2929 0d0a 2020 2020 2020 2020  ad(1))..        
-00022fb0: 7265 7475 726e 2046 616c 7365 0d0a 0d0a  return False....
-00022fc0: 2020 2020 2340 6d65 6173 7572 655f 7469      #@measure_ti
-00022fd0: 6d65 0d0a 2020 2020 2320 7661 6c69 6461  me..    # valida
-00022fe0: 7465 2069 6620 5253 4920 6973 2077 6974  te if RSI is wit
-00022ff0: 6869 6e20 6769 7665 6e20 7261 6e67 650d  hin given range.
-00023000: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
-00023010: 6552 5349 2873 656c 662c 2064 662c 2073  eRSI(self, df, s
-00023020: 6372 6565 6e44 6963 742c 2073 6176 6544  creenDict, saveD
-00023030: 6963 742c 206d 696e 5253 492c 206d 6178  ict, minRSI, max
-00023040: 5253 492c 7273 694b 6579 3d22 5253 4922  RSI,rsiKey="RSI"
-00023050: 293a 0d0a 2020 2020 2020 2020 6966 2064  ):..        if d
-00023060: 6620 6973 204e 6f6e 6520 6f72 206c 656e  f is None or len
-00023070: 2864 6629 203d 3d20 303a 0d0a 2020 2020  (df) == 0:..    
-00023080: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-00023090: 616c 7365 0d0a 2020 2020 2020 2020 6966  alse..        if
-000230a0: 2072 7369 4b65 7920 6e6f 7420 696e 2064   rsiKey not in d
-000230b0: 662e 636f 6c75 6d6e 733a 0d0a 2020 2020  f.columns:..    
-000230c0: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-000230d0: 616c 7365 0d0a 2020 2020 2020 2020 6461  alse..        da
-000230e0: 7461 203d 2064 662e 636f 7079 2829 0d0a  ta = df.copy()..
-000230f0: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
-00023100: 6174 612e 6669 6c6c 6e61 2830 290d 0a20  ata.fillna(0).. 
-00023110: 2020 2020 2020 2064 6174 6120 3d20 6461         data = da
-00023120: 7461 2e72 6570 6c61 6365 285b 6e70 2e69  ta.replace([np.i
-00023130: 6e66 2c20 2d6e 702e 696e 665d 2c20 3029  nf, -np.inf], 0)
-00023140: 0d0a 2020 2020 2020 2020 7273 6920 3d20  ..        rsi = 
-00023150: 696e 7428 6461 7461 2e68 6561 6428 3129  int(data.head(1)
-00023160: 5b72 7369 4b65 795d 2e69 6c6f 635b 305d  [rsiKey].iloc[0]
-00023170: 290d 0a20 2020 2020 2020 2073 6176 6544  )..        saveD
-00023180: 6963 745b 7273 694b 6579 5d20 3d20 7273  ict[rsiKey] = rs
-00023190: 690d 0a20 2020 2020 2020 2023 2068 7474  i..        # htt
-000231a0: 7073 3a2f 2f63 6861 7274 696e 6b2e 636f  ps://chartink.co
-000231b0: 6d2f 7363 7265 656e 6572 2f72 7369 2d73  m/screener/rsi-s
-000231c0: 6372 6565 6e69 6e67 0d0a 2020 2020 2020  creening..      
-000231d0: 2020 6966 2072 7369 3e20 3020 616e 6420    if rsi> 0 and 
-000231e0: 7273 6920 3e3d 206d 696e 5253 4920 616e  rsi >= minRSI an
-000231f0: 6420 7273 6920 3c3d 206d 6178 5253 493a  d rsi <= maxRSI:
-00023200: 2020 2320 6f72 2028 7273 6920 3c3d 2037    # or (rsi <= 7
-00023210: 3120 616e 6420 7273 6920 3e3d 2036 3729  1 and rsi >= 67)
-00023220: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-00023230: 6372 6565 6e44 6963 745b 7273 694b 6579  creenDict[rsiKey
-00023240: 5d20 3d20 280d 0a20 2020 2020 2020 2020  ] = (..         
-00023250: 2020 2020 2020 2063 6f6c 6f72 5465 7874         colorText
-00023260: 2e42 4f4c 4420 2b20 636f 6c6f 7254 6578  .BOLD + colorTex
-00023270: 742e 4752 4545 4e20 2b20 7374 7228 7273  t.GREEN + str(rs
-00023280: 6929 202b 2063 6f6c 6f72 5465 7874 2e45  i) + colorText.E
-00023290: 4e44 0d0a 2020 2020 2020 2020 2020 2020  ND..            
-000232a0: 290d 0a20 2020 2020 2020 2020 2020 2072  )..            r
-000232b0: 6574 7572 6e20 5472 7565 2069 6620 2872  eturn True if (r
-000232c0: 7369 4b65 7920 3d3d 2022 5253 4969 2229  siKey == "RSIi")
-000232d0: 2065 6c73 6520 2873 656c 662e 7661 6c69   else (self.vali
-000232e0: 6461 7465 5253 4928 6466 2c20 7363 7265  dateRSI(df, scre
-000232f0: 656e 4469 6374 2c20 7361 7665 4469 6374  enDict, saveDict
-00023300: 2c20 6d69 6e52 5349 2c20 6d61 7852 5349  , minRSI, maxRSI
-00023310: 2c72 7369 4b65 793d 2252 5349 6922 2920  ,rsiKey="RSIi") 
-00023320: 6f72 2054 7275 6529 0d0a 2020 2020 2020  or True)..      
-00023330: 2020 7363 7265 656e 4469 6374 5b72 7369    screenDict[rsi
-00023340: 4b65 795d 203d 2063 6f6c 6f72 5465 7874  Key] = colorText
-00023350: 2e42 4f4c 4420 2b20 636f 6c6f 7254 6578  .BOLD + colorTex
-00023360: 742e 4641 494c 202b 2073 7472 2872 7369  t.FAIL + str(rsi
-00023370: 2920 2b20 636f 6c6f 7254 6578 742e 454e  ) + colorText.EN
-00023380: 440d 0a20 2020 2020 2020 2023 2049 6620  D..        # If 
-00023390: 6569 7468 6572 2064 6169 6c79 206f 7220  either daily or 
-000233a0: 696e 7472 6164 6179 2052 5349 2063 6f6d  intraday RSI com
-000233b0: 6573 2077 6974 6869 6e20 7261 6e67 653f  es within range?
-000233c0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-000233d0: 2046 616c 7365 2069 6620 2872 7369 4b65   False if (rsiKe
-000233e0: 7920 3d3d 2022 5253 4969 2229 2065 6c73  y == "RSIi") els
-000233f0: 6520 2873 656c 662e 7661 6c69 6461 7465  e (self.validate
-00023400: 5253 4928 6466 2c20 7363 7265 656e 4469  RSI(df, screenDi
-00023410: 6374 2c20 7361 7665 4469 6374 2c20 6d69  ct, saveDict, mi
-00023420: 6e52 5349 2c20 6d61 7852 5349 2c72 7369  nRSI, maxRSI,rsi
-00023430: 4b65 793d 2252 5349 6922 2929 0d0a 0d0a  Key="RSIi"))....
-00023440: 2020 2020 2320 5661 6c69 6461 7465 2069      # Validate i
-00023450: 6620 7468 6520 7374 6f63 6b20 6973 2062  f the stock is b
-00023460: 756c 6c69 7368 2069 6e20 7468 6520 7368  ullish in the sh
-00023470: 6f72 7420 7465 726d 0d0a 2020 2020 6465  ort term..    de
-00023480: 6620 7661 6c69 6461 7465 5368 6f72 7454  f validateShortT
-00023490: 6572 6d42 756c 6c69 7368 2873 656c 662c  ermBullish(self,
-000234a0: 2064 662c 2073 6372 6565 6e44 6963 742c   df, screenDict,
-000234b0: 2073 6176 6544 6963 7429 3a0d 0a20 2020   saveDict):..   
-000234c0: 2020 2020 2069 6620 6466 2069 7320 4e6f       if df is No
-000234d0: 6e65 206f 7220 6c65 6e28 6466 2920 3d3d  ne or len(df) ==
-000234e0: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
-000234f0: 2072 6574 7572 6e20 4661 6c73 650d 0a20   return False.. 
-00023500: 2020 2020 2020 2064 6174 6120 3d20 6466         data = df
-00023510: 2e63 6f70 7928 290d 0a20 2020 2020 2020  .copy()..       
-00023520: 2023 2068 7474 7073 3a2f 2f63 6861 7274   # https://chart
-00023530: 696e 6b2e 636f 6d2f 7363 7265 656e 6572  ink.com/screener
-00023540: 2f73 686f 7274 2d74 6572 6d2d 6275 6c6c  /short-term-bull
-00023550: 6973 680d 0a20 2020 2020 2020 2064 6174  ish..        dat
-00023560: 6120 3d20 6461 7461 2e66 696c 6c6e 6128  a = data.fillna(
-00023570: 3029 0d0a 2020 2020 2020 2020 6461 7461  0)..        data
-00023580: 203d 2064 6174 612e 7265 706c 6163 6528   = data.replace(
-00023590: 5b6e 702e 696e 662c 202d 6e70 2e69 6e66  [np.inf, -np.inf
-000235a0: 5d2c 2030 290d 0a20 2020 2020 2020 2072  ], 0)..        r
-000235b0: 6563 656e 7420 3d20 6461 7461 2e68 6561  ecent = data.hea
-000235c0: 6428 3129 0d0a 2020 2020 2020 2020 666b  d(1)..        fk
-000235d0: 203d 2030 2069 6620 6c65 6e28 6461 7461   = 0 if len(data
-000235e0: 2920 3c20 3320 656c 7365 206e 702e 726f  ) < 3 else np.ro
-000235f0: 756e 6428 6461 7461 5b22 4641 5354 4b22  und(data["FASTK"
-00023600: 5d2e 696c 6f63 5b32 5d2c 2035 290d 0a20  ].iloc[2], 5).. 
-00023610: 2020 2020 2020 2023 2052 6576 6572 7365         # Reverse
-00023620: 2074 6865 2064 6174 6166 7261 6d65 2066   the dataframe f
-00023630: 6f72 2069 6368 696d 6f6b 7520 6361 6c63  or ichimoku calc
-00023640: 756c 6174 696f 6e73 2077 6974 6820 6461  ulations with da
-00023650: 7465 2069 6e20 6173 6365 6e64 696e 6720  te in ascending 
-00023660: 6f72 6465 720d 0a20 2020 2020 2020 2064  order..        d
-00023670: 665f 6e65 7720 3d20 6461 7461 5b3a 3a2d  f_new = data[::-
-00023680: 315d 0d0a 2020 2020 2020 2020 7472 793a  1]..        try:
-00023690: 0d0a 2020 2020 2020 2020 2020 2020 6466  ..            df
-000236a0: 5f69 6368 6920 3d20 6466 5f6e 6577 2e72  _ichi = df_new.r
-000236b0: 656e 616d 6528 0d0a 2020 2020 2020 2020  ename(..        
-000236c0: 2020 2020 2020 2020 636f 6c75 6d6e 733d          columns=
-000236d0: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
-000236e0: 2020 2020 2020 2022 4f70 656e 223a 2022         "Open": "
-000236f0: 6f70 656e 222c 0d0a 2020 2020 2020 2020  open",..        
-00023700: 2020 2020 2020 2020 2020 2020 2248 6967              "Hig
-00023710: 6822 3a20 2268 6967 6822 2c0d 0a20 2020  h": "high",..   
-00023720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023730: 2022 4c6f 7722 3a20 226c 6f77 222c 0d0a   "Low": "low",..
-00023740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023750: 2020 2020 2243 6c6f 7365 223a 2022 636c      "Close": "cl
-00023760: 6f73 6522 2c0d 0a20 2020 2020 2020 2020  ose",..         
-00023770: 2020 2020 2020 2020 2020 2022 566f 6c75             "Volu
-00023780: 6d65 223a 2022 766f 6c75 6d65 222c 0d0a  me": "volume",..
-00023790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000237a0: 7d0d 0a20 2020 2020 2020 2020 2020 2029  }..            )
-000237b0: 0d0a 2020 2020 2020 2020 2020 2020 6963  ..            ic
-000237c0: 6869 203d 2070 6b74 616c 6962 2e69 6368  hi = pktalib.ich
-000237d0: 696d 6f6b 7528 6466 5f69 6368 692c 2039  imoku(df_ichi, 9
-000237e0: 2c20 3236 2c20 3532 2c20 3236 290d 0a20  , 26, 52, 26).. 
-000237f0: 2020 2020 2020 2020 2020 2069 6620 6963             if ic
-00023800: 6869 2069 7320 4e6f 6e65 3a0d 0a20 2020  hi is None:..   
-00023810: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00023820: 7572 6e20 4661 6c73 650d 0a20 2020 2020  urn False..     
-00023830: 2020 2020 2020 2064 665f 6e65 7720 3d20         df_new = 
-00023840: 7064 2e63 6f6e 6361 7428 5b64 665f 6e65  pd.concat([df_ne
-00023850: 772c 2069 6368 695d 2c20 6178 6973 3d31  w, ichi], axis=1
-00023860: 290d 0a20 2020 2020 2020 2020 2020 2023  )..            #
-00023870: 2052 6576 6572 7365 2061 6761 696e 2074   Reverse again t
-00023880: 6f20 6765 7420 7468 6520 6d6f 7374 2072  o get the most r
-00023890: 6563 656e 7420 6461 7465 206f 6e20 746f  ecent date on to
-000238a0: 700d 0a20 2020 2020 2020 2020 2020 2064  p..            d
-000238b0: 665f 6e65 7720 3d20 6466 5f6e 6577 5b3a  f_new = df_new[:
-000238c0: 3a2d 315d 0d0a 2020 2020 2020 2020 2020  :-1]..          
-000238d0: 2020 6466 5f6e 6577 203d 2064 665f 6e65    df_new = df_ne
-000238e0: 772e 6865 6164 2831 290d 0a20 2020 2020  w.head(1)..     
-000238f0: 2020 2020 2020 2064 665f 6e65 775b 2263         df_new["c
-00023900: 6c6f 7564 5f67 7265 656e 225d 203d 2064  loud_green"] = d
-00023910: 665f 6e65 775b 2249 5341 5f39 225d 2e69  f_new["ISA_9"].i
-00023920: 6c6f 635b 305d 203e 2064 665f 6e65 775b  loc[0] > df_new[
-00023930: 2249 5342 5f32 3622 5d2e 696c 6f63 5b30  "ISB_26"].iloc[0
-00023940: 5d0d 0a20 2020 2020 2020 2020 2020 2064  ]..            d
-00023950: 665f 6e65 775b 2263 6c6f 7564 5f72 6564  f_new["cloud_red
-00023960: 225d 203d 2064 665f 6e65 775b 2249 5342  "] = df_new["ISB
-00023970: 5f32 3622 5d2e 696c 6f63 5b30 5d20 3e20  _26"].iloc[0] > 
-00023980: 6466 5f6e 6577 5b22 4953 415f 3922 5d2e  df_new["ISA_9"].
-00023990: 696c 6f63 5b30 5d0d 0a20 2020 2020 2020  iloc[0]..       
-000239a0: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
-000239b0: 6e20 6173 2065 3a20 2023 2070 7261 676d  n as e:  # pragm
-000239c0: 613a 206e 6f20 636f 7665 720d 0a20 2020  a: no cover..   
-000239d0: 2020 2020 2020 2020 2073 656c 662e 6465           self.de
-000239e0: 6661 756c 745f 6c6f 6767 6572 2e64 6562  fault_logger.deb
-000239f0: 7567 2865 2c20 6578 635f 696e 666f 3d54  ug(e, exc_info=T
-00023a00: 7275 6529 0d0a 2020 2020 2020 2020 2020  rue)..          
-00023a10: 2020 7061 7373 0d0a 2020 2020 2020 2020    pass..        
-00023a20: 6162 6f76 6543 6c6f 7564 546f 7020 3d20  aboveCloudTop = 
-00023a30: 4661 6c73 650d 0a20 2020 2020 2020 2023  False..        #
-00023a40: 2062 6173 656c 696e 6520 3e20 636c 6f75   baseline > clou
-00023a50: 6420 746f 7020 2863 6c6f 7564 2069 7320  d top (cloud is 
-00023a60: 626f 756e 6420 6279 2073 7061 6e20 6120  bound by span a 
-00023a70: 616e 6420 7370 616e 2062 2920 616e 6420  and span b) and 
-00023a80: 636c 6f73 6520 6973 203e 2063 6c6f 7564  close is > cloud
-00023a90: 2074 6f70 0d0a 2020 2020 2020 2020 6966   top..        if
-00023aa0: 2064 665f 6e65 775b 2263 6c6f 7564 5f67   df_new["cloud_g
-00023ab0: 7265 656e 225d 2e69 6c6f 635b 305d 3a0d  reen"].iloc[0]:.
-00023ac0: 0a20 2020 2020 2020 2020 2020 2061 626f  .            abo
-00023ad0: 7665 436c 6f75 6454 6f70 203d 2028 0d0a  veCloudTop = (..
-00023ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023af0: 6466 5f6e 6577 5b22 494b 535f 3236 225d  df_new["IKS_26"]
-00023b00: 2e69 6c6f 635b 305d 203e 2064 665f 6e65  .iloc[0] > df_ne
-00023b10: 775b 2249 5341 5f39 225d 2e69 6c6f 635b  w["ISA_9"].iloc[
-00023b20: 305d 0d0a 2020 2020 2020 2020 2020 2020  0]..            
-00023b30: 2020 2020 616e 6420 7265 6365 6e74 5b22      and recent["
-00023b40: 436c 6f73 6522 5d2e 696c 6f63 5b30 5d20  Close"].iloc[0] 
-00023b50: 3e20 6466 5f6e 6577 5b22 4953 415f 3922  > df_new["ISA_9"
-00023b60: 5d2e 696c 6f63 5b30 5d0d 0a20 2020 2020  ].iloc[0]..     
-00023b70: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-00023b80: 2020 656c 6966 2064 665f 6e65 775b 2263    elif df_new["c
-00023b90: 6c6f 7564 5f72 6564 225d 2e69 6c6f 635b  loud_red"].iloc[
-00023ba0: 305d 3a0d 0a20 2020 2020 2020 2020 2020  0]:..           
-00023bb0: 2061 626f 7665 436c 6f75 6454 6f70 203d   aboveCloudTop =
-00023bc0: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
-00023bd0: 2020 2020 6466 5f6e 6577 5b22 494b 535f      df_new["IKS_
-00023be0: 3236 225d 2e69 6c6f 635b 305d 203e 2064  26"].iloc[0] > d
-00023bf0: 665f 6e65 775b 2249 5342 5f32 3622 5d2e  f_new["ISB_26"].
-00023c00: 696c 6f63 5b30 5d0d 0a20 2020 2020 2020  iloc[0]..       
-00023c10: 2020 2020 2020 2020 2061 6e64 2072 6563           and rec
-00023c20: 656e 745b 2243 6c6f 7365 225d 2e69 6c6f  ent["Close"].ilo
-00023c30: 635b 305d 203e 2064 665f 6e65 775b 2249  c[0] > df_new["I
-00023c40: 5342 5f32 3622 5d2e 696c 6f63 5b30 5d0d  SB_26"].iloc[0].
-00023c50: 0a20 2020 2020 2020 2020 2020 2029 0d0a  .            )..
-00023c60: 0d0a 2020 2020 2020 2020 2320 4c61 7465  ..        # Late
-00023c70: 7374 2049 6368 696d 6f6b 7520 6261 7365  st Ichimoku base
-00023c80: 6c69 6e65 2069 7320 3c20 6c61 7465 7374  line is < latest
-00023c90: 2049 6368 696d 6f6b 7520 636f 6e76 6572   Ichimoku conver
-00023ca0: 7369 6f6e 206c 696e 650d 0a20 2020 2020  sion line..     
-00023cb0: 2020 2069 6620 6162 6f76 6543 6c6f 7564     if aboveCloud
-00023cc0: 546f 7020 616e 6420 6466 5f6e 6577 5b22  Top and df_new["
-00023cd0: 494b 535f 3236 225d 2e69 6c6f 635b 305d  IKS_26"].iloc[0]
-00023ce0: 203c 2064 665f 6e65 775b 2249 5453 5f39   < df_new["ITS_9
-00023cf0: 225d 2e69 6c6f 635b 305d 3a0d 0a20 2020  "].iloc[0]:..   
-00023d00: 2020 2020 2020 2020 2023 2053 746f 6368           # Stoch
-00023d10: 5253 4920 6372 6f73 7365 6420 3230 2061  RSI crossed 20 a
-00023d20: 6e64 2052 5349 203e 2035 300d 0a20 2020  nd RSI > 50..   
-00023d30: 2020 2020 2020 2020 2069 6620 666b 203e           if fk >
-00023d40: 2032 3020 616e 6420 7265 6365 6e74 5b22   20 and recent["
-00023d50: 5253 4922 5d2e 696c 6f63 5b30 5d20 3e20  RSI"].iloc[0] > 
-00023d60: 3530 3a0d 0a20 2020 2020 2020 2020 2020  50:..           
-00023d70: 2020 2020 2023 2063 6f6e 6469 7469 6f6e       # condition
-00023d80: 206f 6620 6372 6f73 7369 6e67 2074 6865   of crossing the
-00023d90: 2053 746f 6368 5253 4920 6d61 696e 2073   StochRSI main s
-00023da0: 6967 6e61 6c20 6c69 6e65 2066 726f 6d20  ignal line from 
-00023db0: 626f 7474 6f6d 2074 6f20 746f 700d 0a20  bottom to top.. 
-00023dc0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00023dd0: 6620 280d 0a20 2020 2020 2020 2020 2020  f (..           
-00023de0: 2020 2020 2020 2020 2064 6174 615b 2246           data["F
-00023df0: 4153 5444 225d 2e69 6c6f 635b 3130 305d  ASTD"].iloc[100]
-00023e00: 203c 2064 6174 615b 2246 4153 544b 225d   < data["FASTK"]
-00023e10: 2e69 6c6f 635b 3130 305d 0d0a 2020 2020  .iloc[100]..    
-00023e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023e30: 616e 6420 6461 7461 5b22 4641 5354 4422  and data["FASTD"
-00023e40: 5d2e 696c 6f63 5b31 3031 5d20 3e20 6461  ].iloc[101] > da
-00023e50: 7461 5b22 4641 5354 4b22 5d2e 696c 6f63  ta["FASTK"].iloc
-00023e60: 5b31 3031 5d0d 0a20 2020 2020 2020 2020  [101]..         
-00023e70: 2020 2020 2020 2029 3a0d 0a20 2020 2020         ):..     
-00023e80: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00023e90: 2063 6c6f 7365 203e 2035 3020 7065 7269   close > 50 peri
-00023ea0: 6f64 2053 4d41 2f45 4d41 2061 6e64 2032  od SMA/EMA and 2
-00023eb0: 3030 2070 6572 696f 6420 534d 412f 454d  00 period SMA/EM
-00023ec0: 410d 0a20 2020 2020 2020 2020 2020 2020  A..             
-00023ed0: 2020 2020 2020 2069 6620 280d 0a20 2020         if (..   
-00023ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023ef0: 2020 2020 2072 6563 656e 745b 2253 534d       recent["SSM
-00023f00: 4122 5d2e 696c 6f63 5b30 5d20 3e20 7265  A"].iloc[0] > re
-00023f10: 6365 6e74 5b22 534d 4122 5d2e 696c 6f63  cent["SMA"].iloc
-00023f20: 5b30 5d0d 0a20 2020 2020 2020 2020 2020  [0]..           
-00023f30: 2020 2020 2020 2020 2020 2020 2061 6e64               and
-00023f40: 2072 6563 656e 745b 2243 6c6f 7365 225d   recent["Close"]
-00023f50: 2e69 6c6f 635b 305d 203e 2072 6563 656e  .iloc[0] > recen
-00023f60: 745b 2253 534d 4122 5d2e 696c 6f63 5b30  t["SSMA"].iloc[0
-00023f70: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00023f80: 2020 2020 2020 2020 2020 2061 6e64 2072             and r
-00023f90: 6563 656e 745b 2243 6c6f 7365 225d 2e69  ecent["Close"].i
-00023fa0: 6c6f 635b 305d 203e 2072 6563 656e 745b  loc[0] > recent[
-00023fb0: 224c 4d41 225d 2e69 6c6f 635b 305d 0d0a  "LMA"].iloc[0]..
-00023fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023fd0: 2020 2020 293a 0d0a 2020 2020 2020 2020      ):..        
-00023fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023ff0: 7361 7665 6420 3d20 7365 6c66 2e66 696e  saved = self.fin
-00024000: 6443 7572 7265 6e74 5361 7665 6456 616c  dCurrentSavedVal
-00024010: 7565 2873 6372 6565 6e44 6963 742c 7361  ue(screenDict,sa
-00024020: 7665 4469 6374 2c22 4d41 2d53 6967 6e61  veDict,"MA-Signa
-00024030: 6c22 290d 0a20 2020 2020 2020 2020 2020  l")..           
-00024040: 2020 2020 2020 2020 2020 2020 2073 6372               scr
-00024050: 6565 6e44 6963 745b 224d 412d 5369 676e  eenDict["MA-Sign
-00024060: 616c 225d 203d 2028 0d0a 2020 2020 2020  al"] = (..      
-00024070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024080: 2020 2020 2020 7361 7665 645b 305d 202b        saved[0] +
-00024090: 2063 6f6c 6f72 5465 7874 2e42 4f4c 4420   colorText.BOLD 
-000240a0: 2b20 636f 6c6f 7254 6578 742e 4752 4545  + colorText.GREE
-000240b0: 4e20 2b20 2242 756c 6c69 7368 2220 2b20  N + "Bullish" + 
-000240c0: 636f 6c6f 7254 6578 742e 454e 440d 0a20  colorText.END.. 
-000240d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000240e0: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-000240f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024100: 2020 7361 7665 4469 6374 5b22 4d41 2d53    saveDict["MA-S
-00024110: 6967 6e61 6c22 5d20 3d20 7361 7665 645b  ignal"] = saved[
-00024120: 315d 202b 2022 4275 6c6c 6973 6822 0d0a  1] + "Bullish"..
-00024130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024140: 2020 2020 2020 2020 7265 7475 726e 2054          return T
-00024150: 7275 650d 0a20 2020 2020 2020 2072 6574  rue..        ret
-00024160: 7572 6e20 4661 6c73 650d 0a0d 0a20 2020  urn False....   
-00024170: 2023 2056 616c 6964 6174 6520 5650 430d   # Validate VPC.
-00024180: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
-00024190: 6556 4350 280d 0a20 2020 2020 2020 2073  eVCP(..        s
-000241a0: 656c 662c 2064 662c 2073 6372 6565 6e44  elf, df, screenD
-000241b0: 6963 742c 2073 6176 6544 6963 742c 2073  ict, saveDict, s
-000241c0: 746f 636b 4e61 6d65 3d4e 6f6e 652c 2077  tockName=None, w
-000241d0: 696e 646f 773d 332c 2070 6572 6365 6e74  indow=3, percent
-000241e0: 6167 6546 726f 6d54 6f70 3d33 0d0a 2020  ageFromTop=3..  
-000241f0: 2020 293a 0d0a 2020 2020 2020 2020 6966    ):..        if
-00024200: 2064 6620 6973 204e 6f6e 6520 6f72 206c   df is None or l
-00024210: 656e 2864 6629 203d 3d20 303a 0d0a 2020  en(df) == 0:..  
-00024220: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00024230: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
-00024240: 6461 7461 203d 2064 662e 636f 7079 2829  data = df.copy()
-00024250: 0d0a 2020 2020 2020 2020 7472 793a 0d0a  ..        try:..
-00024260: 2020 2020 2020 2020 2020 2020 7065 7263              perc
-00024270: 656e 7461 6765 4672 6f6d 546f 7020 2f3d  entageFromTop /=
-00024280: 2031 3030 0d0a 2020 2020 2020 2020 2020   100..          
-00024290: 2020 6461 7461 2e72 6573 6574 5f69 6e64    data.reset_ind
-000242a0: 6578 2869 6e70 6c61 6365 3d54 7275 6529  ex(inplace=True)
-000242b0: 0d0a 2020 2020 2020 2020 2020 2020 6461  ..            da
-000242c0: 7461 2e72 656e 616d 6528 636f 6c75 6d6e  ta.rename(column
-000242d0: 733d 7b22 696e 6465 7822 3a20 2244 6174  s={"index": "Dat
-000242e0: 6522 7d2c 2069 6e70 6c61 6365 3d54 7275  e"}, inplace=Tru
-000242f0: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
-00024300: 6461 7461 5b22 746f 7073 225d 203d 2028  data["tops"] = (
-00024310: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00024320: 2020 6461 7461 5b22 4869 6768 225d 0d0a    data["High"]..
-00024330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024340: 2e69 6c6f 635b 0d0a 2020 2020 2020 2020  .iloc[..        
-00024350: 2020 2020 2020 2020 2020 2020 6c69 7374              list
-00024360: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
-00024370: 2020 2020 2020 2020 2020 2070 6b74 616c             pktal
-00024380: 6962 2e61 7267 7265 6c65 7874 7265 6d61  ib.argrelextrema
-00024390: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
-000243a0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-000243b0: 702e 6172 7261 7928 6461 7461 5b22 4869  p.array(data["Hi
-000243c0: 6768 225d 292c 206e 702e 6772 6561 7465  gh"]), np.greate
-000243d0: 725f 6571 7561 6c2c 206f 7264 6572 3d77  r_equal, order=w
-000243e0: 696e 646f 770d 0a20 2020 2020 2020 2020  indow..         
-000243f0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00024400: 5b30 5d0d 0a20 2020 2020 2020 2020 2020  [0]..           
-00024410: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
-00024420: 2020 2020 2020 2020 2020 2020 5d0d 0a20              ].. 
-00024430: 2020 2020 2020 2020 2020 2020 2020 202e                 .
-00024440: 6865 6164 2834 290d 0a20 2020 2020 2020  head(4)..       
-00024450: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
-00024460: 2020 2020 6461 7461 5b22 626f 7473 225d      data["bots"]
-00024470: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
-00024480: 2020 2020 2020 6461 7461 5b22 4c6f 7722        data["Low"
-00024490: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-000244a0: 2020 202e 696c 6f63 5b0d 0a20 2020 2020     .iloc[..     
-000244b0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-000244c0: 6973 7428 0d0a 2020 2020 2020 2020 2020  ist(..          
-000244d0: 2020 2020 2020 2020 2020 2020 2020 706b                pk
-000244e0: 7461 6c69 622e 6172 6772 656c 6578 7472  talib.argrelextr
-000244f0: 656d 6128 0d0a 2020 2020 2020 2020 2020  ema(..          
-00024500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024510: 2020 6e70 2e61 7272 6179 2864 6174 615b    np.array(data[
-00024520: 224c 6f77 225d 292c 206e 702e 6c65 7373  "Low"]), np.less
-00024530: 5f65 7175 616c 2c20 6f72 6465 723d 7769  _equal, order=wi
-00024540: 6e64 6f77 0d0a 2020 2020 2020 2020 2020  ndow..          
-00024550: 2020 2020 2020 2020 2020 2020 2020 295b                )[
-00024560: 305d 0d0a 2020 2020 2020 2020 2020 2020  0]..            
-00024570: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
-00024580: 2020 2020 2020 2020 2020 205d 0d0a 2020             ]..  
-00024590: 2020 2020 2020 2020 2020 2020 2020 2e68                .h
-000245a0: 6561 6428 3429 0d0a 2020 2020 2020 2020  ead(4)..        
-000245b0: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
-000245c0: 2020 2064 6174 6120 3d20 6461 7461 2e66     data = data.f
-000245d0: 696c 6c6e 6128 3029 0d0a 2020 2020 2020  illna(0)..      
-000245e0: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
-000245f0: 612e 7265 706c 6163 6528 5b6e 702e 696e  a.replace([np.in
-00024600: 662c 202d 6e70 2e69 6e66 5d2c 2030 290d  f, -np.inf], 0).
-00024610: 0a20 2020 2020 2020 2020 2020 2074 6f70  .            top
-00024620: 7320 3d20 6461 7461 5b64 6174 612e 746f  s = data[data.to
-00024630: 7073 203e 2030 5d0d 0a20 2020 2020 2020  ps > 0]..       
-00024640: 2020 2020 2023 2062 6f74 7320 3d20 6461       # bots = da
-00024650: 7461 5b64 6174 612e 626f 7473 203e 2030  ta[data.bots > 0
-00024660: 5d0d 0a20 2020 2020 2020 2020 2020 2068  ]..            h
-00024670: 6967 6865 7374 546f 7020 3d20 726f 756e  ighestTop = roun
-00024680: 6428 746f 7073 2e64 6573 6372 6962 6528  d(tops.describe(
-00024690: 295b 2248 6967 6822 5d5b 226d 6178 225d  )["High"]["max"]
-000246a0: 2c20 3129 0d0a 2020 2020 2020 2020 2020  , 1)..          
-000246b0: 2020 6669 6c74 6572 6564 546f 7073 203d    filteredTops =
-000246c0: 2074 6f70 735b 0d0a 2020 2020 2020 2020   tops[..        
-000246d0: 2020 2020 2020 2020 746f 7073 2e74 6f70          tops.top
-000246e0: 7320 3e20 2868 6967 6865 7374 546f 7020  s > (highestTop 
-000246f0: 2d20 2868 6967 6865 7374 546f 7020 2a20  - (highestTop * 
-00024700: 7065 7263 656e 7461 6765 4672 6f6d 546f  percentageFromTo
-00024710: 7029 290d 0a20 2020 2020 2020 2020 2020  p))..           
-00024720: 205d 0d0a 2020 2020 2020 2020 2020 2020   ]..            
-00024730: 6966 2066 696c 7465 7265 6454 6f70 732e  if filteredTops.
-00024740: 6571 7561 6c73 2874 6f70 7329 3a20 2023  equals(tops):  #
-00024750: 2054 6f70 7320 6172 6520 696e 2074 6865   Tops are in the
-00024760: 2072 616e 6765 0d0a 2020 2020 2020 2020   range..        
-00024770: 2020 2020 2020 2020 6c6f 7750 6f69 6e74          lowPoint
-00024780: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
-00024790: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-000247a0: 2072 616e 6765 286c 656e 2874 6f70 7329   range(len(tops)
-000247b0: 202d 2031 293a 0d0a 2020 2020 2020 2020   - 1):..        
-000247c0: 2020 2020 2020 2020 2020 2020 656e 6444              endD
-000247d0: 6174 6520 3d20 746f 7073 2e69 6c6f 635b  ate = tops.iloc[
-000247e0: 695d 5b22 4461 7465 225d 0d0a 2020 2020  i]["Date"]..    
-000247f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024800: 7374 6172 7444 6174 6520 3d20 746f 7073  startDate = tops
-00024810: 2e69 6c6f 635b 6920 2b20 315d 5b22 4461  .iloc[i + 1]["Da
-00024820: 7465 225d 0d0a 2020 2020 2020 2020 2020  te"]..          
-00024830: 2020 2020 2020 2020 2020 6c6f 7750 6f69            lowPoi
-00024840: 6e74 732e 6170 7065 6e64 280d 0a20 2020  nts.append(..   
-00024850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024860: 2020 2020 2064 6174 615b 0d0a 2020 2020       data[..    
-00024870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024880: 2020 2020 2020 2020 2864 6174 612e 4461          (data.Da
-00024890: 7465 203e 3d20 7374 6172 7444 6174 6529  te >= startDate)
-000248a0: 2026 2028 6461 7461 2e44 6174 6520 3c3d   & (data.Date <=
-000248b0: 2065 6e64 4461 7465 290d 0a20 2020 2020   endDate)..     
-000248c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000248d0: 2020 205d 2e64 6573 6372 6962 6528 295b     ].describe()[
-000248e0: 224c 6f77 225d 5b22 6d69 6e22 5d0d 0a20  "Low"]["min"].. 
-000248f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024900: 2020 2029 0d0a 2020 2020 2020 2020 2020     )..          
-00024910: 2020 2020 2020 6c6f 7750 6f69 6e74 734f        lowPointsO
-00024920: 7267 203d 206c 6f77 506f 696e 7473 0d0a  rg = lowPoints..
-00024930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024940: 6c6f 7750 6f69 6e74 732e 736f 7274 2872  lowPoints.sort(r
-00024950: 6576 6572 7365 3d54 7275 6529 0d0a 2020  everse=True)..  
-00024960: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-00024970: 7750 6f69 6e74 7353 6f72 7465 6420 3d20  wPointsSorted = 
-00024980: 6c6f 7750 6f69 6e74 730d 0a20 2020 2020  lowPoints..     
-00024990: 2020 2020 2020 2020 2020 206c 7470 203d             ltp =
-000249a0: 2064 6174 612e 6865 6164 2831 295b 2243   data.head(1)["C
-000249b0: 6c6f 7365 225d 2e69 6c6f 635b 305d 0d0a  lose"].iloc[0]..
-000249c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000249d0: 6966 2028 0d0a 2020 2020 2020 2020 2020  if (..          
-000249e0: 2020 2020 2020 2020 2020 6c6f 7750 6f69            lowPoi
-000249f0: 6e74 734f 7267 203d 3d20 6c6f 7750 6f69  ntsOrg == lowPoi
-00024a00: 6e74 7353 6f72 7465 640d 0a20 2020 2020  ntsSorted..     
-00024a10: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00024a20: 6e64 206c 7470 203c 2068 6967 6865 7374  nd ltp < highest
-00024a30: 546f 700d 0a20 2020 2020 2020 2020 2020  Top..           
-00024a40: 2020 2020 2020 2020 2061 6e64 206c 7470           and ltp
-00024a50: 203e 206c 6f77 506f 696e 7473 5b30 5d0d   > lowPoints[0].
-00024a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00024a70: 2029 3a0d 0a20 2020 2020 2020 2020 2020   ):..           
-00024a80: 2020 2020 2020 2020 2073 6176 6564 203d           saved =
-00024a90: 2073 656c 662e 6669 6e64 4375 7272 656e   self.findCurren
-00024aa0: 7453 6176 6564 5661 6c75 6528 7363 7265  tSavedValue(scre
-00024ab0: 656e 4469 6374 2c20 7361 7665 4469 6374  enDict, saveDict
-00024ac0: 2c20 2250 6174 7465 726e 2229 0d0a 2020  , "Pattern")..  
-00024ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024ae0: 2020 7363 7265 656e 4469 6374 5b22 5061    screenDict["Pa
-00024af0: 7474 6572 6e22 5d20 3d20 280d 0a20 2020  ttern"] = (..   
+000218f0: 315d 202b 2022 3530 4d41 2d53 7570 706f  1] + "50MA-Suppo
+00021900: 7274 220d 0a20 2020 2020 2020 2020 2020  rt"..           
+00021910: 206d 6152 6576 6572 7361 6c20 3d20 310d   maReversal = 1.
+00021920: 0a20 2020 2020 2020 2023 2056 616c 6964  .        # Valid
+00021930: 6174 696e 6720 5265 7369 7374 616e 6365  ating Resistance
+00021940: 2035 300d 0a20 2020 2020 2020 2065 6c69   50..        eli
+00021950: 6620 636c 6f73 6520 3c20 736d 6120 616e  f close < sma an
+00021960: 6420 6869 6768 203e 3d20 2873 6d61 202d  d high >= (sma -
+00021970: 2073 6d61 4465 7629 3a0d 0a20 2020 2020   smaDev):..     
+00021980: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
+00021990: 745b 224d 412d 5369 676e 616c 225d 203d  t["MA-Signal"] =
+000219a0: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
+000219b0: 2020 2020 7361 7665 645b 305d 202b 2063      saved[0] + c
+000219c0: 6f6c 6f72 5465 7874 2e42 4f4c 4420 2b20  olorText.BOLD + 
+000219d0: 636f 6c6f 7254 6578 742e 4641 494c 202b  colorText.FAIL +
+000219e0: 2022 3530 4d41 2d52 6573 6973 7422 202b   "50MA-Resist" +
+000219f0: 2063 6f6c 6f72 5465 7874 2e45 4e44 0d0a   colorText.END..
+00021a00: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
+00021a10: 2020 2020 2020 2020 2020 2073 6176 6544             saveD
+00021a20: 6963 745b 224d 412d 5369 676e 616c 225d  ict["MA-Signal"]
+00021a30: 203d 2073 6176 6564 5b31 5d20 2b20 2235   = saved[1] + "5
+00021a40: 304d 412d 5265 7369 7374 220d 0a20 2020  0MA-Resist"..   
+00021a50: 2020 2020 2020 2020 206d 6152 6576 6572           maRever
+00021a60: 7361 6c20 3d20 2d31 0d0a 2020 2020 2020  sal = -1..      
+00021a70: 2020 2320 5461 6b69 6e67 2053 7570 706f    # Taking Suppo
+00021a80: 7274 2032 3030 0d0a 2020 2020 2020 2020  rt 200..        
+00021a90: 656c 6966 2063 6c6f 7365 203e 206c 6d61  elif close > lma
+00021aa0: 2061 6e64 206c 6f77 203c 3d20 286c 6d61   and low <= (lma
+00021ab0: 202b 206c 6d61 4465 7629 3a0d 0a20 2020   + lmaDev):..   
+00021ac0: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
+00021ad0: 6963 745b 224d 412d 5369 676e 616c 225d  ict["MA-Signal"]
+00021ae0: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
+00021af0: 2020 2020 2020 7361 7665 645b 305d 202b        saved[0] +
+00021b00: 2063 6f6c 6f72 5465 7874 2e42 4f4c 4420   colorText.BOLD 
+00021b10: 2b20 636f 6c6f 7254 6578 742e 4752 4545  + colorText.GREE
+00021b20: 4e20 2b20 2232 3030 4d41 2d53 7570 706f  N + "200MA-Suppo
+00021b30: 7274 2220 2b20 636f 6c6f 7254 6578 742e  rt" + colorText.
+00021b40: 454e 440d 0a20 2020 2020 2020 2020 2020  END..           
+00021b50: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
+00021b60: 7361 7665 4469 6374 5b22 4d41 2d53 6967  saveDict["MA-Sig
+00021b70: 6e61 6c22 5d20 3d20 7361 7665 645b 315d  nal"] = saved[1]
+00021b80: 202b 2022 3230 304d 412d 5375 7070 6f72   + "200MA-Suppor
+00021b90: 7422 0d0a 2020 2020 2020 2020 2020 2020  t"..            
+00021ba0: 6d61 5265 7665 7273 616c 203d 2031 0d0a  maReversal = 1..
+00021bb0: 2020 2020 2020 2020 2320 5661 6c69 6461          # Valida
+00021bc0: 7469 6e67 2052 6573 6973 7461 6e63 6520  ting Resistance 
+00021bd0: 3230 300d 0a20 2020 2020 2020 2065 6c69  200..        eli
+00021be0: 6620 636c 6f73 6520 3c20 6c6d 6120 616e  f close < lma an
+00021bf0: 6420 6869 6768 203e 3d20 286c 6d61 202d  d high >= (lma -
+00021c00: 206c 6d61 4465 7629 3a0d 0a20 2020 2020   lmaDev):..     
+00021c10: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
+00021c20: 745b 224d 412d 5369 676e 616c 225d 203d  t["MA-Signal"] =
+00021c30: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
+00021c40: 2020 2020 7361 7665 645b 305d 202b 2063      saved[0] + c
+00021c50: 6f6c 6f72 5465 7874 2e42 4f4c 4420 2b20  olorText.BOLD + 
+00021c60: 636f 6c6f 7254 6578 742e 4641 494c 202b  colorText.FAIL +
+00021c70: 2022 3230 304d 412d 5265 7369 7374 2220   "200MA-Resist" 
+00021c80: 2b20 636f 6c6f 7254 6578 742e 454e 440d  + colorText.END.
+00021c90: 0a20 2020 2020 2020 2020 2020 2029 0d0a  .            )..
+00021ca0: 2020 2020 2020 2020 2020 2020 7361 7665              save
+00021cb0: 4469 6374 5b22 4d41 2d53 6967 6e61 6c22  Dict["MA-Signal"
+00021cc0: 5d20 3d20 7361 7665 645b 315d 202b 2022  ] = saved[1] + "
+00021cd0: 3230 304d 412d 5265 7369 7374 220d 0a20  200MA-Resist".. 
+00021ce0: 2020 2020 2020 2020 2020 206d 6152 6576             maRev
+00021cf0: 6572 7361 6c20 3d20 2d31 0d0a 2020 2020  ersal = -1..    
+00021d00: 2020 2020 2320 466f 7220 6120 4275 6c6c      # For a Bull
+00021d10: 6973 6820 4361 6e64 6c65 0d0a 2020 2020  ish Candle..    
+00021d20: 2020 2020 6966 2073 656c 662e 6765 7443      if self.getC
+00021d30: 616e 646c 6554 7970 6528 6461 7461 293a  andleType(data):
+00021d40: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00021d50: 4372 6f73 7369 6e67 2075 7020 3530 0d0a  Crossing up 50..
+00021d60: 2020 2020 2020 2020 2020 2020 6966 206f              if o
+00021d70: 7065 6e20 3c20 736d 6120 616e 6420 636c  pen < sma and cl
+00021d80: 6f73 6520 3e20 736d 613a 0d0a 2020 2020  ose > sma:..    
+00021d90: 2020 2020 2020 2020 2020 2020 7363 7265              scre
+00021da0: 656e 4469 6374 5b22 4d41 2d53 6967 6e61  enDict["MA-Signa
+00021db0: 6c22 5d20 3d20 280d 0a20 2020 2020 2020  l"] = (..       
+00021dc0: 2020 2020 2020 2020 2020 2020 2073 6176               sav
+00021dd0: 6564 5b30 5d20 2b20 636f 6c6f 7254 6578  ed[0] + colorTex
+00021de0: 742e 424f 4c44 202b 2063 6f6c 6f72 5465  t.BOLD + colorTe
+00021df0: 7874 2e47 5245 454e 202b 2022 4275 6c6c  xt.GREEN + "Bull
+00021e00: 4372 6f73 732d 3530 4d41 2220 2b20 636f  Cross-50MA" + co
+00021e10: 6c6f 7254 6578 742e 454e 440d 0a20 2020  lorText.END..   
+00021e20: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
+00021e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021e40: 7361 7665 4469 6374 5b22 4d41 2d53 6967  saveDict["MA-Sig
+00021e50: 6e61 6c22 5d20 3d20 7361 7665 645b 315d  nal"] = saved[1]
+00021e60: 202b 2022 4275 6c6c 4372 6f73 732d 3530   + "BullCross-50
+00021e70: 4d41 220d 0a20 2020 2020 2020 2020 2020  MA"..           
+00021e80: 2020 2020 206d 6152 6576 6572 7361 6c20       maReversal 
+00021e90: 3d20 310d 0a20 2020 2020 2020 2020 2020  = 1..           
+00021ea0: 2023 2043 726f 7373 696e 6720 7570 2032   # Crossing up 2
+00021eb0: 3030 0d0a 2020 2020 2020 2020 2020 2020  00..            
+00021ec0: 656c 6966 206f 7065 6e20 3c20 6c6d 6120  elif open < lma 
+00021ed0: 616e 6420 636c 6f73 6520 3e20 6c6d 613a  and close > lma:
+00021ee0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00021ef0: 2020 7363 7265 656e 4469 6374 5b22 4d41    screenDict["MA
+00021f00: 2d53 6967 6e61 6c22 5d20 3d20 280d 0a20  -Signal"] = (.. 
+00021f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021f20: 2020 2073 6176 6564 5b30 5d20 2b20 636f     saved[0] + co
+00021f30: 6c6f 7254 6578 742e 424f 4c44 202b 2063  lorText.BOLD + c
+00021f40: 6f6c 6f72 5465 7874 2e47 5245 454e 202b  olorText.GREEN +
+00021f50: 2022 4275 6c6c 4372 6f73 732d 3230 304d   "BullCross-200M
+00021f60: 4122 202b 2063 6f6c 6f72 5465 7874 2e45  A" + colorText.E
+00021f70: 4e44 0d0a 2020 2020 2020 2020 2020 2020  ND..            
+00021f80: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
+00021f90: 2020 2020 2020 2073 6176 6544 6963 745b         saveDict[
+00021fa0: 224d 412d 5369 676e 616c 225d 203d 2073  "MA-Signal"] = s
+00021fb0: 6176 6564 5b31 5d20 2b20 2242 756c 6c43  aved[1] + "BullC
+00021fc0: 726f 7373 2d32 3030 4d41 220d 0a20 2020  ross-200MA"..   
+00021fd0: 2020 2020 2020 2020 2020 2020 206d 6152               maR
+00021fe0: 6576 6572 7361 6c20 3d20 310d 0a20 2020  eversal = 1..   
+00021ff0: 2020 2020 2023 2046 6f72 2061 2042 6561       # For a Bea
+00022000: 7269 7368 2043 616e 646c 650d 0a20 2020  rish Candle..   
+00022010: 2020 2020 2065 6c69 6620 6e6f 7420 7365       elif not se
+00022020: 6c66 2e67 6574 4361 6e64 6c65 5479 7065  lf.getCandleType
+00022030: 2864 6174 6129 3a0d 0a20 2020 2020 2020  (data):..       
+00022040: 2020 2020 2023 2043 726f 7373 696e 6720       # Crossing 
+00022050: 646f 776e 2035 300d 0a20 2020 2020 2020  down 50..       
+00022060: 2020 2020 2069 6620 6f70 656e 203e 2073       if open > s
+00022070: 6d61 2061 6e64 2063 6c6f 7365 203c 2073  ma and close < s
+00022080: 6d61 3a0d 0a20 2020 2020 2020 2020 2020  ma:..           
+00022090: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
+000220a0: 224d 412d 5369 676e 616c 225d 203d 2028  "MA-Signal"] = (
+000220b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000220c0: 2020 2020 2020 7361 7665 645b 305d 202b        saved[0] +
+000220d0: 2063 6f6c 6f72 5465 7874 2e42 4f4c 4420   colorText.BOLD 
+000220e0: 2b20 636f 6c6f 7254 6578 742e 4641 494c  + colorText.FAIL
+000220f0: 202b 2022 4265 6172 4372 6f73 732d 3530   + "BearCross-50
+00022100: 4d41 2220 2b20 636f 6c6f 7254 6578 742e  MA" + colorText.
+00022110: 454e 440d 0a20 2020 2020 2020 2020 2020  END..           
+00022120: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+00022130: 2020 2020 2020 2020 7361 7665 4469 6374          saveDict
+00022140: 5b22 4d41 2d53 6967 6e61 6c22 5d20 3d20  ["MA-Signal"] = 
+00022150: 7361 7665 645b 315d 202b 2022 4265 6172  saved[1] + "Bear
+00022160: 4372 6f73 732d 3530 4d41 220d 0a20 2020  Cross-50MA"..   
+00022170: 2020 2020 2020 2020 2020 2020 206d 6152               maR
+00022180: 6576 6572 7361 6c20 3d20 2d31 0d0a 2020  eversal = -1..  
+00022190: 2020 2020 2020 2020 2020 2320 4372 6f73            # Cros
+000221a0: 7369 6e67 2075 7020 3230 300d 0a20 2020  sing up 200..   
+000221b0: 2020 2020 2020 2020 2065 6c69 6620 6f70           elif op
+000221c0: 656e 203e 206c 6d61 2061 6e64 2063 6c6f  en > lma and clo
+000221d0: 7365 203c 206c 6d61 3a0d 0a20 2020 2020  se < lma:..     
+000221e0: 2020 2020 2020 2020 2020 2073 6372 6565             scree
+000221f0: 6e44 6963 745b 224d 412d 5369 676e 616c  nDict["MA-Signal
+00022200: 225d 203d 2028 0d0a 2020 2020 2020 2020  "] = (..        
+00022210: 2020 2020 2020 2020 2020 2020 7361 7665              save
+00022220: 645b 305d 202b 2063 6f6c 6f72 5465 7874  d[0] + colorText
+00022230: 2e42 4f4c 4420 2b20 636f 6c6f 7254 6578  .BOLD + colorTex
+00022240: 742e 4641 494c 202b 2022 4265 6172 4372  t.FAIL + "BearCr
+00022250: 6f73 732d 3230 304d 4122 202b 2063 6f6c  oss-200MA" + col
+00022260: 6f72 5465 7874 2e45 4e44 0d0a 2020 2020  orText.END..    
+00022270: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
+00022280: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00022290: 6176 6544 6963 745b 224d 412d 5369 676e  aveDict["MA-Sign
+000222a0: 616c 225d 203d 2073 6176 6564 5b31 5d20  al"] = saved[1] 
+000222b0: 2b20 2242 6561 7243 726f 7373 2d32 3030  + "BearCross-200
+000222c0: 4d41 220d 0a20 2020 2020 2020 2020 2020  MA"..           
+000222d0: 2020 2020 206d 6152 6576 6572 7361 6c20       maReversal 
+000222e0: 3d20 2d31 0d0a 2020 2020 2020 2020 7265  = -1..        re
+000222f0: 7475 726e 206d 6152 6576 6572 7361 6c0d  turn maReversal.
+00022300: 0a0d 0a20 2020 2023 2046 696e 6420 4e52  ...    # Find NR
+00022310: 7820 7261 6e67 6520 666f 7220 5265 7665  x range for Reve
+00022320: 7273 616c 0d0a 2020 2020 6465 6620 7661  rsal..    def va
+00022330: 6c69 6461 7465 4e61 7272 6f77 5261 6e67  lidateNarrowRang
+00022340: 6528 7365 6c66 2c20 6466 2c20 7363 7265  e(self, df, scre
+00022350: 656e 4469 6374 2c20 7361 7665 4469 6374  enDict, saveDict
+00022360: 2c20 6e72 3d34 293a 0d0a 2020 2020 2020  , nr=4):..      
+00022370: 2020 6966 2064 6620 6973 204e 6f6e 6520    if df is None 
+00022380: 6f72 206c 656e 2864 6629 203d 3d20 303a  or len(df) == 0:
+00022390: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+000223a0: 7475 726e 2046 616c 7365 0d0a 2020 2020  turn False..    
+000223b0: 2020 2020 6461 7461 203d 2064 662e 636f      data = df.co
+000223c0: 7079 2829 0d0a 2020 2020 2020 2020 7361  py()..        sa
+000223d0: 7665 6420 3d20 7365 6c66 2e66 696e 6443  ved = self.findC
+000223e0: 7572 7265 6e74 5361 7665 6456 616c 7565  urrentSavedValue
+000223f0: 2873 6372 6565 6e44 6963 742c 2073 6176  (screenDict, sav
+00022400: 6544 6963 742c 2022 5061 7474 6572 6e22  eDict, "Pattern"
+00022410: 290d 0a20 2020 2020 2020 2069 6620 504b  )..        if PK
+00022420: 4461 7465 5574 696c 6974 6965 732e 6973  DateUtilities.is
+00022430: 5472 6164 696e 6754 696d 6528 293a 0d0a  TradingTime():..
+00022440: 2020 2020 2020 2020 2020 2020 7261 6e67              rang
+00022450: 6544 6174 6120 3d20 6461 7461 2e68 6561  eData = data.hea
+00022460: 6428 6e72 202b 2031 295b 313a 5d0d 0a20  d(nr + 1)[1:].. 
+00022470: 2020 2020 2020 2020 2020 206e 6f77 5f63             now_c
+00022480: 616e 646c 6520 3d20 6461 7461 2e68 6561  andle = data.hea
+00022490: 6428 3129 0d0a 2020 2020 2020 2020 2020  d(1)..          
+000224a0: 2020 7261 6e67 6544 6174 615b 2252 616e    rangeData["Ran
+000224b0: 6765 225d 203d 2061 6273 2872 616e 6765  ge"] = abs(range
+000224c0: 4461 7461 5b22 436c 6f73 6522 5d20 2d20  Data["Close"] - 
+000224d0: 7261 6e67 6544 6174 615b 224f 7065 6e22  rangeData["Open"
+000224e0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+000224f0: 7265 6365 6e74 203d 2072 616e 6765 4461  recent = rangeDa
+00022500: 7461 2e68 6561 6428 3129 0d0a 2020 2020  ta.head(1)..    
+00022510: 2020 2020 2020 2020 6966 2028 0d0a 2020          if (..  
+00022520: 2020 2020 2020 2020 2020 2020 2020 6c65                le
+00022530: 6e28 7265 6365 6e74 2920 3d3d 2031 0d0a  n(recent) == 1..
+00022540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022550: 616e 6420 7265 6365 6e74 5b22 5261 6e67  and recent["Rang
+00022560: 6522 5d2e 696c 6f63 5b30 5d20 3d3d 2072  e"].iloc[0] == r
+00022570: 616e 6765 4461 7461 2e64 6573 6372 6962  angeData.describ
+00022580: 6528 295b 2252 616e 6765 225d 5b22 6d69  e()["Range"]["mi
+00022590: 6e22 5d0d 0a20 2020 2020 2020 2020 2020  n"]..           
+000225a0: 2029 3a0d 0a20 2020 2020 2020 2020 2020   ):..           
+000225b0: 2020 2020 2069 6620 280d 0a20 2020 2020       if (..     
+000225c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000225d0: 656c 662e 6765 7443 616e 646c 6554 7970  elf.getCandleTyp
+000225e0: 6528 7265 6365 6e74 290d 0a20 2020 2020  e(recent)..     
+000225f0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00022600: 6e64 206e 6f77 5f63 616e 646c 655b 2243  nd now_candle["C
+00022610: 6c6f 7365 225d 2e69 6c6f 635b 305d 203e  lose"].iloc[0] >
+00022620: 3d20 7265 6365 6e74 5b22 436c 6f73 6522  = recent["Close"
+00022630: 5d2e 696c 6f63 5b30 5d0d 0a20 2020 2020  ].iloc[0]..     
+00022640: 2020 2020 2020 2020 2020 2029 3a0d 0a20             ):.. 
+00022650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022660: 2020 2073 6372 6565 6e44 6963 745b 2250     screenDict["P
+00022670: 6174 7465 726e 225d 203d 2028 0d0a 2020  attern"] = (..  
+00022680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022690: 2020 2020 2020 7361 7665 645b 305d 202b        saved[0] +
+000226a0: 2063 6f6c 6f72 5465 7874 2e42 4f4c 4420   colorText.BOLD 
+000226b0: 2b20 636f 6c6f 7254 6578 742e 4752 4545  + colorText.GREE
+000226c0: 4e20 2b20 6622 4275 792d 4e52 7b6e 727d  N + f"Buy-NR{nr}
+000226d0: 2220 2b20 636f 6c6f 7254 6578 742e 454e  " + colorText.EN
+000226e0: 440d 0a20 2020 2020 2020 2020 2020 2020  D..             
+000226f0: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+00022700: 2020 2020 2020 2020 2020 2020 2020 7361                sa
+00022710: 7665 4469 6374 5b22 5061 7474 6572 6e22  veDict["Pattern"
+00022720: 5d20 3d20 7361 7665 645b 315d 202b 2066  ] = saved[1] + f
+00022730: 2242 7579 2d4e 527b 6e72 7d22 0d0a 2020  "Buy-NR{nr}"..  
+00022740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022750: 2020 7265 7475 726e 2054 7275 650d 0a20    return True.. 
+00022760: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00022770: 6c69 6620 280d 0a20 2020 2020 2020 2020  lif (..         
+00022780: 2020 2020 2020 2020 2020 206e 6f74 2073             not s
+00022790: 656c 662e 6765 7443 616e 646c 6554 7970  elf.getCandleTyp
+000227a0: 6528 7265 6365 6e74 290d 0a20 2020 2020  e(recent)..     
+000227b0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+000227c0: 6e64 206e 6f77 5f63 616e 646c 655b 2243  nd now_candle["C
+000227d0: 6c6f 7365 225d 2e69 6c6f 635b 305d 203c  lose"].iloc[0] <
+000227e0: 3d20 7265 6365 6e74 5b22 436c 6f73 6522  = recent["Close"
+000227f0: 5d2e 696c 6f63 5b30 5d0d 0a20 2020 2020  ].iloc[0]..     
+00022800: 2020 2020 2020 2020 2020 2029 3a0d 0a20             ):.. 
+00022810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022820: 2020 2073 6372 6565 6e44 6963 745b 2250     screenDict["P
+00022830: 6174 7465 726e 225d 203d 2028 0d0a 2020  attern"] = (..  
+00022840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022850: 2020 2020 2020 7361 7665 645b 305d 202b        saved[0] +
+00022860: 2063 6f6c 6f72 5465 7874 2e42 4f4c 4420   colorText.BOLD 
+00022870: 2b20 636f 6c6f 7254 6578 742e 4641 494c  + colorText.FAIL
+00022880: 202b 2066 2253 656c 6c2d 4e52 7b6e 727d   + f"Sell-NR{nr}
+00022890: 2220 2b20 636f 6c6f 7254 6578 742e 454e  " + colorText.EN
+000228a0: 440d 0a20 2020 2020 2020 2020 2020 2020  D..             
+000228b0: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+000228c0: 2020 2020 2020 2020 2020 2020 2020 7361                sa
+000228d0: 7665 4469 6374 5b22 5061 7474 6572 6e22  veDict["Pattern"
+000228e0: 5d20 3d20 7361 7665 645b 315d 202b 2066  ] = saved[1] + f
+000228f0: 2253 656c 6c2d 4e52 7b6e 727d 220d 0a20  "Sell-NR{nr}".. 
+00022900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022910: 2020 2072 6574 7572 6e20 5472 7565 0d0a     return True..
+00022920: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00022930: 726e 2046 616c 7365 0d0a 2020 2020 2020  rn False..      
+00022940: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+00022950: 2020 2020 2072 616e 6765 4461 7461 203d       rangeData =
+00022960: 2064 6174 612e 6865 6164 286e 7229 0d0a   data.head(nr)..
+00022970: 2020 2020 2020 2020 2020 2020 7261 6e67              rang
+00022980: 6544 6174 612e 6c6f 635b 3a2c 2752 616e  eData.loc[:,'Ran
+00022990: 6765 275d 203d 2061 6273 2872 616e 6765  ge'] = abs(range
+000229a0: 4461 7461 5b22 436c 6f73 6522 5d20 2d20  Data["Close"] - 
+000229b0: 7261 6e67 6544 6174 615b 224f 7065 6e22  rangeData["Open"
+000229c0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+000229d0: 7265 6365 6e74 203d 2072 616e 6765 4461  recent = rangeDa
+000229e0: 7461 2e68 6561 6428 3129 0d0a 2020 2020  ta.head(1)..    
+000229f0: 2020 2020 2020 2020 6966 2072 6563 656e          if recen
+00022a00: 745b 2252 616e 6765 225d 2e69 6c6f 635b  t["Range"].iloc[
+00022a10: 305d 203d 3d20 7261 6e67 6544 6174 612e  0] == rangeData.
+00022a20: 6465 7363 7269 6265 2829 5b22 5261 6e67  describe()["Rang
+00022a30: 6522 5d5b 226d 696e 225d 3a0d 0a20 2020  e"]["min"]:..   
+00022a40: 2020 2020 2020 2020 2020 2020 2073 6372               scr
+00022a50: 6565 6e44 6963 745b 2250 6174 7465 726e  eenDict["Pattern
+00022a60: 225d 203d 2028 0d0a 2020 2020 2020 2020  "] = (..        
+00022a70: 2020 2020 2020 2020 2020 2020 7361 7665              save
+00022a80: 645b 305d 202b 2063 6f6c 6f72 5465 7874  d[0] + colorText
+00022a90: 2e42 4f4c 4420 2b20 636f 6c6f 7254 6578  .BOLD + colorTex
+00022aa0: 742e 4752 4545 4e20 2b20 6622 4e52 7b6e  t.GREEN + f"NR{n
+00022ab0: 727d 2220 2b20 636f 6c6f 7254 6578 742e  r}" + colorText.
+00022ac0: 454e 440d 0a20 2020 2020 2020 2020 2020  END..           
+00022ad0: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+00022ae0: 2020 2020 2020 2020 7361 7665 4469 6374          saveDict
+00022af0: 5b22 5061 7474 6572 6e22 5d20 3d20 7361  ["Pattern"] = sa
+00022b00: 7665 645b 315d 202b 2066 224e 527b 6e72  ved[1] + f"NR{nr
+00022b10: 7d22 0d0a 2020 2020 2020 2020 2020 2020  }"..            
+00022b20: 2020 2020 7265 7475 726e 2054 7275 650d      return True.
+00022b30: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00022b40: 7572 6e20 4661 6c73 650d 0a0d 0a20 2020  urn False....   
+00022b50: 2023 2046 696e 6420 6966 2073 746f 636b   # Find if stock
+00022b60: 2069 7320 6e65 776c 7920 6c69 7374 6564   is newly listed
+00022b70: 0d0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
+00022b80: 7465 4e65 776c 794c 6973 7465 6428 7365  teNewlyListed(se
+00022b90: 6c66 2c20 6466 2c20 6461 7973 546f 4c6f  lf, df, daysToLo
+00022ba0: 6f6b 6261 636b 293a 0d0a 2020 2020 2020  okback):..      
+00022bb0: 2020 6966 2064 6620 6973 204e 6f6e 6520    if df is None 
+00022bc0: 6f72 206c 656e 2864 6629 203d 3d20 303a  or len(df) == 0:
+00022bd0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00022be0: 7475 726e 2046 616c 7365 0d0a 2020 2020  turn False..    
+00022bf0: 2020 2020 6461 7461 203d 2064 662e 636f      data = df.co
+00022c00: 7079 2829 0d0a 2020 2020 2020 2020 6461  py()..        da
+00022c10: 7973 546f 4c6f 6f6b 6261 636b 203d 2069  ysToLookback = i
+00022c20: 6e74 2864 6179 7354 6f4c 6f6f 6b62 6163  nt(daysToLookbac
+00022c30: 6b5b 3a2d 315d 290d 0a20 2020 2020 2020  k[:-1])..       
+00022c40: 2072 6563 656e 7420 3d20 6461 7461 2e68   recent = data.h
+00022c50: 6561 6428 3129 0d0a 2020 2020 2020 2020  ead(1)..        
+00022c60: 6966 206c 656e 2872 6563 656e 7429 203c  if len(recent) <
+00022c70: 2031 3a0d 0a20 2020 2020 2020 2020 2020   1:..           
+00022c80: 2072 6574 7572 6e20 4661 6c73 650d 0a20   return False.. 
+00022c90: 2020 2020 2020 2069 6620 6c65 6e28 6461         if len(da
+00022ca0: 7461 2920 3c20 6461 7973 546f 4c6f 6f6b  ta) < daysToLook
+00022cb0: 6261 636b 2061 6e64 2028 0d0a 2020 2020  back and (..    
+00022cc0: 2020 2020 2020 2020 7265 6365 6e74 5b22          recent["
+00022cd0: 436c 6f73 6522 5d2e 696c 6f63 5b30 5d20  Close"].iloc[0] 
+00022ce0: 213d 206e 702e 6e61 6e20 616e 6420 7265  != np.nan and re
+00022cf0: 6365 6e74 5b22 436c 6f73 6522 5d2e 696c  cent["Close"].il
+00022d00: 6f63 5b30 5d20 3e20 300d 0a20 2020 2020  oc[0] > 0..     
+00022d10: 2020 2029 3a0d 0a20 2020 2020 2020 2020     ):..         
+00022d20: 2020 2072 6574 7572 6e20 5472 7565 0d0a     return True..
+00022d30: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+00022d40: 616c 7365 0d0a 0d0a 2020 2020 2320 5661  alse....    # Va
+00022d50: 6c69 6461 7465 2069 6620 7468 6520 7374  lidate if the st
+00022d60: 6f63 6b20 7072 6963 6573 2061 7265 2061  ock prices are a
+00022d70: 7420 6c65 6173 7420 7269 7369 6e67 2062  t least rising b
+00022d80: 7920 3225 2066 6f72 2074 6865 206c 6173  y 2% for the las
+00022d90: 7420 3320 7365 7373 696f 6e73 0d0a 2020  t 3 sessions..  
+00022da0: 2020 6465 6620 7661 6c69 6461 7465 5072    def validatePr
+00022db0: 6963 6552 6973 696e 6742 7941 744c 6561  iceRisingByAtLea
+00022dc0: 7374 3250 6572 6365 6e74 2873 656c 662c  st2Percent(self,
+00022dd0: 2064 662c 2073 6372 6565 6e44 6963 742c   df, screenDict,
+00022de0: 2073 6176 6544 6963 7429 3a0d 0a20 2020   saveDict):..   
+00022df0: 2020 2020 2069 6620 6466 2069 7320 4e6f       if df is No
+00022e00: 6e65 206f 7220 6c65 6e28 6466 2920 3d3d  ne or len(df) ==
+00022e10: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
+00022e20: 2072 6574 7572 6e20 4661 6c73 650d 0a20   return False.. 
+00022e30: 2020 2020 2020 2064 6174 6120 3d20 6466         data = df
+00022e40: 2e63 6f70 7928 290d 0a20 2020 2020 2020  .copy()..       
+00022e50: 2064 6174 6120 3d20 6461 7461 2e66 696c   data = data.fil
+00022e60: 6c6e 6128 3029 0d0a 2020 2020 2020 2020  lna(0)..        
+00022e70: 6461 7461 203d 2064 6174 612e 7265 706c  data = data.repl
+00022e80: 6163 6528 5b6e 702e 696e 662c 202d 6e70  ace([np.inf, -np
+00022e90: 2e69 6e66 5d2c 2030 290d 0a20 2020 2020  .inf], 0)..     
+00022ea0: 2020 2064 6174 6120 3d20 6461 7461 2e68     data = data.h
+00022eb0: 6561 6428 3429 0d0a 2020 2020 2020 2020  ead(4)..        
+00022ec0: 6966 206c 656e 2864 6174 6129 203c 2034  if len(data) < 4
+00022ed0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+00022ee0: 6574 7572 6e20 4661 6c73 650d 0a20 2020  eturn False..   
+00022ef0: 2020 2020 2064 6179 3020 3d20 6461 7461       day0 = data
+00022f00: 2e69 6c6f 635b 305d 5b22 436c 6f73 6522  .iloc[0]["Close"
+00022f10: 5d2e 6974 656d 2829 0d0a 2020 2020 2020  ].item()..      
+00022f20: 2020 6461 794d 696e 7573 3120 3d20 6461    dayMinus1 = da
+00022f30: 7461 2e69 6c6f 635b 315d 5b22 436c 6f73  ta.iloc[1]["Clos
+00022f40: 6522 5d2e 6974 656d 2829 0d0a 2020 2020  e"].item()..    
+00022f50: 2020 2020 6461 794d 696e 7573 3220 3d20      dayMinus2 = 
+00022f60: 6461 7461 2e69 6c6f 635b 325d 5b22 436c  data.iloc[2]["Cl
+00022f70: 6f73 6522 5d2e 6974 656d 2829 0d0a 2020  ose"].item()..  
+00022f80: 2020 2020 2020 6461 794d 696e 7573 3320        dayMinus3 
+00022f90: 3d20 6461 7461 2e69 6c6f 635b 335d 5b22  = data.iloc[3]["
+00022fa0: 436c 6f73 6522 5d2e 6974 656d 2829 0d0a  Close"].item()..
+00022fb0: 2020 2020 2020 2020 7065 7263 656e 7433          percent3
+00022fc0: 203d 2072 6f75 6e64 2828 6461 794d 696e   = round((dayMin
+00022fd0: 7573 3220 2d20 6461 794d 696e 7573 3329  us2 - dayMinus3)
+00022fe0: 202a 2031 3030 202f 2064 6179 4d69 6e75   * 100 / dayMinu
+00022ff0: 7333 2c20 3229 0d0a 2020 2020 2020 2020  s3, 2)..        
+00023000: 7065 7263 656e 7432 203d 2072 6f75 6e64  percent2 = round
+00023010: 2828 6461 794d 696e 7573 3120 2d20 6461  ((dayMinus1 - da
+00023020: 794d 696e 7573 3229 202a 2031 3030 202f  yMinus2) * 100 /
+00023030: 2064 6179 4d69 6e75 7332 2c20 3229 0d0a   dayMinus2, 2)..
+00023040: 2020 2020 2020 2020 7065 7263 656e 7431          percent1
+00023050: 203d 2072 6f75 6e64 2828 6461 7930 202d   = round((day0 -
+00023060: 2064 6179 4d69 6e75 7331 2920 2a20 3130   dayMinus1) * 10
+00023070: 3020 2f20 6461 794d 696e 7573 312c 2032  0 / dayMinus1, 2
+00023080: 290d 0a0d 0a20 2020 2020 2020 2069 6620  )....        if 
+00023090: 7065 7263 656e 7431 203e 3d20 3220 616e  percent1 >= 2 an
+000230a0: 6420 7065 7263 656e 7432 203e 3d20 3220  d percent2 >= 2 
+000230b0: 616e 6420 7065 7263 656e 7433 203e 3d20  and percent3 >= 
+000230c0: 323a 0d0a 2020 2020 2020 2020 2020 2020  2:..            
+000230d0: 7063 745f 6368 616e 6765 5f74 6578 7420  pct_change_text 
+000230e0: 3d20 280d 0a20 2020 2020 2020 2020 2020  = (..           
+000230f0: 2020 2020 2028 2225 2e31 6625 2522 2025       ("%.1f%%" %
+00023100: 2070 6572 6365 6e74 3129 0d0a 2020 2020   percent1)..    
+00023110: 2020 2020 2020 2020 2020 2020 2b20 2822              + ("
+00023120: 2028 252e 3166 2525 2c22 2025 2070 6572   (%.1f%%," % per
+00023130: 6365 6e74 3229 0d0a 2020 2020 2020 2020  cent2)..        
+00023140: 2020 2020 2020 2020 2b20 2822 2025 2e31          + (" %.1
+00023150: 6625 2529 2220 2520 7065 7263 656e 7433  f%%)" % percent3
+00023160: 290d 0a20 2020 2020 2020 2020 2020 2029  )..            )
+00023170: 0d0a 2020 2020 2020 2020 2020 2020 7361  ..            sa
+00023180: 7665 4469 6374 5b22 2543 686e 6722 5d20  veDict["%Chng"] 
+00023190: 3d20 7063 745f 6368 616e 6765 5f74 6578  = pct_change_tex
+000231a0: 740d 0a20 2020 2020 2020 2020 2020 2073  t..            s
+000231b0: 6372 6565 6e44 6963 745b 2225 4368 6e67  creenDict["%Chng
+000231c0: 225d 203d 2063 6f6c 6f72 5465 7874 2e47  "] = colorText.G
+000231d0: 5245 454e 202b 2070 6374 5f63 6861 6e67  REEN + pct_chang
+000231e0: 655f 7465 7874 202b 2063 6f6c 6f72 5465  e_text + colorTe
+000231f0: 7874 2e45 4e44 0d0a 2020 2020 2020 2020  xt.END..        
+00023200: 2020 2020 7265 7475 726e 2054 7275 6520      return True 
+00023210: 616e 6420 7365 6c66 2e67 6574 4361 6e64  and self.getCand
+00023220: 6c65 5479 7065 2864 6174 612e 6865 6164  leType(data.head
+00023230: 2831 2929 0d0a 2020 2020 2020 2020 7265  (1))..        re
+00023240: 7475 726e 2046 616c 7365 0d0a 0d0a 2020  turn False....  
+00023250: 2020 2340 6d65 6173 7572 655f 7469 6d65    #@measure_time
+00023260: 0d0a 2020 2020 2320 7661 6c69 6461 7465  ..    # validate
+00023270: 2069 6620 5253 4920 6973 2077 6974 6869   if RSI is withi
+00023280: 6e20 6769 7665 6e20 7261 6e67 650d 0a20  n given range.. 
+00023290: 2020 2064 6566 2076 616c 6964 6174 6552     def validateR
+000232a0: 5349 2873 656c 662c 2064 662c 2073 6372  SI(self, df, scr
+000232b0: 6565 6e44 6963 742c 2073 6176 6544 6963  eenDict, saveDic
+000232c0: 742c 206d 696e 5253 492c 206d 6178 5253  t, minRSI, maxRS
+000232d0: 492c 7273 694b 6579 3d22 5253 4922 293a  I,rsiKey="RSI"):
+000232e0: 0d0a 2020 2020 2020 2020 6966 2064 6620  ..        if df 
+000232f0: 6973 204e 6f6e 6520 6f72 206c 656e 2864  is None or len(d
+00023300: 6629 203d 3d20 303a 0d0a 2020 2020 2020  f) == 0:..      
+00023310: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+00023320: 7365 0d0a 2020 2020 2020 2020 6966 2072  se..        if r
+00023330: 7369 4b65 7920 6e6f 7420 696e 2064 662e  siKey not in df.
+00023340: 636f 6c75 6d6e 733a 0d0a 2020 2020 2020  columns:..      
+00023350: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+00023360: 7365 0d0a 2020 2020 2020 2020 6461 7461  se..        data
+00023370: 203d 2064 662e 636f 7079 2829 0d0a 2020   = df.copy()..  
+00023380: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
+00023390: 612e 6669 6c6c 6e61 2830 290d 0a20 2020  a.fillna(0)..   
+000233a0: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
+000233b0: 2e72 6570 6c61 6365 285b 6e70 2e69 6e66  .replace([np.inf
+000233c0: 2c20 2d6e 702e 696e 665d 2c20 3029 0d0a  , -np.inf], 0)..
+000233d0: 2020 2020 2020 2020 7273 6920 3d20 696e          rsi = in
+000233e0: 7428 6461 7461 2e68 6561 6428 3129 5b72  t(data.head(1)[r
+000233f0: 7369 4b65 795d 2e69 6c6f 635b 305d 290d  siKey].iloc[0]).
+00023400: 0a20 2020 2020 2020 2073 6176 6544 6963  .        saveDic
+00023410: 745b 7273 694b 6579 5d20 3d20 7273 690d  t[rsiKey] = rsi.
+00023420: 0a20 2020 2020 2020 2023 2068 7474 7073  .        # https
+00023430: 3a2f 2f63 6861 7274 696e 6b2e 636f 6d2f  ://chartink.com/
+00023440: 7363 7265 656e 6572 2f72 7369 2d73 6372  screener/rsi-scr
+00023450: 6565 6e69 6e67 0d0a 2020 2020 2020 2020  eening..        
+00023460: 6966 2072 7369 3e20 3020 616e 6420 7273  if rsi> 0 and rs
+00023470: 6920 3e3d 206d 696e 5253 4920 616e 6420  i >= minRSI and 
+00023480: 7273 6920 3c3d 206d 6178 5253 493a 2020  rsi <= maxRSI:  
+00023490: 2320 6f72 2028 7273 6920 3c3d 2037 3120  # or (rsi <= 71 
+000234a0: 616e 6420 7273 6920 3e3d 2036 3729 3a0d  and rsi >= 67):.
+000234b0: 0a20 2020 2020 2020 2020 2020 2073 6372  .            scr
+000234c0: 6565 6e44 6963 745b 7273 694b 6579 5d20  eenDict[rsiKey] 
+000234d0: 3d20 280d 0a20 2020 2020 2020 2020 2020  = (..           
+000234e0: 2020 2020 2063 6f6c 6f72 5465 7874 2e42       colorText.B
+000234f0: 4f4c 4420 2b20 636f 6c6f 7254 6578 742e  OLD + colorText.
+00023500: 4752 4545 4e20 2b20 7374 7228 7273 6929  GREEN + str(rsi)
+00023510: 202b 2063 6f6c 6f72 5465 7874 2e45 4e44   + colorText.END
+00023520: 0d0a 2020 2020 2020 2020 2020 2020 290d  ..            ).
+00023530: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00023540: 7572 6e20 5472 7565 2069 6620 2872 7369  urn True if (rsi
+00023550: 4b65 7920 3d3d 2022 5253 4969 2229 2065  Key == "RSIi") e
+00023560: 6c73 6520 2873 656c 662e 7661 6c69 6461  lse (self.valida
+00023570: 7465 5253 4928 6466 2c20 7363 7265 656e  teRSI(df, screen
+00023580: 4469 6374 2c20 7361 7665 4469 6374 2c20  Dict, saveDict, 
+00023590: 6d69 6e52 5349 2c20 6d61 7852 5349 2c72  minRSI, maxRSI,r
+000235a0: 7369 4b65 793d 2252 5349 6922 2920 6f72  siKey="RSIi") or
+000235b0: 2054 7275 6529 0d0a 2020 2020 2020 2020   True)..        
+000235c0: 7363 7265 656e 4469 6374 5b72 7369 4b65  screenDict[rsiKe
+000235d0: 795d 203d 2063 6f6c 6f72 5465 7874 2e42  y] = colorText.B
+000235e0: 4f4c 4420 2b20 636f 6c6f 7254 6578 742e  OLD + colorText.
+000235f0: 4641 494c 202b 2073 7472 2872 7369 2920  FAIL + str(rsi) 
+00023600: 2b20 636f 6c6f 7254 6578 742e 454e 440d  + colorText.END.
+00023610: 0a20 2020 2020 2020 2023 2049 6620 6569  .        # If ei
+00023620: 7468 6572 2064 6169 6c79 206f 7220 696e  ther daily or in
+00023630: 7472 6164 6179 2052 5349 2063 6f6d 6573  traday RSI comes
+00023640: 2077 6974 6869 6e20 7261 6e67 653f 0d0a   within range?..
+00023650: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+00023660: 616c 7365 2069 6620 2872 7369 4b65 7920  alse if (rsiKey 
+00023670: 3d3d 2022 5253 4969 2229 2065 6c73 6520  == "RSIi") else 
+00023680: 2873 656c 662e 7661 6c69 6461 7465 5253  (self.validateRS
+00023690: 4928 6466 2c20 7363 7265 656e 4469 6374  I(df, screenDict
+000236a0: 2c20 7361 7665 4469 6374 2c20 6d69 6e52  , saveDict, minR
+000236b0: 5349 2c20 6d61 7852 5349 2c72 7369 4b65  SI, maxRSI,rsiKe
+000236c0: 793d 2252 5349 6922 2929 0d0a 0d0a 2020  y="RSIi"))....  
+000236d0: 2020 2320 5661 6c69 6461 7465 2069 6620    # Validate if 
+000236e0: 7468 6520 7374 6f63 6b20 6973 2062 756c  the stock is bul
+000236f0: 6c69 7368 2069 6e20 7468 6520 7368 6f72  lish in the shor
+00023700: 7420 7465 726d 0d0a 2020 2020 6465 6620  t term..    def 
+00023710: 7661 6c69 6461 7465 5368 6f72 7454 6572  validateShortTer
+00023720: 6d42 756c 6c69 7368 2873 656c 662c 2064  mBullish(self, d
+00023730: 662c 2073 6372 6565 6e44 6963 742c 2073  f, screenDict, s
+00023740: 6176 6544 6963 7429 3a0d 0a20 2020 2020  aveDict):..     
+00023750: 2020 2069 6620 6466 2069 7320 4e6f 6e65     if df is None
+00023760: 206f 7220 6c65 6e28 6466 2920 3d3d 2030   or len(df) == 0
+00023770: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+00023780: 6574 7572 6e20 4661 6c73 650d 0a20 2020  eturn False..   
+00023790: 2020 2020 2064 6174 6120 3d20 6466 2e63       data = df.c
+000237a0: 6f70 7928 290d 0a20 2020 2020 2020 2023  opy()..        #
+000237b0: 2068 7474 7073 3a2f 2f63 6861 7274 696e   https://chartin
+000237c0: 6b2e 636f 6d2f 7363 7265 656e 6572 2f73  k.com/screener/s
+000237d0: 686f 7274 2d74 6572 6d2d 6275 6c6c 6973  hort-term-bullis
+000237e0: 680d 0a20 2020 2020 2020 2064 6174 6120  h..        data 
+000237f0: 3d20 6461 7461 2e66 696c 6c6e 6128 3029  = data.fillna(0)
+00023800: 0d0a 2020 2020 2020 2020 6461 7461 203d  ..        data =
+00023810: 2064 6174 612e 7265 706c 6163 6528 5b6e   data.replace([n
+00023820: 702e 696e 662c 202d 6e70 2e69 6e66 5d2c  p.inf, -np.inf],
+00023830: 2030 290d 0a20 2020 2020 2020 2072 6563   0)..        rec
+00023840: 656e 7420 3d20 6461 7461 2e68 6561 6428  ent = data.head(
+00023850: 3129 0d0a 2020 2020 2020 2020 666b 203d  1)..        fk =
+00023860: 2030 2069 6620 6c65 6e28 6461 7461 2920   0 if len(data) 
+00023870: 3c20 3320 656c 7365 206e 702e 726f 756e  < 3 else np.roun
+00023880: 6428 6461 7461 5b22 4641 5354 4b22 5d2e  d(data["FASTK"].
+00023890: 696c 6f63 5b32 5d2c 2035 290d 0a20 2020  iloc[2], 5)..   
+000238a0: 2020 2020 2023 2052 6576 6572 7365 2074       # Reverse t
+000238b0: 6865 2064 6174 6166 7261 6d65 2066 6f72  he dataframe for
+000238c0: 2069 6368 696d 6f6b 7520 6361 6c63 756c   ichimoku calcul
+000238d0: 6174 696f 6e73 2077 6974 6820 6461 7465  ations with date
+000238e0: 2069 6e20 6173 6365 6e64 696e 6720 6f72   in ascending or
+000238f0: 6465 720d 0a20 2020 2020 2020 2064 665f  der..        df_
+00023900: 6e65 7720 3d20 6461 7461 5b3a 3a2d 315d  new = data[::-1]
+00023910: 0d0a 2020 2020 2020 2020 7472 793a 0d0a  ..        try:..
+00023920: 2020 2020 2020 2020 2020 2020 6466 5f69              df_i
+00023930: 6368 6920 3d20 6466 5f6e 6577 2e72 656e  chi = df_new.ren
+00023940: 616d 6528 0d0a 2020 2020 2020 2020 2020  ame(..          
+00023950: 2020 2020 2020 636f 6c75 6d6e 733d 7b0d        columns={.
+00023960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00023970: 2020 2020 2022 4f70 656e 223a 2022 6f70       "Open": "op
+00023980: 656e 222c 0d0a 2020 2020 2020 2020 2020  en",..          
+00023990: 2020 2020 2020 2020 2020 2248 6967 6822            "High"
+000239a0: 3a20 2268 6967 6822 2c0d 0a20 2020 2020  : "high",..     
+000239b0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000239c0: 4c6f 7722 3a20 226c 6f77 222c 0d0a 2020  Low": "low",..  
+000239d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000239e0: 2020 2243 6c6f 7365 223a 2022 636c 6f73    "Close": "clos
+000239f0: 6522 2c0d 0a20 2020 2020 2020 2020 2020  e",..           
+00023a00: 2020 2020 2020 2020 2022 566f 6c75 6d65           "Volume
+00023a10: 223a 2022 766f 6c75 6d65 222c 0d0a 2020  ": "volume",..  
+00023a20: 2020 2020 2020 2020 2020 2020 2020 7d0d                }.
+00023a30: 0a20 2020 2020 2020 2020 2020 2029 0d0a  .            )..
+00023a40: 2020 2020 2020 2020 2020 2020 6963 6869              ichi
+00023a50: 203d 2070 6b74 616c 6962 2e69 6368 696d   = pktalib.ichim
+00023a60: 6f6b 7528 6466 5f69 6368 692c 2039 2c20  oku(df_ichi, 9, 
+00023a70: 3236 2c20 3532 2c20 3236 290d 0a20 2020  26, 52, 26)..   
+00023a80: 2020 2020 2020 2020 2069 6620 6963 6869           if ichi
+00023a90: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
+00023aa0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00023ab0: 6e20 4661 6c73 650d 0a20 2020 2020 2020  n False..       
+00023ac0: 2020 2020 2064 665f 6e65 7720 3d20 7064       df_new = pd
+00023ad0: 2e63 6f6e 6361 7428 5b64 665f 6e65 772c  .concat([df_new,
+00023ae0: 2069 6368 695d 2c20 6178 6973 3d31 290d   ichi], axis=1).
+00023af0: 0a20 2020 2020 2020 2020 2020 2023 2052  .            # R
+00023b00: 6576 6572 7365 2061 6761 696e 2074 6f20  everse again to 
+00023b10: 6765 7420 7468 6520 6d6f 7374 2072 6563  get the most rec
+00023b20: 656e 7420 6461 7465 206f 6e20 746f 700d  ent date on top.
+00023b30: 0a20 2020 2020 2020 2020 2020 2064 665f  .            df_
+00023b40: 6e65 7720 3d20 6466 5f6e 6577 5b3a 3a2d  new = df_new[::-
+00023b50: 315d 0d0a 2020 2020 2020 2020 2020 2020  1]..            
+00023b60: 6466 5f6e 6577 203d 2064 665f 6e65 772e  df_new = df_new.
+00023b70: 6865 6164 2831 290d 0a20 2020 2020 2020  head(1)..       
+00023b80: 2020 2020 2064 665f 6e65 775b 2263 6c6f       df_new["clo
+00023b90: 7564 5f67 7265 656e 225d 203d 2064 665f  ud_green"] = df_
+00023ba0: 6e65 775b 2249 5341 5f39 225d 2e69 6c6f  new["ISA_9"].ilo
+00023bb0: 635b 305d 203e 2064 665f 6e65 775b 2249  c[0] > df_new["I
+00023bc0: 5342 5f32 3622 5d2e 696c 6f63 5b30 5d0d  SB_26"].iloc[0].
+00023bd0: 0a20 2020 2020 2020 2020 2020 2064 665f  .            df_
+00023be0: 6e65 775b 2263 6c6f 7564 5f72 6564 225d  new["cloud_red"]
+00023bf0: 203d 2064 665f 6e65 775b 2249 5342 5f32   = df_new["ISB_2
+00023c00: 3622 5d2e 696c 6f63 5b30 5d20 3e20 6466  6"].iloc[0] > df
+00023c10: 5f6e 6577 5b22 4953 415f 3922 5d2e 696c  _new["ISA_9"].il
+00023c20: 6f63 5b30 5d0d 0a20 2020 2020 2020 2065  oc[0]..        e
+00023c30: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
+00023c40: 6173 2065 3a20 2023 2070 7261 676d 613a  as e:  # pragma:
+00023c50: 206e 6f20 636f 7665 720d 0a20 2020 2020   no cover..     
+00023c60: 2020 2020 2020 2073 656c 662e 6465 6661         self.defa
+00023c70: 756c 745f 6c6f 6767 6572 2e64 6562 7567  ult_logger.debug
+00023c80: 2865 2c20 6578 635f 696e 666f 3d54 7275  (e, exc_info=Tru
+00023c90: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
+00023ca0: 7061 7373 0d0a 2020 2020 2020 2020 6162  pass..        ab
+00023cb0: 6f76 6543 6c6f 7564 546f 7020 3d20 4661  oveCloudTop = Fa
+00023cc0: 6c73 650d 0a20 2020 2020 2020 2023 2062  lse..        # b
+00023cd0: 6173 656c 696e 6520 3e20 636c 6f75 6420  aseline > cloud 
+00023ce0: 746f 7020 2863 6c6f 7564 2069 7320 626f  top (cloud is bo
+00023cf0: 756e 6420 6279 2073 7061 6e20 6120 616e  und by span a an
+00023d00: 6420 7370 616e 2062 2920 616e 6420 636c  d span b) and cl
+00023d10: 6f73 6520 6973 203e 2063 6c6f 7564 2074  ose is > cloud t
+00023d20: 6f70 0d0a 2020 2020 2020 2020 6966 2064  op..        if d
+00023d30: 665f 6e65 775b 2263 6c6f 7564 5f67 7265  f_new["cloud_gre
+00023d40: 656e 225d 2e69 6c6f 635b 305d 3a0d 0a20  en"].iloc[0]:.. 
+00023d50: 2020 2020 2020 2020 2020 2061 626f 7665             above
+00023d60: 436c 6f75 6454 6f70 203d 2028 0d0a 2020  CloudTop = (..  
+00023d70: 2020 2020 2020 2020 2020 2020 2020 6466                df
+00023d80: 5f6e 6577 5b22 494b 535f 3236 225d 2e69  _new["IKS_26"].i
+00023d90: 6c6f 635b 305d 203e 2064 665f 6e65 775b  loc[0] > df_new[
+00023da0: 2249 5341 5f39 225d 2e69 6c6f 635b 305d  "ISA_9"].iloc[0]
+00023db0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00023dc0: 2020 616e 6420 7265 6365 6e74 5b22 436c    and recent["Cl
+00023dd0: 6f73 6522 5d2e 696c 6f63 5b30 5d20 3e20  ose"].iloc[0] > 
+00023de0: 6466 5f6e 6577 5b22 4953 415f 3922 5d2e  df_new["ISA_9"].
+00023df0: 696c 6f63 5b30 5d0d 0a20 2020 2020 2020  iloc[0]..       
+00023e00: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+00023e10: 656c 6966 2064 665f 6e65 775b 2263 6c6f  elif df_new["clo
+00023e20: 7564 5f72 6564 225d 2e69 6c6f 635b 305d  ud_red"].iloc[0]
+00023e30: 3a0d 0a20 2020 2020 2020 2020 2020 2061  :..            a
+00023e40: 626f 7665 436c 6f75 6454 6f70 203d 2028  boveCloudTop = (
+00023e50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00023e60: 2020 6466 5f6e 6577 5b22 494b 535f 3236    df_new["IKS_26
+00023e70: 225d 2e69 6c6f 635b 305d 203e 2064 665f  "].iloc[0] > df_
+00023e80: 6e65 775b 2249 5342 5f32 3622 5d2e 696c  new["ISB_26"].il
+00023e90: 6f63 5b30 5d0d 0a20 2020 2020 2020 2020  oc[0]..         
+00023ea0: 2020 2020 2020 2061 6e64 2072 6563 656e         and recen
+00023eb0: 745b 2243 6c6f 7365 225d 2e69 6c6f 635b  t["Close"].iloc[
+00023ec0: 305d 203e 2064 665f 6e65 775b 2249 5342  0] > df_new["ISB
+00023ed0: 5f32 3622 5d2e 696c 6f63 5b30 5d0d 0a20  _26"].iloc[0].. 
+00023ee0: 2020 2020 2020 2020 2020 2029 0d0a 0d0a             )....
+00023ef0: 2020 2020 2020 2020 2320 4c61 7465 7374          # Latest
+00023f00: 2049 6368 696d 6f6b 7520 6261 7365 6c69   Ichimoku baseli
+00023f10: 6e65 2069 7320 3c20 6c61 7465 7374 2049  ne is < latest I
+00023f20: 6368 696d 6f6b 7520 636f 6e76 6572 7369  chimoku conversi
+00023f30: 6f6e 206c 696e 650d 0a20 2020 2020 2020  on line..       
+00023f40: 2069 6620 6162 6f76 6543 6c6f 7564 546f   if aboveCloudTo
+00023f50: 7020 616e 6420 6466 5f6e 6577 5b22 494b  p and df_new["IK
+00023f60: 535f 3236 225d 2e69 6c6f 635b 305d 203c  S_26"].iloc[0] <
+00023f70: 2064 665f 6e65 775b 2249 5453 5f39 225d   df_new["ITS_9"]
+00023f80: 2e69 6c6f 635b 305d 3a0d 0a20 2020 2020  .iloc[0]:..     
+00023f90: 2020 2020 2020 2023 2053 746f 6368 5253         # StochRS
+00023fa0: 4920 6372 6f73 7365 6420 3230 2061 6e64  I crossed 20 and
+00023fb0: 2052 5349 203e 2035 300d 0a20 2020 2020   RSI > 50..     
+00023fc0: 2020 2020 2020 2069 6620 666b 203e 2032         if fk > 2
+00023fd0: 3020 616e 6420 7265 6365 6e74 5b22 5253  0 and recent["RS
+00023fe0: 4922 5d2e 696c 6f63 5b30 5d20 3e20 3530  I"].iloc[0] > 50
+00023ff0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00024000: 2020 2023 2063 6f6e 6469 7469 6f6e 206f     # condition o
+00024010: 6620 6372 6f73 7369 6e67 2074 6865 2053  f crossing the S
+00024020: 746f 6368 5253 4920 6d61 696e 2073 6967  tochRSI main sig
+00024030: 6e61 6c20 6c69 6e65 2066 726f 6d20 626f  nal line from bo
+00024040: 7474 6f6d 2074 6f20 746f 700d 0a20 2020  ttom to top..   
+00024050: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00024060: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+00024070: 2020 2020 2020 2064 6174 615b 2246 4153         data["FAS
+00024080: 5444 225d 2e69 6c6f 635b 3130 305d 203c  TD"].iloc[100] <
+00024090: 2064 6174 615b 2246 4153 544b 225d 2e69   data["FASTK"].i
+000240a0: 6c6f 635b 3130 305d 0d0a 2020 2020 2020  loc[100]..      
+000240b0: 2020 2020 2020 2020 2020 2020 2020 616e                an
+000240c0: 6420 6461 7461 5b22 4641 5354 4422 5d2e  d data["FASTD"].
+000240d0: 696c 6f63 5b31 3031 5d20 3e20 6461 7461  iloc[101] > data
+000240e0: 5b22 4641 5354 4b22 5d2e 696c 6f63 5b31  ["FASTK"].iloc[1
+000240f0: 3031 5d0d 0a20 2020 2020 2020 2020 2020  01]..           
+00024100: 2020 2020 2029 3a0d 0a20 2020 2020 2020       ):..       
+00024110: 2020 2020 2020 2020 2020 2020 2023 2063               # c
+00024120: 6c6f 7365 203e 2035 3020 7065 7269 6f64  lose > 50 period
+00024130: 2053 4d41 2f45 4d41 2061 6e64 2032 3030   SMA/EMA and 200
+00024140: 2070 6572 696f 6420 534d 412f 454d 410d   period SMA/EMA.
+00024150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00024160: 2020 2020 2069 6620 280d 0a20 2020 2020       if (..     
+00024170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024180: 2020 2072 6563 656e 745b 2253 534d 4122     recent["SSMA"
+00024190: 5d2e 696c 6f63 5b30 5d20 3e20 7265 6365  ].iloc[0] > rece
+000241a0: 6e74 5b22 534d 4122 5d2e 696c 6f63 5b30  nt["SMA"].iloc[0
+000241b0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+000241c0: 2020 2020 2020 2020 2020 2061 6e64 2072             and r
+000241d0: 6563 656e 745b 2243 6c6f 7365 225d 2e69  ecent["Close"].i
+000241e0: 6c6f 635b 305d 203e 2072 6563 656e 745b  loc[0] > recent[
+000241f0: 2253 534d 4122 5d2e 696c 6f63 5b30 5d0d  "SSMA"].iloc[0].
+00024200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00024210: 2020 2020 2020 2020 2061 6e64 2072 6563           and rec
+00024220: 656e 745b 2243 6c6f 7365 225d 2e69 6c6f  ent["Close"].ilo
+00024230: 635b 305d 203e 2072 6563 656e 745b 224c  c[0] > recent["L
+00024240: 4d41 225d 2e69 6c6f 635b 305d 0d0a 2020  MA"].iloc[0]..  
+00024250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024260: 2020 293a 0d0a 2020 2020 2020 2020 2020    ):..          
+00024270: 2020 2020 2020 2020 2020 2020 2020 7361                sa
+00024280: 7665 6420 3d20 7365 6c66 2e66 696e 6443  ved = self.findC
+00024290: 7572 7265 6e74 5361 7665 6456 616c 7565  urrentSavedValue
+000242a0: 2873 6372 6565 6e44 6963 742c 7361 7665  (screenDict,save
+000242b0: 4469 6374 2c22 4d41 2d53 6967 6e61 6c22  Dict,"MA-Signal"
+000242c0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000242d0: 2020 2020 2020 2020 2020 2073 6372 6565             scree
+000242e0: 6e44 6963 745b 224d 412d 5369 676e 616c  nDict["MA-Signal
+000242f0: 225d 203d 2028 0d0a 2020 2020 2020 2020  "] = (..        
+00024300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024310: 2020 2020 7361 7665 645b 305d 202b 2063      saved[0] + c
+00024320: 6f6c 6f72 5465 7874 2e42 4f4c 4420 2b20  olorText.BOLD + 
+00024330: 636f 6c6f 7254 6578 742e 4752 4545 4e20  colorText.GREEN 
+00024340: 2b20 2242 756c 6c69 7368 2220 2b20 636f  + "Bullish" + co
+00024350: 6c6f 7254 6578 742e 454e 440d 0a20 2020  lorText.END..   
+00024360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024370: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+00024380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024390: 7361 7665 4469 6374 5b22 4d41 2d53 6967  saveDict["MA-Sig
+000243a0: 6e61 6c22 5d20 3d20 7361 7665 645b 315d  nal"] = saved[1]
+000243b0: 202b 2022 4275 6c6c 6973 6822 0d0a 2020   + "Bullish"..  
+000243c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000243d0: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
+000243e0: 650d 0a20 2020 2020 2020 2072 6574 7572  e..        retur
+000243f0: 6e20 4661 6c73 650d 0a0d 0a20 2020 2023  n False....    #
+00024400: 2056 616c 6964 6174 6520 5650 430d 0a20   Validate VPC.. 
+00024410: 2020 2064 6566 2076 616c 6964 6174 6556     def validateV
+00024420: 4350 280d 0a20 2020 2020 2020 2073 656c  CP(..        sel
+00024430: 662c 2064 662c 2073 6372 6565 6e44 6963  f, df, screenDic
+00024440: 742c 2073 6176 6544 6963 742c 2073 746f  t, saveDict, sto
+00024450: 636b 4e61 6d65 3d4e 6f6e 652c 2077 696e  ckName=None, win
+00024460: 646f 773d 332c 2070 6572 6365 6e74 6167  dow=3, percentag
+00024470: 6546 726f 6d54 6f70 3d33 0d0a 2020 2020  eFromTop=3..    
+00024480: 293a 0d0a 2020 2020 2020 2020 6966 2064  ):..        if d
+00024490: 6620 6973 204e 6f6e 6520 6f72 206c 656e  f is None or len
+000244a0: 2864 6629 203d 3d20 303a 0d0a 2020 2020  (df) == 0:..    
+000244b0: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+000244c0: 616c 7365 0d0a 2020 2020 2020 2020 6461  alse..        da
+000244d0: 7461 203d 2064 662e 636f 7079 2829 0d0a  ta = df.copy()..
+000244e0: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
+000244f0: 2020 2020 2020 2020 2020 7065 7263 656e            percen
+00024500: 7461 6765 4672 6f6d 546f 7020 2f3d 2031  tageFromTop /= 1
+00024510: 3030 0d0a 2020 2020 2020 2020 2020 2020  00..            
+00024520: 6461 7461 2e72 6573 6574 5f69 6e64 6578  data.reset_index
+00024530: 2869 6e70 6c61 6365 3d54 7275 6529 0d0a  (inplace=True)..
+00024540: 2020 2020 2020 2020 2020 2020 6461 7461              data
+00024550: 2e72 656e 616d 6528 636f 6c75 6d6e 733d  .rename(columns=
+00024560: 7b22 696e 6465 7822 3a20 2244 6174 6522  {"index": "Date"
+00024570: 7d2c 2069 6e70 6c61 6365 3d54 7275 6529  }, inplace=True)
+00024580: 0d0a 2020 2020 2020 2020 2020 2020 6461  ..            da
+00024590: 7461 5b22 746f 7073 225d 203d 2028 0d0a  ta["tops"] = (..
+000245a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000245b0: 6461 7461 5b22 4869 6768 225d 0d0a 2020  data["High"]..  
+000245c0: 2020 2020 2020 2020 2020 2020 2020 2e69                .i
+000245d0: 6c6f 635b 0d0a 2020 2020 2020 2020 2020  loc[..          
+000245e0: 2020 2020 2020 2020 2020 6c69 7374 280d            list(.
+000245f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00024600: 2020 2020 2020 2020 2070 6b74 616c 6962           pktalib
+00024610: 2e61 7267 7265 6c65 7874 7265 6d61 280d  .argrelextrema(.
+00024620: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00024630: 2020 2020 2020 2020 2020 2020 206e 702e               np.
+00024640: 6172 7261 7928 6461 7461 5b22 4869 6768  array(data["High
+00024650: 225d 292c 206e 702e 6772 6561 7465 725f  "]), np.greater_
+00024660: 6571 7561 6c2c 206f 7264 6572 3d77 696e  equal, order=win
+00024670: 646f 770d 0a20 2020 2020 2020 2020 2020  dow..           
+00024680: 2020 2020 2020 2020 2020 2020 2029 5b30               )[0
+00024690: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+000246a0: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+000246b0: 2020 2020 2020 2020 2020 5d0d 0a20 2020            ]..   
+000246c0: 2020 2020 2020 2020 2020 2020 202e 6865               .he
+000246d0: 6164 2834 290d 0a20 2020 2020 2020 2020  ad(4)..         
+000246e0: 2020 2029 0d0a 2020 2020 2020 2020 2020     )..          
+000246f0: 2020 6461 7461 5b22 626f 7473 225d 203d    data["bots"] =
+00024700: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
+00024710: 2020 2020 6461 7461 5b22 4c6f 7722 5d0d      data["Low"].
+00024720: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00024730: 202e 696c 6f63 5b0d 0a20 2020 2020 2020   .iloc[..       
+00024740: 2020 2020 2020 2020 2020 2020 206c 6973               lis
+00024750: 7428 0d0a 2020 2020 2020 2020 2020 2020  t(..            
+00024760: 2020 2020 2020 2020 2020 2020 706b 7461              pkta
+00024770: 6c69 622e 6172 6772 656c 6578 7472 656d  lib.argrelextrem
+00024780: 6128 0d0a 2020 2020 2020 2020 2020 2020  a(..            
+00024790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000247a0: 6e70 2e61 7272 6179 2864 6174 615b 224c  np.array(data["L
+000247b0: 6f77 225d 292c 206e 702e 6c65 7373 5f65  ow"]), np.less_e
+000247c0: 7175 616c 2c20 6f72 6465 723d 7769 6e64  qual, order=wind
+000247d0: 6f77 0d0a 2020 2020 2020 2020 2020 2020  ow..            
+000247e0: 2020 2020 2020 2020 2020 2020 295b 305d              )[0]
+000247f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00024800: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+00024810: 2020 2020 2020 2020 205d 0d0a 2020 2020           ]..    
+00024820: 2020 2020 2020 2020 2020 2020 2e68 6561              .hea
+00024830: 6428 3429 0d0a 2020 2020 2020 2020 2020  d(4)..          
+00024840: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
+00024850: 2064 6174 6120 3d20 6461 7461 2e66 696c   data = data.fil
+00024860: 6c6e 6128 3029 0d0a 2020 2020 2020 2020  lna(0)..        
+00024870: 2020 2020 6461 7461 203d 2064 6174 612e      data = data.
+00024880: 7265 706c 6163 6528 5b6e 702e 696e 662c  replace([np.inf,
+00024890: 202d 6e70 2e69 6e66 5d2c 2030 290d 0a20   -np.inf], 0).. 
+000248a0: 2020 2020 2020 2020 2020 2074 6f70 7320             tops 
+000248b0: 3d20 6461 7461 5b64 6174 612e 746f 7073  = data[data.tops
+000248c0: 203e 2030 5d0d 0a20 2020 2020 2020 2020   > 0]..         
+000248d0: 2020 2023 2062 6f74 7320 3d20 6461 7461     # bots = data
+000248e0: 5b64 6174 612e 626f 7473 203e 2030 5d0d  [data.bots > 0].
+000248f0: 0a20 2020 2020 2020 2020 2020 2068 6967  .            hig
+00024900: 6865 7374 546f 7020 3d20 726f 756e 6428  hestTop = round(
+00024910: 746f 7073 2e64 6573 6372 6962 6528 295b  tops.describe()[
+00024920: 2248 6967 6822 5d5b 226d 6178 225d 2c20  "High"]["max"], 
+00024930: 3129 0d0a 2020 2020 2020 2020 2020 2020  1)..            
+00024940: 6669 6c74 6572 6564 546f 7073 203d 2074  filteredTops = t
+00024950: 6f70 735b 0d0a 2020 2020 2020 2020 2020  ops[..          
+00024960: 2020 2020 2020 746f 7073 2e74 6f70 7320        tops.tops 
+00024970: 3e20 2868 6967 6865 7374 546f 7020 2d20  > (highestTop - 
+00024980: 2868 6967 6865 7374 546f 7020 2a20 7065  (highestTop * pe
+00024990: 7263 656e 7461 6765 4672 6f6d 546f 7029  rcentageFromTop)
+000249a0: 290d 0a20 2020 2020 2020 2020 2020 205d  )..            ]
+000249b0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+000249c0: 2066 696c 7465 7265 6454 6f70 732e 6571   filteredTops.eq
+000249d0: 7561 6c73 2874 6f70 7329 3a20 2023 2054  uals(tops):  # T
+000249e0: 6f70 7320 6172 6520 696e 2074 6865 2072  ops are in the r
+000249f0: 616e 6765 0d0a 2020 2020 2020 2020 2020  ange..          
+00024a00: 2020 2020 2020 6c6f 7750 6f69 6e74 7320        lowPoints 
+00024a10: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00024a20: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
+00024a30: 616e 6765 286c 656e 2874 6f70 7329 202d  ange(len(tops) -
+00024a40: 2031 293a 0d0a 2020 2020 2020 2020 2020   1):..          
+00024a50: 2020 2020 2020 2020 2020 656e 6444 6174            endDat
+00024a60: 6520 3d20 746f 7073 2e69 6c6f 635b 695d  e = tops.iloc[i]
+00024a70: 5b22 4461 7465 225d 0d0a 2020 2020 2020  ["Date"]..      
+00024a80: 2020 2020 2020 2020 2020 2020 2020 7374                st
+00024a90: 6172 7444 6174 6520 3d20 746f 7073 2e69  artDate = tops.i
+00024aa0: 6c6f 635b 6920 2b20 315d 5b22 4461 7465  loc[i + 1]["Date
+00024ab0: 225d 0d0a 2020 2020 2020 2020 2020 2020  "]..            
+00024ac0: 2020 2020 2020 2020 6c6f 7750 6f69 6e74          lowPoint
+00024ad0: 732e 6170 7065 6e64 280d 0a20 2020 2020  s.append(..     
+00024ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024af0: 2020 2064 6174 615b 0d0a 2020 2020 2020     data[..      
 00024b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024b10: 2020 2020 2073 6176 6564 5b30 5d20 0d0a       saved[0] ..
-00024b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024b30: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
-00024b40: 6578 742e 424f 4c44 0d0a 2020 2020 2020  ext.BOLD..      
+00024b10: 2020 2020 2020 2864 6174 612e 4461 7465        (data.Date
+00024b20: 203e 3d20 7374 6172 7444 6174 6529 2026   >= startDate) &
+00024b30: 2028 6461 7461 2e44 6174 6520 3c3d 2065   (data.Date <= e
+00024b40: 6e64 4461 7465 290d 0a20 2020 2020 2020  ndDate)..       
 00024b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024b60: 2020 2b20 636f 6c6f 7254 6578 742e 4752    + colorText.GR
-00024b70: 4545 4e0d 0a20 2020 2020 2020 2020 2020  EEN..           
-00024b80: 2020 2020 2020 2020 2020 2020 202b 2066               + f
-00024b90: 2256 4350 2028 424f 3a20 7b68 6967 6865  "VCP (BO: {highe
-00024ba0: 7374 546f 707d 2922 0d0a 2020 2020 2020  stTop})"..      
-00024bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024bc0: 2020 2b20 636f 6c6f 7254 6578 742e 454e    + colorText.EN
-00024bd0: 440d 0a20 2020 2020 2020 2020 2020 2020  D..             
-00024be0: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-00024bf0: 2020 2020 2020 2020 2020 2020 2020 7361                sa
-00024c00: 7665 4469 6374 5b22 5061 7474 6572 6e22  veDict["Pattern"
-00024c10: 5d20 3d20 7361 7665 645b 315d 202b 2066  ] = saved[1] + f
-00024c20: 2256 4350 2028 424f 3a20 7b68 6967 6865  "VCP (BO: {highe
-00024c30: 7374 546f 707d 2922 0d0a 2020 2020 2020  stTop})"..      
-00024c40: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00024c50: 7475 726e 2054 7275 650d 0a20 2020 2020  turn True..     
-00024c60: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
-00024c70: 696f 6e20 6173 2065 3a20 2023 2070 7261  ion as e:  # pra
-00024c80: 676d 613a 206e 6f20 636f 7665 720d 0a20  gma: no cover.. 
-00024c90: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00024ca0: 6465 6661 756c 745f 6c6f 6767 6572 2e64  default_logger.d
-00024cb0: 6562 7567 2865 2c20 6578 635f 696e 666f  ebug(e, exc_info
-00024cc0: 3d54 7275 6529 0d0a 2020 2020 2020 2020  =True)..        
-00024cd0: 7265 7475 726e 2046 616c 7365 0d0a 0d0a  return False....
-00024ce0: 2020 2020 2320 5661 6c69 6461 7465 2069      # Validate i
-00024cf0: 6620 766f 6c75 6d65 206f 6620 6c61 7374  f volume of last
-00024d00: 2064 6179 2069 7320 6869 6768 6572 2074   day is higher t
-00024d10: 6861 6e20 6176 670d 0a20 2020 2064 6566  han avg..    def
-00024d20: 2076 616c 6964 6174 6556 6f6c 756d 6528   validateVolume(
-00024d30: 0d0a 2020 2020 2020 2020 7365 6c66 2c20  ..        self, 
-00024d40: 6466 2c20 7363 7265 656e 4469 6374 2c20  df, screenDict, 
-00024d50: 7361 7665 4469 6374 2c20 766f 6c75 6d65  saveDict, volume
-00024d60: 5261 7469 6f3d 322e 352c 206d 696e 566f  Ratio=2.5, minVo
-00024d70: 6c75 6d65 3d31 3030 0d0a 2020 2020 293a  lume=100..    ):
-00024d80: 0d0a 2020 2020 2020 2020 6966 2064 6620  ..        if df 
-00024d90: 6973 204e 6f6e 6520 6f72 206c 656e 2864  is None or len(d
-00024da0: 6629 203d 3d20 303a 0d0a 2020 2020 2020  f) == 0:..      
-00024db0: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-00024dc0: 7365 2c20 4661 6c73 650d 0a20 2020 2020  se, False..     
-00024dd0: 2020 2064 6174 6120 3d20 6466 2e63 6f70     data = df.cop
-00024de0: 7928 290d 0a20 2020 2020 2020 2064 6174  y()..        dat
-00024df0: 6120 3d20 6461 7461 2e66 696c 6c6e 6128  a = data.fillna(
-00024e00: 3029 0d0a 2020 2020 2020 2020 6461 7461  0)..        data
-00024e10: 203d 2064 6174 612e 7265 706c 6163 6528   = data.replace(
-00024e20: 5b6e 702e 696e 662c 202d 6e70 2e69 6e66  [np.inf, -np.inf
-00024e30: 5d2c 2030 290d 0a20 2020 2020 2020 2072  ], 0)..        r
-00024e40: 6563 656e 7420 3d20 6461 7461 2e68 6561  ecent = data.hea
-00024e50: 6428 3129 0d0a 2020 2020 2020 2020 2320  d(1)..        # 
-00024e60: 4569 7468 6572 2074 6865 2072 6f6c 6c69  Either the rolli
-00024e70: 6e67 2076 6f6c 756d 6520 6f66 2070 6173  ng volume of pas
-00024e80: 7420 3230 2073 6573 7369 6f6e 7320 6f72  t 20 sessions or
-00024e90: 2074 6f64 6179 2773 2076 6f6c 756d 6520   today's volume 
-00024ea0: 7368 6f75 6c64 2062 6520 3e20 6d69 6e20  should be > min 
-00024eb0: 766f 6c75 6d65 0d0a 2020 2020 2020 2020  volume..        
-00024ec0: 6861 734d 696e 696d 756d 566f 6c75 6d65  hasMinimumVolume
-00024ed0: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
-00024ee0: 2020 7265 6365 6e74 5b22 566f 6c4d 4122    recent["VolMA"
-00024ef0: 5d2e 696c 6f63 5b30 5d20 3e3d 206d 696e  ].iloc[0] >= min
-00024f00: 566f 6c75 6d65 0d0a 2020 2020 2020 2020  Volume..        
-00024f10: 2020 2020 6f72 2072 6563 656e 745b 2256      or recent["V
-00024f20: 6f6c 756d 6522 5d2e 696c 6f63 5b30 5d20  olume"].iloc[0] 
-00024f30: 3e3d 206d 696e 566f 6c75 6d65 0d0a 2020  >= minVolume..  
-00024f40: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-00024f50: 2069 6620 7265 6365 6e74 5b22 566f 6c4d   if recent["VolM
-00024f60: 4122 5d2e 696c 6f63 5b30 5d20 3d3d 2030  A"].iloc[0] == 0
-00024f70: 3a20 2023 2048 616e 646c 6573 2044 6976  :  # Handles Div
-00024f80: 6964 6520 6279 2030 2077 6172 6e69 6e67  ide by 0 warning
-00024f90: 0d0a 2020 2020 2020 2020 2020 2020 7361  ..            sa
-00024fa0: 7665 4469 6374 5b22 566f 6c75 6d65 225d  veDict["Volume"]
-00024fb0: 203d 2030 2020 2320 2255 6e6b 6e6f 776e   = 0  # "Unknown
-00024fc0: 220d 0a20 2020 2020 2020 2020 2020 2073  "..            s
-00024fd0: 6372 6565 6e44 6963 745b 2256 6f6c 756d  creenDict["Volum
-00024fe0: 6522 5d20 3d20 300d 0a20 2020 2020 2020  e"] = 0..       
-00024ff0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
-00025000: 652c 2068 6173 4d69 6e69 6d75 6d56 6f6c  e, hasMinimumVol
-00025010: 756d 650d 0a20 2020 2020 2020 2072 6174  ume..        rat
-00025020: 696f 203d 2072 6f75 6e64 2872 6563 656e  io = round(recen
-00025030: 745b 2256 6f6c 756d 6522 5d2e 696c 6f63  t["Volume"].iloc
-00025040: 5b30 5d20 2f20 7265 6365 6e74 5b22 566f  [0] / recent["Vo
-00025050: 6c4d 4122 5d2e 696c 6f63 5b30 5d2c 2032  lMA"].iloc[0], 2
-00025060: 290d 0a20 2020 2020 2020 2073 6176 6544  )..        saveD
-00025070: 6963 745b 2256 6f6c 756d 6522 5d20 3d20  ict["Volume"] = 
-00025080: 7261 7469 6f0d 0a20 2020 2020 2020 2069  ratio..        i
-00025090: 6620 7261 7469 6f20 3e3d 2076 6f6c 756d  f ratio >= volum
-000250a0: 6552 6174 696f 2061 6e64 2072 6174 696f  eRatio and ratio
-000250b0: 2021 3d20 6e70 2e6e 616e 2061 6e64 2028   != np.nan and (
-000250c0: 6e6f 7420 6d61 7468 2e69 7369 6e66 2872  not math.isinf(r
-000250d0: 6174 696f 2929 3a0d 0a20 2020 2020 2020  atio)):..       
-000250e0: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
-000250f0: 2256 6f6c 756d 6522 5d20 3d20 7261 7469  "Volume"] = rati
-00025100: 6f0d 0a20 2020 2020 2020 2020 2020 2072  o..            r
-00025110: 6574 7572 6e20 5472 7565 2c20 6861 734d  eturn True, hasM
-00025120: 696e 696d 756d 566f 6c75 6d65 0d0a 2020  inimumVolume..  
-00025130: 2020 2020 2020 7363 7265 656e 4469 6374        screenDict
-00025140: 5b22 566f 6c75 6d65 225d 203d 2072 6174  ["Volume"] = rat
-00025150: 696f 0d0a 2020 2020 2020 2020 7265 7475  io..        retu
-00025160: 726e 2046 616c 7365 2c20 6861 734d 696e  rn False, hasMin
-00025170: 696d 756d 566f 6c75 6d65 0d0a 0d0a 2020  imumVolume....  
-00025180: 2020 2320 4669 6e64 2069 6620 7374 6f63    # Find if stoc
-00025190: 6b20 6973 2076 616c 6964 6174 696e 6720  k is validating 
-000251a0: 766f 6c75 6d65 2073 7072 6561 6420 616e  volume spread an
-000251b0: 616c 7973 6973 0d0a 2020 2020 6465 6620  alysis..    def 
-000251c0: 7661 6c69 6461 7465 566f 6c75 6d65 5370  validateVolumeSp
-000251d0: 7265 6164 416e 616c 7973 6973 2873 656c  readAnalysis(sel
-000251e0: 662c 2064 662c 2073 6372 6565 6e44 6963  f, df, screenDic
-000251f0: 742c 2073 6176 6544 6963 7429 3a0d 0a20  t, saveDict):.. 
-00025200: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
-00025210: 2020 2020 2020 2020 2069 6620 6466 2069           if df i
-00025220: 7320 4e6f 6e65 206f 7220 6c65 6e28 6466  s None or len(df
-00025230: 2920 3d3d 2030 3a0d 0a20 2020 2020 2020  ) == 0:..       
-00025240: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00025250: 4661 6c73 650d 0a20 2020 2020 2020 2020  False..         
-00025260: 2020 2064 6174 6120 3d20 6466 2e63 6f70     data = df.cop
-00025270: 7928 290d 0a20 2020 2020 2020 2020 2020  y()..           
-00025280: 2064 6174 6120 3d20 6461 7461 2e68 6561   data = data.hea
-00025290: 6428 3229 0d0a 2020 2020 2020 2020 2020  d(2)..          
-000252a0: 2020 6966 206c 656e 2864 6174 6129 203c    if len(data) <
-000252b0: 2032 3a0d 0a20 2020 2020 2020 2020 2020   2:..           
-000252c0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
-000252d0: 650d 0a20 2020 2020 2020 2020 2020 2074  e..            t
-000252e0: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
-000252f0: 2020 2020 2023 2043 6865 636b 2066 6f72       # Check for
-00025300: 2070 7265 7669 6f75 7320 5245 4420 6361   previous RED ca
-00025310: 6e64 6c65 730d 0a20 2020 2020 2020 2020  ndles..         
-00025320: 2020 2020 2020 2023 2043 7572 7265 6e74         # Current
-00025330: 2063 616e 646c 6520 3d20 3074 682c 2050   candle = 0th, P
-00025340: 7265 7669 6f75 7320 4361 6e64 6c65 203d  revious Candle =
-00025350: 2031 7374 2066 6f72 2066 6f6c 6c6f 7769   1st for followi
-00025360: 6e67 206c 6f67 6963 0d0a 2020 2020 2020  ng logic..      
-00025370: 2020 2020 2020 2020 2020 6966 2064 6174            if dat
-00025380: 612e 696c 6f63 5b31 5d5b 224f 7065 6e22  a.iloc[1]["Open"
-00025390: 5d20 3e3d 2064 6174 612e 696c 6f63 5b31  ] >= data.iloc[1
-000253a0: 5d5b 2243 6c6f 7365 225d 3a0d 0a20 2020  ]["Close"]:..   
-000253b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000253c0: 2073 7072 6561 6431 203d 2061 6273 2864   spread1 = abs(d
-000253d0: 6174 612e 696c 6f63 5b31 5d5b 224f 7065  ata.iloc[1]["Ope
-000253e0: 6e22 5d20 2d20 6461 7461 2e69 6c6f 635b  n"] - data.iloc[
-000253f0: 315d 5b22 436c 6f73 6522 5d29 0d0a 2020  1]["Close"])..  
-00025400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025410: 2020 7370 7265 6164 3020 3d20 6162 7328    spread0 = abs(
-00025420: 6461 7461 2e69 6c6f 635b 305d 5b22 4f70  data.iloc[0]["Op
-00025430: 656e 225d 202d 2064 6174 612e 696c 6f63  en"] - data.iloc
-00025440: 5b30 5d5b 2243 6c6f 7365 225d 290d 0a20  [0]["Close"]).. 
-00025450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025460: 2020 206c 6f77 6572 5f77 6963 6b5f 7370     lower_wick_sp
-00025470: 7265 6164 3020 3d20 280d 0a20 2020 2020  read0 = (..     
-00025480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025490: 2020 206d 6178 2864 6174 612e 696c 6f63     max(data.iloc
-000254a0: 5b30 5d5b 224f 7065 6e22 5d2c 2064 6174  [0]["Open"], dat
-000254b0: 612e 696c 6f63 5b30 5d5b 2243 6c6f 7365  a.iloc[0]["Close
-000254c0: 225d 290d 0a20 2020 2020 2020 2020 2020  "])..           
-000254d0: 2020 2020 2020 2020 2020 2020 202d 2064               - d
-000254e0: 6174 612e 696c 6f63 5b30 5d5b 224c 6f77  ata.iloc[0]["Low
-000254f0: 225d 0d0a 2020 2020 2020 2020 2020 2020  "]..            
-00025500: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
-00025510: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-00025520: 6f6c 3120 3d20 6461 7461 2e69 6c6f 635b  ol1 = data.iloc[
-00025530: 315d 5b22 566f 6c75 6d65 225d 0d0a 2020  1]["Volume"]..  
-00025540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025550: 2020 766f 6c30 203d 2064 6174 612e 696c    vol0 = data.il
-00025560: 6f63 5b30 5d5b 2256 6f6c 756d 6522 5d0d  oc[0]["Volume"].
-00025570: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00025580: 2020 2020 2073 6176 6564 203d 2073 656c       saved = sel
-00025590: 662e 6669 6e64 4375 7272 656e 7453 6176  f.findCurrentSav
-000255a0: 6564 5661 6c75 6528 7363 7265 656e 4469  edValue(screenDi
-000255b0: 6374 2c20 7361 7665 4469 6374 2c20 2250  ct, saveDict, "P
-000255c0: 6174 7465 726e 2229 0d0a 2020 2020 2020  attern")..      
-000255d0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000255e0: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
-000255f0: 2020 2020 2020 2020 2020 2020 7370 7265              spre
-00025600: 6164 3020 3e20 7370 7265 6164 310d 0a20  ad0 > spread1.. 
-00025610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025620: 2020 2020 2020 2061 6e64 2076 6f6c 3020         and vol0 
-00025630: 3c20 766f 6c31 0d0a 2020 2020 2020 2020  < vol1..        
-00025640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025650: 616e 6420 6461 7461 2e69 6c6f 635b 305d  and data.iloc[0]
-00025660: 5b22 566f 6c75 6d65 225d 203c 2064 6174  ["Volume"] < dat
-00025670: 612e 696c 6f63 5b30 5d5b 2256 6f6c 4d41  a.iloc[0]["VolMA
-00025680: 225d 0d0a 2020 2020 2020 2020 2020 2020  "]..            
-00025690: 2020 2020 2020 2020 2020 2020 616e 6420              and 
-000256a0: 6461 7461 2e69 6c6f 635b 305d 5b22 436c  data.iloc[0]["Cl
-000256b0: 6f73 6522 5d20 3c3d 2064 6174 612e 696c  ose"] <= data.il
-000256c0: 6f63 5b31 5d5b 224f 7065 6e22 5d0d 0a20  oc[1]["Open"].. 
-000256d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000256e0: 2020 2020 2020 2061 6e64 2073 7072 6561         and sprea
-000256f0: 6430 203c 206c 6f77 6572 5f77 6963 6b5f  d0 < lower_wick_
-00025700: 7370 7265 6164 300d 0a20 2020 2020 2020  spread0..       
+00024b60: 205d 2e64 6573 6372 6962 6528 295b 224c   ].describe()["L
+00024b70: 6f77 225d 5b22 6d69 6e22 5d0d 0a20 2020  ow"]["min"]..   
+00024b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024b90: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
+00024ba0: 2020 2020 6c6f 7750 6f69 6e74 734f 7267      lowPointsOrg
+00024bb0: 203d 206c 6f77 506f 696e 7473 0d0a 2020   = lowPoints..  
+00024bc0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+00024bd0: 7750 6f69 6e74 732e 736f 7274 2872 6576  wPoints.sort(rev
+00024be0: 6572 7365 3d54 7275 6529 0d0a 2020 2020  erse=True)..    
+00024bf0: 2020 2020 2020 2020 2020 2020 6c6f 7750              lowP
+00024c00: 6f69 6e74 7353 6f72 7465 6420 3d20 6c6f  ointsSorted = lo
+00024c10: 7750 6f69 6e74 730d 0a20 2020 2020 2020  wPoints..       
+00024c20: 2020 2020 2020 2020 206c 7470 203d 2064           ltp = d
+00024c30: 6174 612e 6865 6164 2831 295b 2243 6c6f  ata.head(1)["Clo
+00024c40: 7365 225d 2e69 6c6f 635b 305d 0d0a 2020  se"].iloc[0]..  
+00024c50: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00024c60: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
+00024c70: 2020 2020 2020 2020 6c6f 7750 6f69 6e74          lowPoint
+00024c80: 734f 7267 203d 3d20 6c6f 7750 6f69 6e74  sOrg == lowPoint
+00024c90: 7353 6f72 7465 640d 0a20 2020 2020 2020  sSorted..       
+00024ca0: 2020 2020 2020 2020 2020 2020 2061 6e64               and
+00024cb0: 206c 7470 203c 2068 6967 6865 7374 546f   ltp < highestTo
+00024cc0: 700d 0a20 2020 2020 2020 2020 2020 2020  p..             
+00024cd0: 2020 2020 2020 2061 6e64 206c 7470 203e         and ltp >
+00024ce0: 206c 6f77 506f 696e 7473 5b30 5d0d 0a20   lowPoints[0].. 
+00024cf0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00024d00: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00024d10: 2020 2020 2020 2073 6176 6564 203d 2073         saved = s
+00024d20: 656c 662e 6669 6e64 4375 7272 656e 7453  elf.findCurrentS
+00024d30: 6176 6564 5661 6c75 6528 7363 7265 656e  avedValue(screen
+00024d40: 4469 6374 2c20 7361 7665 4469 6374 2c20  Dict, saveDict, 
+00024d50: 2250 6174 7465 726e 2229 0d0a 2020 2020  "Pattern")..    
+00024d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024d70: 7363 7265 656e 4469 6374 5b22 5061 7474  screenDict["Patt
+00024d80: 6572 6e22 5d20 3d20 280d 0a20 2020 2020  ern"] = (..     
+00024d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024da0: 2020 2073 6176 6564 5b30 5d20 0d0a 2020     saved[0] ..  
+00024db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024dc0: 2020 2020 2020 2b20 636f 6c6f 7254 6578        + colorTex
+00024dd0: 742e 424f 4c44 0d0a 2020 2020 2020 2020  t.BOLD..        
+00024de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024df0: 2b20 636f 6c6f 7254 6578 742e 4752 4545  + colorText.GREE
+00024e00: 4e0d 0a20 2020 2020 2020 2020 2020 2020  N..             
+00024e10: 2020 2020 2020 2020 2020 202b 2066 2256             + f"V
+00024e20: 4350 2028 424f 3a20 7b68 6967 6865 7374  CP (BO: {highest
+00024e30: 546f 707d 2922 0d0a 2020 2020 2020 2020  Top})"..        
+00024e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024e50: 2b20 636f 6c6f 7254 6578 742e 454e 440d  + colorText.END.
+00024e60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00024e70: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+00024e80: 2020 2020 2020 2020 2020 2020 7361 7665              save
+00024e90: 4469 6374 5b22 5061 7474 6572 6e22 5d20  Dict["Pattern"] 
+00024ea0: 3d20 7361 7665 645b 315d 202b 2066 2256  = saved[1] + f"V
+00024eb0: 4350 2028 424f 3a20 7b68 6967 6865 7374  CP (BO: {highest
+00024ec0: 546f 707d 2922 0d0a 2020 2020 2020 2020  Top})"..        
+00024ed0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00024ee0: 726e 2054 7275 650d 0a20 2020 2020 2020  rn True..       
+00024ef0: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+00024f00: 6e20 6173 2065 3a20 2023 2070 7261 676d  n as e:  # pragm
+00024f10: 613a 206e 6f20 636f 7665 720d 0a20 2020  a: no cover..   
+00024f20: 2020 2020 2020 2020 2073 656c 662e 6465           self.de
+00024f30: 6661 756c 745f 6c6f 6767 6572 2e64 6562  fault_logger.deb
+00024f40: 7567 2865 2c20 6578 635f 696e 666f 3d54  ug(e, exc_info=T
+00024f50: 7275 6529 0d0a 2020 2020 2020 2020 7265  rue)..        re
+00024f60: 7475 726e 2046 616c 7365 0d0a 0d0a 2020  turn False....  
+00024f70: 2020 2320 5661 6c69 6461 7465 2069 6620    # Validate if 
+00024f80: 766f 6c75 6d65 206f 6620 6c61 7374 2064  volume of last d
+00024f90: 6179 2069 7320 6869 6768 6572 2074 6861  ay is higher tha
+00024fa0: 6e20 6176 670d 0a20 2020 2064 6566 2076  n avg..    def v
+00024fb0: 616c 6964 6174 6556 6f6c 756d 6528 0d0a  alidateVolume(..
+00024fc0: 2020 2020 2020 2020 7365 6c66 2c20 6466          self, df
+00024fd0: 2c20 7363 7265 656e 4469 6374 2c20 7361  , screenDict, sa
+00024fe0: 7665 4469 6374 2c20 766f 6c75 6d65 5261  veDict, volumeRa
+00024ff0: 7469 6f3d 322e 352c 206d 696e 566f 6c75  tio=2.5, minVolu
+00025000: 6d65 3d31 3030 0d0a 2020 2020 293a 0d0a  me=100..    ):..
+00025010: 2020 2020 2020 2020 6966 2064 6620 6973          if df is
+00025020: 204e 6f6e 6520 6f72 206c 656e 2864 6629   None or len(df)
+00025030: 203d 3d20 303a 0d0a 2020 2020 2020 2020   == 0:..        
+00025040: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+00025050: 2c20 4661 6c73 650d 0a20 2020 2020 2020  , False..       
+00025060: 2064 6174 6120 3d20 6466 2e63 6f70 7928   data = df.copy(
+00025070: 290d 0a20 2020 2020 2020 2064 6174 6120  )..        data 
+00025080: 3d20 6461 7461 2e66 696c 6c6e 6128 3029  = data.fillna(0)
+00025090: 0d0a 2020 2020 2020 2020 6461 7461 203d  ..        data =
+000250a0: 2064 6174 612e 7265 706c 6163 6528 5b6e   data.replace([n
+000250b0: 702e 696e 662c 202d 6e70 2e69 6e66 5d2c  p.inf, -np.inf],
+000250c0: 2030 290d 0a20 2020 2020 2020 2072 6563   0)..        rec
+000250d0: 656e 7420 3d20 6461 7461 2e68 6561 6428  ent = data.head(
+000250e0: 3129 0d0a 2020 2020 2020 2020 2320 4569  1)..        # Ei
+000250f0: 7468 6572 2074 6865 2072 6f6c 6c69 6e67  ther the rolling
+00025100: 2076 6f6c 756d 6520 6f66 2070 6173 7420   volume of past 
+00025110: 3230 2073 6573 7369 6f6e 7320 6f72 2074  20 sessions or t
+00025120: 6f64 6179 2773 2076 6f6c 756d 6520 7368  oday's volume sh
+00025130: 6f75 6c64 2062 6520 3e20 6d69 6e20 766f  ould be > min vo
+00025140: 6c75 6d65 0d0a 2020 2020 2020 2020 6861  lume..        ha
+00025150: 734d 696e 696d 756d 566f 6c75 6d65 203d  sMinimumVolume =
+00025160: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
+00025170: 7265 6365 6e74 5b22 566f 6c4d 4122 5d2e  recent["VolMA"].
+00025180: 696c 6f63 5b30 5d20 3e3d 206d 696e 566f  iloc[0] >= minVo
+00025190: 6c75 6d65 0d0a 2020 2020 2020 2020 2020  lume..          
+000251a0: 2020 6f72 2072 6563 656e 745b 2256 6f6c    or recent["Vol
+000251b0: 756d 6522 5d2e 696c 6f63 5b30 5d20 3e3d  ume"].iloc[0] >=
+000251c0: 206d 696e 566f 6c75 6d65 0d0a 2020 2020   minVolume..    
+000251d0: 2020 2020 290d 0a20 2020 2020 2020 2069      )..        i
+000251e0: 6620 7265 6365 6e74 5b22 566f 6c4d 4122  f recent["VolMA"
+000251f0: 5d2e 696c 6f63 5b30 5d20 3d3d 2030 3a20  ].iloc[0] == 0: 
+00025200: 2023 2048 616e 646c 6573 2044 6976 6964   # Handles Divid
+00025210: 6520 6279 2030 2077 6172 6e69 6e67 0d0a  e by 0 warning..
+00025220: 2020 2020 2020 2020 2020 2020 7361 7665              save
+00025230: 4469 6374 5b22 566f 6c75 6d65 225d 203d  Dict["Volume"] =
+00025240: 2030 2020 2320 2255 6e6b 6e6f 776e 220d   0  # "Unknown".
+00025250: 0a20 2020 2020 2020 2020 2020 2073 6372  .            scr
+00025260: 6565 6e44 6963 745b 2256 6f6c 756d 6522  eenDict["Volume"
+00025270: 5d20 3d20 300d 0a20 2020 2020 2020 2020  ] = 0..         
+00025280: 2020 2072 6574 7572 6e20 4661 6c73 652c     return False,
+00025290: 2068 6173 4d69 6e69 6d75 6d56 6f6c 756d   hasMinimumVolum
+000252a0: 650d 0a20 2020 2020 2020 2072 6174 696f  e..        ratio
+000252b0: 203d 2072 6f75 6e64 2872 6563 656e 745b   = round(recent[
+000252c0: 2256 6f6c 756d 6522 5d2e 696c 6f63 5b30  "Volume"].iloc[0
+000252d0: 5d20 2f20 7265 6365 6e74 5b22 566f 6c4d  ] / recent["VolM
+000252e0: 4122 5d2e 696c 6f63 5b30 5d2c 2032 290d  A"].iloc[0], 2).
+000252f0: 0a20 2020 2020 2020 2073 6176 6544 6963  .        saveDic
+00025300: 745b 2256 6f6c 756d 6522 5d20 3d20 7261  t["Volume"] = ra
+00025310: 7469 6f0d 0a20 2020 2020 2020 2069 6620  tio..        if 
+00025320: 7261 7469 6f20 3e3d 2076 6f6c 756d 6552  ratio >= volumeR
+00025330: 6174 696f 2061 6e64 2072 6174 696f 2021  atio and ratio !
+00025340: 3d20 6e70 2e6e 616e 2061 6e64 2028 6e6f  = np.nan and (no
+00025350: 7420 6d61 7468 2e69 7369 6e66 2872 6174  t math.isinf(rat
+00025360: 696f 2929 3a0d 0a20 2020 2020 2020 2020  io)):..         
+00025370: 2020 2073 6372 6565 6e44 6963 745b 2256     screenDict["V
+00025380: 6f6c 756d 6522 5d20 3d20 7261 7469 6f0d  olume"] = ratio.
+00025390: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000253a0: 7572 6e20 5472 7565 2c20 6861 734d 696e  urn True, hasMin
+000253b0: 696d 756d 566f 6c75 6d65 0d0a 2020 2020  imumVolume..    
+000253c0: 2020 2020 7363 7265 656e 4469 6374 5b22      screenDict["
+000253d0: 566f 6c75 6d65 225d 203d 2072 6174 696f  Volume"] = ratio
+000253e0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+000253f0: 2046 616c 7365 2c20 6861 734d 696e 696d   False, hasMinim
+00025400: 756d 566f 6c75 6d65 0d0a 0d0a 2020 2020  umVolume....    
+00025410: 2320 4669 6e64 2069 6620 7374 6f63 6b20  # Find if stock 
+00025420: 6973 2076 616c 6964 6174 696e 6720 766f  is validating vo
+00025430: 6c75 6d65 2073 7072 6561 6420 616e 616c  lume spread anal
+00025440: 7973 6973 0d0a 2020 2020 6465 6620 7661  ysis..    def va
+00025450: 6c69 6461 7465 566f 6c75 6d65 5370 7265  lidateVolumeSpre
+00025460: 6164 416e 616c 7973 6973 2873 656c 662c  adAnalysis(self,
+00025470: 2064 662c 2073 6372 6565 6e44 6963 742c   df, screenDict,
+00025480: 2073 6176 6544 6963 7429 3a0d 0a20 2020   saveDict):..   
+00025490: 2020 2020 2074 7279 3a0d 0a20 2020 2020       try:..     
+000254a0: 2020 2020 2020 2069 6620 6466 2069 7320         if df is 
+000254b0: 4e6f 6e65 206f 7220 6c65 6e28 6466 2920  None or len(df) 
+000254c0: 3d3d 2030 3a0d 0a20 2020 2020 2020 2020  == 0:..         
+000254d0: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+000254e0: 6c73 650d 0a20 2020 2020 2020 2020 2020  lse..           
+000254f0: 2064 6174 6120 3d20 6466 2e63 6f70 7928   data = df.copy(
+00025500: 290d 0a20 2020 2020 2020 2020 2020 2064  )..            d
+00025510: 6174 6120 3d20 6461 7461 2e68 6561 6428  ata = data.head(
+00025520: 3229 0d0a 2020 2020 2020 2020 2020 2020  2)..            
+00025530: 6966 206c 656e 2864 6174 6129 203c 2032  if len(data) < 2
+00025540: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00025550: 2020 2072 6574 7572 6e20 4661 6c73 650d     return False.
+00025560: 0a20 2020 2020 2020 2020 2020 2074 7279  .            try
+00025570: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00025580: 2020 2023 2043 6865 636b 2066 6f72 2070     # Check for p
+00025590: 7265 7669 6f75 7320 5245 4420 6361 6e64  revious RED cand
+000255a0: 6c65 730d 0a20 2020 2020 2020 2020 2020  les..           
+000255b0: 2020 2020 2023 2043 7572 7265 6e74 2063       # Current c
+000255c0: 616e 646c 6520 3d20 3074 682c 2050 7265  andle = 0th, Pre
+000255d0: 7669 6f75 7320 4361 6e64 6c65 203d 2031  vious Candle = 1
+000255e0: 7374 2066 6f72 2066 6f6c 6c6f 7769 6e67  st for following
+000255f0: 206c 6f67 6963 0d0a 2020 2020 2020 2020   logic..        
+00025600: 2020 2020 2020 2020 6966 2064 6174 612e          if data.
+00025610: 696c 6f63 5b31 5d5b 224f 7065 6e22 5d20  iloc[1]["Open"] 
+00025620: 3e3d 2064 6174 612e 696c 6f63 5b31 5d5b  >= data.iloc[1][
+00025630: 2243 6c6f 7365 225d 3a0d 0a20 2020 2020  "Close"]:..     
+00025640: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00025650: 7072 6561 6431 203d 2061 6273 2864 6174  pread1 = abs(dat
+00025660: 612e 696c 6f63 5b31 5d5b 224f 7065 6e22  a.iloc[1]["Open"
+00025670: 5d20 2d20 6461 7461 2e69 6c6f 635b 315d  ] - data.iloc[1]
+00025680: 5b22 436c 6f73 6522 5d29 0d0a 2020 2020  ["Close"])..    
+00025690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000256a0: 7370 7265 6164 3020 3d20 6162 7328 6461  spread0 = abs(da
+000256b0: 7461 2e69 6c6f 635b 305d 5b22 4f70 656e  ta.iloc[0]["Open
+000256c0: 225d 202d 2064 6174 612e 696c 6f63 5b30  "] - data.iloc[0
+000256d0: 5d5b 2243 6c6f 7365 225d 290d 0a20 2020  ]["Close"])..   
+000256e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000256f0: 206c 6f77 6572 5f77 6963 6b5f 7370 7265   lower_wick_spre
+00025700: 6164 3020 3d20 280d 0a20 2020 2020 2020  ad0 = (..       
 00025710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025720: 2061 6e64 2064 6174 612e 696c 6f63 5b30   and data.iloc[0
-00025730: 5d5b 2256 6f6c 756d 6522 5d20 3c3d 2069  ]["Volume"] <= i
-00025740: 6e74 2864 6174 612e 696c 6f63 5b31 5d5b  nt(data.iloc[1][
-00025750: 2256 6f6c 756d 6522 5d20 2a20 302e 3735  "Volume"] * 0.75
-00025760: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00025770: 2020 2020 2020 2029 3a0d 0a20 2020 2020         ):..     
-00025780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025790: 2020 2073 6372 6565 6e44 6963 745b 2250     screenDict["P
-000257a0: 6174 7465 726e 225d 203d 2028 0d0a 2020  attern"] = (..  
-000257b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000257c0: 2020 2020 2020 2020 2020 7361 7665 645b            saved[
-000257d0: 305d 200d 0a20 2020 2020 2020 2020 2020  0] ..           
-000257e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000257f0: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
-00025800: 440d 0a20 2020 2020 2020 2020 2020 2020  D..             
-00025810: 2020 2020 2020 2020 2020 2020 2020 202b                 +
-00025820: 2063 6f6c 6f72 5465 7874 2e47 5245 454e   colorText.GREEN
-00025830: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00025840: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-00025850: 2253 7570 706c 7920 4472 6f75 6768 7422  "Supply Drought"
-00025860: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00025870: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-00025880: 636f 6c6f 7254 6578 742e 454e 440d 0a20  colorText.END.. 
-00025890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000258a0: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-000258b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000258c0: 2020 7361 7665 4469 6374 5b22 5061 7474    saveDict["Patt
-000258d0: 6572 6e22 5d20 3d20 7361 7665 645b 315d  ern"] = saved[1]
-000258e0: 202b 2022 5375 7070 6c79 2044 726f 7567   + "Supply Droug
-000258f0: 6874 220d 0a20 2020 2020 2020 2020 2020  ht"..           
-00025900: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00025910: 7572 6e20 5472 7565 0d0a 2020 2020 2020  urn True..      
-00025920: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00025930: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
-00025940: 2020 2020 2020 2020 2020 2020 7370 7265              spre
-00025950: 6164 3020 3c20 7370 7265 6164 310d 0a20  ad0 < spread1.. 
+00025720: 206d 6178 2864 6174 612e 696c 6f63 5b30   max(data.iloc[0
+00025730: 5d5b 224f 7065 6e22 5d2c 2064 6174 612e  ]["Open"], data.
+00025740: 696c 6f63 5b30 5d5b 2243 6c6f 7365 225d  iloc[0]["Close"]
+00025750: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00025760: 2020 2020 2020 2020 2020 202d 2064 6174             - dat
+00025770: 612e 696c 6f63 5b30 5d5b 224c 6f77 225d  a.iloc[0]["Low"]
+00025780: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00025790: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+000257a0: 2020 2020 2020 2020 2020 2020 2076 6f6c               vol
+000257b0: 3120 3d20 6461 7461 2e69 6c6f 635b 315d  1 = data.iloc[1]
+000257c0: 5b22 566f 6c75 6d65 225d 0d0a 2020 2020  ["Volume"]..    
+000257d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000257e0: 766f 6c30 203d 2064 6174 612e 696c 6f63  vol0 = data.iloc
+000257f0: 5b30 5d5b 2256 6f6c 756d 6522 5d0d 0a20  [0]["Volume"].. 
+00025800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025810: 2020 2073 6176 6564 203d 2073 656c 662e     saved = self.
+00025820: 6669 6e64 4375 7272 656e 7453 6176 6564  findCurrentSaved
+00025830: 5661 6c75 6528 7363 7265 656e 4469 6374  Value(screenDict
+00025840: 2c20 7361 7665 4469 6374 2c20 2250 6174  , saveDict, "Pat
+00025850: 7465 726e 2229 0d0a 2020 2020 2020 2020  tern")..        
+00025860: 2020 2020 2020 2020 2020 2020 6966 2028              if (
+00025870: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00025880: 2020 2020 2020 2020 2020 7370 7265 6164            spread
+00025890: 3020 3e20 7370 7265 6164 310d 0a20 2020  0 > spread1..   
+000258a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000258b0: 2020 2020 2061 6e64 2076 6f6c 3020 3c20       and vol0 < 
+000258c0: 766f 6c31 0d0a 2020 2020 2020 2020 2020  vol1..          
+000258d0: 2020 2020 2020 2020 2020 2020 2020 616e                an
+000258e0: 6420 6461 7461 2e69 6c6f 635b 305d 5b22  d data.iloc[0]["
+000258f0: 566f 6c75 6d65 225d 203c 2064 6174 612e  Volume"] < data.
+00025900: 696c 6f63 5b30 5d5b 2256 6f6c 4d41 225d  iloc[0]["VolMA"]
+00025910: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00025920: 2020 2020 2020 2020 2020 616e 6420 6461            and da
+00025930: 7461 2e69 6c6f 635b 305d 5b22 436c 6f73  ta.iloc[0]["Clos
+00025940: 6522 5d20 3c3d 2064 6174 612e 696c 6f63  e"] <= data.iloc
+00025950: 5b31 5d5b 224f 7065 6e22 5d0d 0a20 2020  [1]["Open"]..   
 00025960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025970: 2020 2020 2020 2061 6e64 2076 6f6c 3020         and vol0 
-00025980: 3e20 766f 6c31 0d0a 2020 2020 2020 2020  > vol1..        
-00025990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000259a0: 616e 6420 6461 7461 2e69 6c6f 635b 305d  and data.iloc[0]
-000259b0: 5b22 566f 6c75 6d65 225d 203e 2064 6174  ["Volume"] > dat
-000259c0: 612e 696c 6f63 5b30 5d5b 2256 6f6c 4d41  a.iloc[0]["VolMA
-000259d0: 225d 0d0a 2020 2020 2020 2020 2020 2020  "]..            
-000259e0: 2020 2020 2020 2020 2020 2020 616e 6420              and 
-000259f0: 6461 7461 2e69 6c6f 635b 305d 5b22 436c  data.iloc[0]["Cl
-00025a00: 6f73 6522 5d20 3c3d 2064 6174 612e 696c  ose"] <= data.il
-00025a10: 6f63 5b31 5d5b 224f 7065 6e22 5d0d 0a20  oc[1]["Open"].. 
-00025a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025a30: 2020 2029 3a0d 0a20 2020 2020 2020 2020     ):..         
-00025a40: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00025a50: 6372 6565 6e44 6963 745b 2250 6174 7465  creenDict["Patte
-00025a60: 726e 225d 203d 2028 0d0a 2020 2020 2020  rn"] = (..      
-00025a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025a80: 2020 2020 2020 7361 7665 645b 305d 200d        saved[0] .
+00025970: 2020 2020 2061 6e64 2073 7072 6561 6430       and spread0
+00025980: 203c 206c 6f77 6572 5f77 6963 6b5f 7370   < lower_wick_sp
+00025990: 7265 6164 300d 0a20 2020 2020 2020 2020  read0..         
+000259a0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+000259b0: 6e64 2064 6174 612e 696c 6f63 5b30 5d5b  nd data.iloc[0][
+000259c0: 2256 6f6c 756d 6522 5d20 3c3d 2069 6e74  "Volume"] <= int
+000259d0: 2864 6174 612e 696c 6f63 5b31 5d5b 2256  (data.iloc[1]["V
+000259e0: 6f6c 756d 6522 5d20 2a20 302e 3735 290d  olume"] * 0.75).
+000259f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00025a00: 2020 2020 2029 3a0d 0a20 2020 2020 2020       ):..       
+00025a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025a20: 2073 6372 6565 6e44 6963 745b 2250 6174   screenDict["Pat
+00025a30: 7465 726e 225d 203d 2028 0d0a 2020 2020  tern"] = (..    
+00025a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025a50: 2020 2020 2020 2020 7361 7665 645b 305d          saved[0]
+00025a60: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00025a70: 2020 2020 2020 2020 2020 2020 2020 202b                 +
+00025a80: 2063 6f6c 6f72 5465 7874 2e42 4f4c 440d   colorText.BOLD.
 00025a90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00025aa0: 2020 2020 2020 2020 2020 2020 202b 2063               + c
-00025ab0: 6f6c 6f72 5465 7874 2e42 4f4c 440d 0a20  olorText.BOLD.. 
+00025ab0: 6f6c 6f72 5465 7874 2e47 5245 454e 0d0a  olorText.GREEN..
 00025ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025ad0: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
-00025ae0: 6f72 5465 7874 2e47 5245 454e 0d0a 2020  orText.GREEN..  
+00025ad0: 2020 2020 2020 2020 2020 2020 2b20 2253              + "S
+00025ae0: 7570 706c 7920 4472 6f75 6768 7422 0d0a  upply Drought"..
 00025af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025b00: 2020 2020 2020 2020 2020 2b20 2244 656d            + "Dem
-00025b10: 616e 6420 5269 7365 220d 0a20 2020 2020  and Rise"..     
+00025b00: 2020 2020 2020 2020 2020 2020 2b20 636f              + co
+00025b10: 6c6f 7254 6578 742e 454e 440d 0a20 2020  lorText.END..   
 00025b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025b30: 2020 2020 2020 202b 2063 6f6c 6f72 5465         + colorTe
-00025b40: 7874 2e45 4e44 0d0a 2020 2020 2020 2020  xt.END..        
-00025b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025b60: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00025b70: 2020 2020 2020 2020 2020 2073 6176 6544             saveD
-00025b80: 6963 745b 2250 6174 7465 726e 225d 203d  ict["Pattern"] =
-00025b90: 2073 6176 6564 5b31 5d20 2b20 2244 656d   saved[1] + "Dem
-00025ba0: 616e 6420 5269 7365 220d 0a20 2020 2020  and Rise"..     
-00025bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025bc0: 2020 2072 6574 7572 6e20 5472 7565 0d0a     return True..
-00025bd0: 2020 2020 2020 2020 2020 2020 6578 6365              exce
-00025be0: 7074 2049 6e64 6578 4572 726f 7220 6173  pt IndexError as
-00025bf0: 2065 3a20 2320 7072 6167 6d61 3a20 6e6f   e: # pragma: no
-00025c00: 2063 6f76 6572 0d0a 2020 2020 2020 2020   cover..        
-00025c10: 2020 2020 2020 2020 7365 6c66 2e64 6566          self.def
-00025c20: 6175 6c74 5f6c 6f67 6765 722e 6465 6275  ault_logger.debu
-00025c30: 6728 652c 2065 7863 5f69 6e66 6f3d 5472  g(e, exc_info=Tr
-00025c40: 7565 290d 0a20 2020 2020 2020 2020 2020  ue)..           
-00025c50: 2020 2020 2070 6173 730d 0a20 2020 2020       pass..     
-00025c60: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-00025c70: 6c73 650d 0a20 2020 2020 2020 2065 7863  lse..        exc
-00025c80: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
-00025c90: 2065 3a20 2023 2070 7261 676d 613a 206e   e:  # pragma: n
-00025ca0: 6f20 636f 7665 720d 0a20 2020 2020 2020  o cover..       
-00025cb0: 2020 2020 2073 656c 662e 6465 6661 756c       self.defaul
-00025cc0: 745f 6c6f 6767 6572 2e64 6562 7567 2865  t_logger.debug(e
-00025cd0: 2c20 6578 635f 696e 666f 3d54 7275 6529  , exc_info=True)
-00025ce0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00025cf0: 7475 726e 2046 616c 7365 0d0a            turn False..
+00025b30: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+00025b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025b50: 7361 7665 4469 6374 5b22 5061 7474 6572  saveDict["Patter
+00025b60: 6e22 5d20 3d20 7361 7665 645b 315d 202b  n"] = saved[1] +
+00025b70: 2022 5375 7070 6c79 2044 726f 7567 6874   "Supply Drought
+00025b80: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
+00025b90: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00025ba0: 6e20 5472 7565 0d0a 2020 2020 2020 2020  n True..        
+00025bb0: 2020 2020 2020 2020 2020 2020 6966 2028              if (
+00025bc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00025bd0: 2020 2020 2020 2020 2020 7370 7265 6164            spread
+00025be0: 3020 3c20 7370 7265 6164 310d 0a20 2020  0 < spread1..   
+00025bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025c00: 2020 2020 2061 6e64 2076 6f6c 3020 3e20       and vol0 > 
+00025c10: 766f 6c31 0d0a 2020 2020 2020 2020 2020  vol1..          
+00025c20: 2020 2020 2020 2020 2020 2020 2020 616e                an
+00025c30: 6420 6461 7461 2e69 6c6f 635b 305d 5b22  d data.iloc[0]["
+00025c40: 566f 6c75 6d65 225d 203e 2064 6174 612e  Volume"] > data.
+00025c50: 696c 6f63 5b30 5d5b 2256 6f6c 4d41 225d  iloc[0]["VolMA"]
+00025c60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00025c70: 2020 2020 2020 2020 2020 616e 6420 6461            and da
+00025c80: 7461 2e69 6c6f 635b 305d 5b22 436c 6f73  ta.iloc[0]["Clos
+00025c90: 6522 5d20 3c3d 2064 6174 612e 696c 6f63  e"] <= data.iloc
+00025ca0: 5b31 5d5b 224f 7065 6e22 5d0d 0a20 2020  [1]["Open"]..   
+00025cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025cc0: 2029 3a0d 0a20 2020 2020 2020 2020 2020   ):..           
+00025cd0: 2020 2020 2020 2020 2020 2020 2073 6372               scr
+00025ce0: 6565 6e44 6963 745b 2250 6174 7465 726e  eenDict["Pattern
+00025cf0: 225d 203d 2028 0d0a 2020 2020 2020 2020  "] = (..        
+00025d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025d10: 2020 2020 7361 7665 645b 305d 200d 0a20      saved[0] .. 
+00025d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025d30: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
+00025d40: 6f72 5465 7874 2e42 4f4c 440d 0a20 2020  orText.BOLD..   
+00025d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025d60: 2020 2020 2020 2020 202b 2063 6f6c 6f72           + color
+00025d70: 5465 7874 2e47 5245 454e 0d0a 2020 2020  Text.GREEN..    
+00025d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025d90: 2020 2020 2020 2020 2b20 2244 656d 616e          + "Deman
+00025da0: 6420 5269 7365 220d 0a20 2020 2020 2020  d Rise"..       
+00025db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025dc0: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
+00025dd0: 2e45 4e44 0d0a 2020 2020 2020 2020 2020  .END..          
+00025de0: 2020 2020 2020 2020 2020 2020 2020 290d                ).
+00025df0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00025e00: 2020 2020 2020 2020 2073 6176 6544 6963           saveDic
+00025e10: 745b 2250 6174 7465 726e 225d 203d 2073  t["Pattern"] = s
+00025e20: 6176 6564 5b31 5d20 2b20 2244 656d 616e  aved[1] + "Deman
+00025e30: 6420 5269 7365 220d 0a20 2020 2020 2020  d Rise"..       
+00025e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025e50: 2072 6574 7572 6e20 5472 7565 0d0a 2020   return True..  
+00025e60: 2020 2020 2020 2020 2020 6578 6365 7074            except
+00025e70: 2049 6e64 6578 4572 726f 7220 6173 2065   IndexError as e
+00025e80: 3a20 2320 7072 6167 6d61 3a20 6e6f 2063  : # pragma: no c
+00025e90: 6f76 6572 0d0a 2020 2020 2020 2020 2020  over..          
+00025ea0: 2020 2020 2020 7365 6c66 2e64 6566 6175        self.defau
+00025eb0: 6c74 5f6c 6f67 6765 722e 6465 6275 6728  lt_logger.debug(
+00025ec0: 652c 2065 7863 5f69 6e66 6f3d 5472 7565  e, exc_info=True
+00025ed0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00025ee0: 2020 2070 6173 730d 0a20 2020 2020 2020     pass..       
+00025ef0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+00025f00: 650d 0a20 2020 2020 2020 2065 7863 6570  e..        excep
+00025f10: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
+00025f20: 3a20 2023 2070 7261 676d 613a 206e 6f20  :  # pragma: no 
+00025f30: 636f 7665 720d 0a20 2020 2020 2020 2020  cover..         
+00025f40: 2020 2073 656c 662e 6465 6661 756c 745f     self.default_
+00025f50: 6c6f 6767 6572 2e64 6562 7567 2865 2c20  logger.debug(e, 
+00025f60: 6578 635f 696e 666f 3d54 7275 6529 0d0a  exc_info=True)..
+00025f70: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00025f80: 726e 2046 616c 7365 0d0a                 rn False..
```

### Comparing `pkscreener-0.44.20240515.377/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240516.378/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.377/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240516.378/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.377/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240516.378/pkscreener/classes/Utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -1364,21 +1364,22 @@
                     + """[+] Select Option:"""
                     + colorText.END
                 ) or "3"
             )
             if resp >= 0 and resp <= 10:
                 if resp == 4:
                     try:
+                        defaultMALength = 9 if configManager.duration.endswith("m") else 50
                         maLength = int(
                             input(
                                 colorText.BOLD
                                 + colorText.WARN
-                                + "\n[+] Enter MA Length (E.g. 50 or 200) (Default=50): "
+                                + f"\n[+] Enter MA Length (E.g. 9,10,20,50 or 200) (Default={defaultMALength}): "
                                 + colorText.END
-                            ) or "50"
+                            ) or str(defaultMALength)
                         )
                         return resp, maLength
                     except ValueError as e:  # pragma: no cover
                         default_logger().debug(e, exc_info=True)
                         OutputControls().printOutput(
                             colorText.BOLD
                             + colorText.FAIL
```

### Comparing `pkscreener-0.44.20240515.377/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240516.378/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.377/pkscreener/classes/keys.py` & `pkscreener-0.44.20240516.378/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.377/pkscreener/courbd.ttf` & `pkscreener-0.44.20240516.378/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.377/pkscreener/globals.py` & `pkscreener-0.44.20240516.378/pkscreener/globals.py`

 * *Files 0% similar despite different names*

```diff
@@ -1634,17 +1634,18 @@
                 showBacktestResults(task.result, sortKey=None, optionalName=task.taskName)
     
     return summary_df,sorting,sortKeys
 
 def addOrRunPipedMenus():
     global userPassedArgs
     # User must have selected menu "P" earlier
-    savedPipes = f"{userPassedArgs.pipedmenus}:;|" if len(userPassedArgs.pipedmenus) > 0 else ""
+    savedPipes = f"{userPassedArgs.pipedmenus}:>|" if len(userPassedArgs.pipedmenus) > 0 else ""
     userPassedArgs.pipedmenus = f"{savedPipes}{userPassedArgs.options}"
     userPassedArgs.pipedmenus = userPassedArgs.pipedmenus.replace("::",":D:")
+    userPassedArgs.pipedmenus = f"{userPassedArgs.pipedmenus}{('i '+configManager.duration) if configManager.isIntradayConfig() else ''}"
     OutputControls().printOutput(
             colorText.GREEN
             + f"[+] {len(userPassedArgs.pipedmenus.split('|'))} Scanners piped so far: {colorText.END}{colorText.WARN+userPassedArgs.pipedmenus+colorText.END}\n{colorText.GREEN}[+] Do you want to add any more scanners into the pipe?"
             + colorText.END
         )
     shouldAddMoreIntoPipe = input(colorText.FAIL + "[+] Select [Y/N] (Default:N): " + colorText.END) or 'n'
     if shouldAddMoreIntoPipe.lower() != 'y':
@@ -1733,21 +1734,23 @@
             sorting = False
     else:
         OutputControls().printOutput("Finished backtesting!")
         sorting = False
     return sorting
 
 def resetConfigToDefault():
+    global userPassedArgs
     isIntraday = userPassedArgs is not None and userPassedArgs.intraday is not None
     if configManager.isIntradayConfig() or isIntraday:
         configManager.toggleConfig(candleDuration="1d", clearCache=False)
-    if "PKDevTools_Default_Log_Level" in os.environ.keys():
-        if userPassedArgs is None or (userPassedArgs is not None and userPassedArgs.options is not None and "|" not in userPassedArgs.options):
-            del os.environ['PKDevTools_Default_Log_Level']
-    configManager.logsEnabled = False
+    if userPassedArgs.monitor is None:
+        if "PKDevTools_Default_Log_Level" in os.environ.keys():
+            if userPassedArgs is None or (userPassedArgs is not None and userPassedArgs.options is not None and "|" not in userPassedArgs.options):
+                del os.environ['PKDevTools_Default_Log_Level']
+        configManager.logsEnabled = False
     configManager.setConfig(ConfigManager.parser,default=True,showFileCreatedText=False)
 
 def prepareStocksForScreening(testing, downloadOnly, listStockCodes, indexOption):
     if not downloadOnly:
         updateMenuChoiceHierarchy()
     indexOption = int(indexOption)
     if listStockCodes is None or len(listStockCodes) == 0:
@@ -1850,21 +1853,21 @@
         input("\nPress <Enter> to Continue...\n")
         return
 
 def handleRequestForSpecificStocks(options, indexOption):
     listStockCodes = []
     strOptions = ""
     if isinstance(options, list):
-        strOptions = ":".join(options).split(";")[0]
+        strOptions = ":".join(options).split(">")[0]
     else:
-        strOptions = options.split(";")[0]
+        strOptions = options.split(">")[0]
     
     if indexOption == 0:
         if len(strOptions) >= 4:
-            strOptions = strOptions.replace(":D:",":").replace(";","")
+            strOptions = strOptions.replace(":D:",":").replace(">","")
             providedOptions = strOptions.split(":")
             for option in providedOptions:
                 if not "".join(str(option).split(".")).isdecimal() and len(option.strip()) > 1:
                     listStockCodes = str(option.strip()).split(",")
                     break
     return listStockCodes
```

### Comparing `pkscreener-0.44.20240515.377/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240516.378/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.377/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240516.378/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.377/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240516.378/pkscreener/pkscreenercli.py`

 * *Files 2% similar despite different names*

```diff
@@ -268,14 +268,20 @@
         except:
             pass
         index += 1
     argsv = argParser.parse_known_args()
     args = argsv[0]
     if args is not None and args.options is not None and not args.options.upper().startswith("T"):
         resetConfigToDefault()
+    if args.monitor is not None:
+        if "PKDevTools_Default_Log_Level" in os.environ.keys():
+            if args is None or (args is not None and args.options is not None and "|" not in args.options):
+                del os.environ['PKDevTools_Default_Log_Level']
+        configManager.logsEnabled = False
+    configManager.setConfig(ConfigManager.parser,default=True,showFileCreatedText=False)
 
 def logFilePath():
     try:
         from PKDevTools.classes import Archiver
 
         filePath = os.path.join(Archiver.get_user_outputs_dir(), "pkscreener-logs.txt")
         f = open(filePath, "w")
@@ -425,25 +431,15 @@
                     if start_time is None:
                         start_time = time.time()
                     else:
                         elapsed_time = round(time.time() - start_time,2)
                         start_time = time.time()
                 monitorOption_org = MarketMonitor().currentMonitorOption()
                 monitorOption = monitorOption_org
-                lastComponent = monitorOption.split(":")[-1]
-                # previousCandleDuration = configManager.duration
-                if "i" in lastComponent:
-                    # We need to switch to intraday scan
-                    monitorOption = monitorOption.replace(lastComponent,"")
-                    args.intraday = lastComponent.replace("i","").strip()
-                    configManager.toggleConfig(candleDuration=args.intraday, clearCache=False)
-                else:
-                    # We need to switch to daily scan
-                    args.intraday = None
-                    configManager.toggleConfig(candleDuration='1d', clearCache=False)
+                monitorOption = checkIntradayComponent(args, monitorOption)
                 if monitorOption.startswith("|"):
                     monitorOption = monitorOption[1:]
                     monitorOptions = monitorOption.split(":")
                     if monitorOptions[1] != "0":
                         monitorOptions[1] = "0"
                         monitorOption = ":".join(monitorOptions)
                     # We need to pipe the output from previous run into the next one
@@ -520,14 +516,29 @@
                 # results = results[~results.index.duplicated(keep='first')]
                 resultStocks = plainResults.index
             if args.monitor is not None:
                 MarketMonitor().saveMonitorResultStocks(plainResults)
                 if results is not None and len(monitorOption_org) > 0:
                     MarketMonitor().refresh(screen_df=results,screenOptions=monitorOption_org, chosenMenu=updateMenuChoiceHierarchy(),dbTimestamp=f"{dbTimestamp} | CycleTime:{elapsed_time}s",telegram=args.telegram)
 
+def checkIntradayComponent(args, monitorOption):
+    lastComponent = monitorOption.split(":")[-1]
+                # previousCandleDuration = configManager.duration
+    if "i" in lastComponent:
+                    # We need to switch to intraday scan
+        monitorOption = monitorOption.replace(lastComponent,"")
+        args.intraday = lastComponent.replace("i","").strip()
+        configManager.toggleConfig(candleDuration=args.intraday, clearCache=False)
+        # args.options = f"{monitorOption}:{args.options[len(lastComponent):]}"
+    else:
+                    # We need to switch to daily scan
+        args.intraday = None
+        configManager.toggleConfig(candleDuration='1d', clearCache=False)
+    return monitorOption
+
 
 def pipeResults(prevOutput,args):
     nextOnes = args.options.split(">")
     hasFoundStocks = False
     if len(nextOnes) > 1:
         monitorOption = nextOnes[1]
         if len(monitorOption) == 0:
```

### Comparing `pkscreener-0.44.20240515.377/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240516.378/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240515.377
+Version: 0.44.20240516.378
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240515.377.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240516.378.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240515.376/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240515.377/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240515.376/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240515.377/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240515.376/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240515.377/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240515.377/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240516.378/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.377/setup.py` & `pkscreener-0.44.20240516.378/setup.py`

 * *Files identical despite different names*

