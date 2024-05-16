# Comparing `tmp/pkscreener-0.44.20240515.376.tar.gz` & `tmp/pkscreener-0.44.20240515.377.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240515.376.tar", last modified: Wed May 15 10:24:08 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240515.377.tar", last modified: Wed May 15 20:53:06 2024, max compression
```

## Comparing `pkscreener-0.44.20240515.376.tar` & `pkscreener-0.44.20240515.377.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 10:24:08.678249 pkscreener-0.44.20240515.376/
--rw-rw-rw-   0        0        0     1086 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-05-15 10:24:08.678249 pkscreener-0.44.20240515.376/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 10:24:08.662029 pkscreener-0.44.20240515.376/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 10:24:08.678249 pkscreener-0.44.20240515.376/pkscreener/classes/
--rw-rw-rw-   0        0        0    13324 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/ArtTexts.py
--rw-rw-rw-   0        0        0    10156 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1537 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    34204 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0    10076 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0    11409 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    42096 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    12534 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    23700 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    22221 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8158 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    18947 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   154876 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    56135 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4993 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    83651 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3789 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-15 10:24:01.000000 pkscreener-0.44.20240515.376/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     5262 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   140752 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/globals.py
--rw-rw-rw-   0        0        0     1041 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    53036 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    32153 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-05-15 10:24:08.662029 pkscreener-0.44.20240515.376/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-05-15 10:24:08.000000 pkscreener-0.44.20240515.376/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2024-05-15 10:24:08.000000 pkscreener-0.44.20240515.376/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 10:24:08.000000 pkscreener-0.44.20240515.376/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-05-15 10:24:08.000000 pkscreener-0.44.20240515.376/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-15 10:24:08.000000 pkscreener-0.44.20240515.376/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-15 10:24:08.000000 pkscreener-0.44.20240515.376/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-15 10:24:08.678249 pkscreener-0.44.20240515.376/setup.cfg
--rw-rw-rw-   0        0        0     4765 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 20:53:06.662270 pkscreener-0.44.20240515.377/
+-rw-rw-rw-   0        0        0     1086 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-05-15 20:53:06.662270 pkscreener-0.44.20240515.377/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 20:53:06.646645 pkscreener-0.44.20240515.377/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 20:53:06.662270 pkscreener-0.44.20240515.377/pkscreener/classes/
+-rw-rw-rw-   0        0        0    13324 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/ArtTexts.py
+-rw-rw-rw-   0        0        0    10156 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1537 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    34250 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10076 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    11407 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    42465 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    12534 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    24534 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    22221 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8158 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    18947 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   154876 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    56135 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4993 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    84592 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3789 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-15 20:53:00.000000 pkscreener-0.44.20240515.377/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     5262 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   141172 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/globals.py
+-rw-rw-rw-   0        0        0     1090 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    53036 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    33205 2024-05-15 20:49:47.000000 pkscreener-0.44.20240515.377/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-05-15 20:53:06.646645 pkscreener-0.44.20240515.377/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-05-15 20:53:06.000000 pkscreener-0.44.20240515.377/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2024-05-15 20:53:06.000000 pkscreener-0.44.20240515.377/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 20:53:06.000000 pkscreener-0.44.20240515.377/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-05-15 20:53:06.000000 pkscreener-0.44.20240515.377/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-15 20:53:06.000000 pkscreener-0.44.20240515.377/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-15 20:53:06.000000 pkscreener-0.44.20240515.377/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-15 20:53:06.662270 pkscreener-0.44.20240515.377/setup.cfg
+-rw-rw-rw-   0        0        0     4765 2024-05-15 20:49:48.000000 pkscreener-0.44.20240515.377/setup.py
```

### Comparing `pkscreener-0.44.20240515.376/LICENSE` & `pkscreener-0.44.20240515.377/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.376/LICENSE-Others` & `pkscreener-0.44.20240515.377/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.376/PKG-INFO` & `pkscreener-0.44.20240515.377/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240515.376
+Version: 0.44.20240515.377
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240515.376.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240515.377.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.375/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240515.376/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.375/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240515.376/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.375/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240515.376/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240515.376/README.md` & `pkscreener-0.44.20240515.377/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.375/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240515.376/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.375/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240515.376/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.375/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240515.376/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240515.376/pkscreener/__init__.py` & `pkscreener-0.44.20240515.377/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.376/pkscreener/classes/ArtTexts.py` & `pkscreener-0.44.20240515.377/pkscreener/classes/ArtTexts.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.376/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240515.377/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.376/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240515.377/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.376/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240515.377/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.376/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240515.377/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.376/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240515.377/pkscreener/classes/ConfigManager.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,18 +72,18 @@
         self.atrTrailingStopSensitivity = 1
         self.atrTrailingStopPeriod = 10
         self.atrTrailingStopEMAPeriod = 200
         # This determines how many days apart the backtest calculations are run.
         # For example, for weekly backtest calculations, set this to 5 (5 days = 1 week)
         # For fortnightly, set this to 10 and so on (10 trading sessions = 2 weeks)
         self.backtestPeriodFactor = 1
-        self.maxDashboardWidgetsPerRow = 3
-        self.maxNumResultRowsInMonitor = 2
+        self.maxDashboardWidgetsPerRow = 5
+        self.maxNumResultRowsInMonitor = 3
         self.calculatersiintraday = False
-        self.defaultMonitorOptions = "X:12:9:2.5,|X:0:5:0:40:i 1m,|{1}X:12:27:,X:12:28,X:12:23,|{3}X:0:31:,X:12:7:3:.01:1,|{1}X:0:29:,X:12:6:3,X:12:6:8,X:12:6:7:1,X:12:6:9,X:12:6:10:1,X:12:7:3:.02:1,X:12:7:6:1,X:12:17,X:12:2,X:12:24,X:12:12:i 5m,X:12:13:i 1m"
+        self.defaultMonitorOptions = " X:12:9:2.5,X:12:23,X:12:28,X:12:31,|{1}X:0:23:>|X:0:27:>|X:0:31:,|{2}X:0:31:,|{3}X:0:27:,X:12:7:3:.01:1,|{5}X:0:5:0:40:,X:12:7:6:1,X:12:11:,X:12:12:i 5m,X:12:17,X:12:24,X:12:6:7:1,X:12:6:3,X:12:6:8,X:12:6:9,X:12:6:10:1,X:12:7:3:.02:1,X:12:13:i 1m,X:12:2,|{1}X:0:29:"
         self.minimumChangePercentage = 0
         self.daysToLookback = 22 * self.backtestPeriodFactor  # 1 month
         self.periods = [1,2,3,4,5,10,15,22,30]
         if self.maxBacktestWindow > self.periods[-1]:
             self.periods.extend(self.maxBacktestWindow)
 
     @property
```

### Comparing `pkscreener-0.44.20240515.376/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240515.377/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.376/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.44.20240515.377/pkscreener/classes/MarketMonitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,18 +79,18 @@
             pass
         return option
 
     def saveMonitorResultStocks(self, results_df):
         if results_df is None or results_df.empty:
             prevOutput_results = "NONE"
         else:
-            prevOutput_results = results_df[~results_df.index.duplicated(keep='first')]
-            prevOutput_results = prevOutput_results.index
-            # Maybe the index is an int ?
-            prevOutput_results = [str(stock) for stock in prevOutput_results]
+            # prevOutput_results = results_df[~results_df.index.duplicated(keep='first')]
+            prevOutput_results = results_df.index
+            # # Maybe the index is an int ?
+            # prevOutput_results = [str(stock) for stock in prevOutput_results]
             prevOutput_results = ",".join(prevOutput_results)
         self.monitorResultStocks[str(self.monitorIndex)] = prevOutput_results
 
     def refresh(self, screen_df:pd.DataFrame=None, screenOptions=None, chosenMenu=None, dbTimestamp="", telegram=False):
         highlightRows = []
         highlightCols = []
         if screen_df is None or screen_df.empty:
```

### Comparing `pkscreener-0.44.20240515.376/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240515.377/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.376/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240515.377/pkscreener/classes/MenuOptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,33 +56,42 @@
     "Z": "Exit (Ctrl + C)",
 }
 level1_P_MenuDict = {
     "1": "Predefined Piped Scanners",
     "2": "Define my custom Piped Scanner",
     "M": "Back to the Top/Main menu",
 }
-level2_P_MenuDict = {
-    "1": "Volume Scanners | High Momentum | ATR Cross",
-    "2": "Volume Scanners | High Momentum",
-    "3": "Volume Scanners | ATR Cross",
-    "4": "Volume Scanners | High Bid/Ask Build Up",
-    "5": "High Momentum | ATR Cross",
-    "6": "High Momentum | ATR Trailing Stop",
-    "7": "ATR Cross | ATR Trailing Stop",
-
-    "M": "Back to the Top/Main menu",
-}
-PIPED_SCANNERS = {"1": "-a y -e -o 'X:12:9:2.5:;|X:0:31:;|X:0:27:'",
-                  "2": "-a y -e -o 'X:12:9:2.5:;|X:0:31:'",
-                  "3": "-a y -e -o 'X:12:9:2.5:;|X:0:27:'",
-                  "4": "-a y -e -o 'X:12:9:2.5:;|X:0:29:'",
-                  "5": "-a y -e -o 'X:12:31:;|X:0:27:'",
-                  "6": "-a y -e -o 'X:12:31:;|X:0:30:1:'",
-                  "7": "-a y -e -o 'X:12:27:;|X:0:30:1:'",
-                  }
+PREDEFINED_SCAN_MENU_KEYS = ["1","2","3","4","5","6","7","8"]
+PREDEFINED_SCAN_MENU_TEXTS = [
+    "Volume Scanners | High Momentum | Breaking Out Now | ATR Cross",
+    "Volume Scanners | High Momentum | ATR Cross",
+    "Volume Scanners | High Momentum",
+    "Volume Scanners | ATR Cross",
+    "Volume Scanners | High Bid/Ask Build Up",
+    "High Momentum | ATR Cross",
+    "High Momentum | ATR Trailing Stop",
+    "ATR Cross | ATR Trailing Stop",
+]
+level2_P_MenuDict = {}
+for key in PREDEFINED_SCAN_MENU_KEYS:
+    level2_P_MenuDict[key] = PREDEFINED_SCAN_MENU_TEXTS[int(key)-1]
+level2_P_MenuDict["M"] = "Back to the Top/Main menu"
+PREDEFINED_SCAN_MENU_VALUES =[
+    "-a y -e -o 'X:12:9:2.5:;|X:0:31:;|X:0:23:;|X:0:27:'",
+    "-a y -e -o 'X:12:9:2.5:;|X:0:31:;|X:0:27:'",
+    "-a y -e -o 'X:12:9:2.5:;|X:0:31:'",
+    "-a y -e -o 'X:12:9:2.5:;|X:0:27:'",
+    "-a y -e -o 'X:12:9:2.5:;|X:0:29:'",
+    "-a y -e -o 'X:12:31:;|X:0:27:'",
+    "-a y -e -o 'X:12:31:;|X:0:30:1:'",
+    "-a y -e -o 'X:12:27:;|X:0:30:1:'",
+]
+PIPED_SCANNERS = {}
+for key in PREDEFINED_SCAN_MENU_KEYS:
+    PIPED_SCANNERS[key] = PREDEFINED_SCAN_MENU_VALUES[int(key)-1]
 
 level1_T_MenuDict = {
     "L": "Long Term",
     "S": "Short Term (Intraday)",
     "M": "Back to the Top/Main menu",
 }
 # Valid periods: 1d,5d,1mo,3mo,6mo,1y,2y,5y,10y,ytd,max
@@ -333,18 +342,19 @@
 # This Class manages application menus
 class menus:
     
     @staticmethod
     def allMenus(topLevel="X",index=12):
         menuOptions = [topLevel]
         indexOptions =[index]
-        scanOptions = [1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,23,24,25,27,28]
+        scanOptions = [1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,23,24,25,27,28,30,31]
         scanSubOptions = {
-                            6:[1,2,3,4,5,6,{7:[1,2]},8,9],
+                            6:[1,2,3,4,5,6,{7:[1,2]},8,9,10],
                             7:[1,2,{3:[1,2]},4,5,{6:[1,3]},7],
+                            30:[1,2],
                             # 21:[3,5,6,7,8,9]
                          }
         runOptions = []
         for menuOption in menuOptions:
             for indexOption in indexOptions:
                 for scanOption in scanOptions:
                     if scanOption in scanSubOptions.keys():
```

### Comparing `pkscreener-0.44.20240515.376/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240515.377/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.376/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240515.377/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,26 +82,36 @@
             morningIntradayCandle = PKMarketOpenCloseAnalyser.getIntradayCandleFromMorning(int_cache_file)
             updatedCandleData = PKMarketOpenCloseAnalyser.combineDailyStockDataWithMorningSimulation(allDailyCandles,morningIntradayCandle)
             # PKMarketOpenCloseAnalyser.updatedCandleData = updatedCandleData
             # PKMarketOpenCloseAnalyser.allDailyCandles = allDailyCandles
             Utility.tools.saveStockData(updatedCandleData,PKMarketOpenCloseAnalyser.configManager,1,False,False, True)
         return updatedCandleData, allDailyCandles
 
-    def runOpenCloseAnalysis(updatedCandleData,allDailyCandles,screen_df,save_df,runOptionName=None):
+    def runOpenCloseAnalysis(updatedCandleData,allDailyCandles,screen_df,save_df,runOptionName=None,filteredListOfStocks=[]):
         # stockListFromMorningTrade,morningIntraday_df = PKMarketOpenCloseAnalyser.simulateMorningTrade(updatedCandleData)
         # latest_daily_df = PKMarketOpenCloseAnalyser.runScanForStocksFromMorningTrade(stockListFromMorningTrade,allDailyCandles)
         try:
-            PKMarketOpenCloseAnalyser.diffMorningCandleDataWithLatestDailyCandleData(screen_df,save_df, updatedCandleData, allDailyCandles,runOptionName=runOptionName)
+            PKMarketOpenCloseAnalyser.diffMorningCandleDataWithLatestDailyCandleData(screen_df,save_df, updatedCandleData, allDailyCandles,runOptionName=runOptionName,filteredListOfStocks=filteredListOfStocks)
         except:
             pass
         Utility.tools.saveStockData(allDailyCandles,PKMarketOpenCloseAnalyser.configManager,1,False,False, True)
 
     def ensureIntradayStockDataExists():
         # Ensure that the intraday_stock_data_<date>.pkl file exists
         exists, cache_file = Utility.tools.afterMarketStockDataExists(intraday=True)
+        copyFilePath = os.path.join(Archiver.get_user_outputs_dir(), f"copy_{cache_file}")
+        srcFilePath = os.path.join(Archiver.get_user_outputs_dir(), cache_file)
+        srcFileSize = os.stat(srcFilePath).st_size
+        if exists and srcFileSize < 1024*1024*50:
+             # File less than 30MB ? Must have been corrupted
+            try:
+                os.remove(srcFilePath)
+                exists = False
+            except:
+                pass
         if not exists:
             savedPeriod = PKMarketOpenCloseAnalyser.configManager.period
             savedDuration = PKMarketOpenCloseAnalyser.configManager.duration
             PKMarketOpenCloseAnalyser.configManager.period = "1d"
             PKMarketOpenCloseAnalyser.configManager.duration = "1m"
             OutputControls().printOutput(f"[+] {colorText.FAIL}{cache_file}{colorText.END} not found under {Archiver.get_user_outputs_dir()} !")
             OutputControls().printOutput(f"[+] {colorText.GREEN}Trying to download {cache_file}{colorText.END}. Please wait ...")
@@ -109,41 +119,47 @@
             exists, cache_file = Utility.tools.afterMarketStockDataExists(intraday=True)
             if not exists:
                 OutputControls().printOutput(f"[+] {colorText.FAIL}{cache_file}{colorText.END} not found under {Archiver.get_user_outputs_dir()} !")
                 OutputControls().printOutput(f"[+] Please run {colorText.FAIL}pkscreener{colorText.END}{colorText.GREEN} -a Y -e -d -i 1m{colorText.END} and then run this menu option again.")
                 input("Press any key to continue...")
             PKMarketOpenCloseAnalyser.configManager.period = savedPeriod
             PKMarketOpenCloseAnalyser.configManager.duration = savedDuration
-        copyFilePath = os.path.join(Archiver.get_user_outputs_dir(), f"copy_{cache_file}")
-        srcFilePath = os.path.join(Archiver.get_user_outputs_dir(), cache_file)
         try:
             if os.path.exists(copyFilePath) and exists:
                 shutil.copy(copyFilePath,srcFilePath) # copy is the saved source of truth
             if not os.path.exists(copyFilePath) and exists: # Let's make a copy of the original one
                 shutil.copy(srcFilePath,copyFilePath)
         except:
             pass
         return exists, cache_file
 
     def ensureDailyStockDataExists():
         # Ensure that the stock_data_<date>.pkl file exists
         exists, cache_file = Utility.tools.afterMarketStockDataExists(intraday=False)
+        copyFilePath = os.path.join(Archiver.get_user_outputs_dir(), f"copy_{cache_file}")
+        srcFilePath = os.path.join(Archiver.get_user_outputs_dir(), cache_file)
+        srcFileSize = os.stat(srcFilePath).st_size
+        if exists and srcFileSize < 1024*1024*50:
+             # File less than 30MB ? Must have been corrupted
+            try:
+                os.remove(srcFilePath)
+                exists = False
+            except:
+                pass
         if not exists:
             OutputControls().printOutput(f"[+] {colorText.FAIL}{cache_file}{colorText.END} not found under {Archiver.get_user_outputs_dir()} !")
         # We should download a fresh copy anyways because we may have altered the existing copy in
         # the previous run. -- !!!! Not required if we saved at the end of last operation !!!!
             OutputControls().printOutput(f"[+] {colorText.GREEN}Trying to download {cache_file}{colorText.END}. Please wait ...")
             Utility.tools.loadStockData({},PKMarketOpenCloseAnalyser.configManager,False,'Y',False,False,None,isIntraday=False,forceRedownload=True)
             exists, cache_file = Utility.tools.afterMarketStockDataExists(intraday=False)
             if not exists:
                 OutputControls().printOutput(f"[+] {colorText.FAIL}{cache_file}{colorText.END} not found under {Archiver.get_user_outputs_dir()} !")
                 OutputControls().printOutput(f"[+] Please run {colorText.FAIL}pkscreener{colorText.END}{colorText.GREEN} -a Y -e -d{colorText.END} and then run this menu option again.")
                 input("Press any key to continue...")
-        copyFilePath = os.path.join(Archiver.get_user_outputs_dir(), f"copy_{cache_file}")
-        srcFilePath = os.path.join(Archiver.get_user_outputs_dir(), cache_file)
         try:
             if os.path.exists(copyFilePath) and exists:
                 shutil.copy(copyFilePath,srcFilePath) # copy is the saved source of truth
             if not os.path.exists(copyFilePath) and exists: # Let's make a copy of the original one
                 shutil.copy(srcFilePath,copyFilePath)
         except:
             pass
@@ -276,23 +292,24 @@
                 continue
         return mutableAllDailyCandles
 
     def runScanForStocksFromMorningTrade(stockListFromMorningTrade,dailyCandleData):
         latest_daily_df = None
         return latest_daily_df
 
-    def diffMorningCandleDataWithLatestDailyCandleData(screen_df,save_df, updatedCandleData, allDailyCandles,runOptionName=None):
+    def diffMorningCandleDataWithLatestDailyCandleData(screen_df,save_df, updatedCandleData, allDailyCandles,runOptionName=None,filteredListOfStocks=[]):
         save_df.reset_index(inplace=True)
         screen_df.reset_index(inplace=True)
         save_df.drop(f"index", axis=1, inplace=True, errors="ignore")
         screen_df.drop(f"index", axis=1, inplace=True, errors="ignore")
         stocks = save_df["Stock"]
         eodLTPs = []
         dayHighLTPs = []
         morningTimestamps = []
+        morningAlertLTPs = []
         sellTimestamps = []
         dayHighTimestamps = []
         sellLTPs = []
         eodDiffs = []
         dayHighDiffs = []
         sqrOffDiffs = []
         index = 0
@@ -326,27 +343,28 @@
                 dayHighTimestamps.append(highTS.strftime("%H:%M"))
                 sellLTPs.append(row["High"][-1])
                 eodLTPs.append(round(endOfDayLTP,2))
                 dayHighLTPs.append(round(dayHighLTP,2))
                 eodDiffs.append(round(endOfDayLTP - morningLTP,2))
                 dayHighDiffs.append(round(dayHighLTP - morningLTP,2))
                 sqrOffDiffs.append(round(row["High"][-1] - morningLTP,2))
+                morningAlertLTPs.append(str(int(round(morningLTP,0))))
                 index += 1
             except:
                 eodLTPs.append("0")
                 eodDiffs.append("0")
                 dayHighLTPs.append("0")
                 dayHighDiffs.append("0")
                 continue
-        diffColumns = ["AlertTime", "SqrOff", "SqrOffLTP", "SqrOffDiff","DayHighTime","DayHigh","DayHighDiff", "EoDLTP", "EoDDiff"]
-        diffValues = [morningTimestamps, sellTimestamps, sellLTPs, sqrOffDiffs,dayHighTimestamps,dayHighLTPs, dayHighDiffs,eodLTPs, eodDiffs]
+        diffColumns = ["LTP@Alert", "AlertTime", "SqrOff", "SqrOffLTP", "SqrOffDiff","DayHighTime","DayHigh","DayHighDiff", "EoDLTP", "EoDDiff"]
+        diffValues = [morningAlertLTPs, morningTimestamps, sellTimestamps, sellLTPs, sqrOffDiffs,dayHighTimestamps,dayHighLTPs, dayHighDiffs,eodLTPs, eodDiffs]
         for col in diffColumns:
             save_df[col] = diffValues[diffColumns.index(col)]
             screen_df.loc[:, col] = save_df.loc[:, col].apply(
-                lambda x: x if col in ["AlertTime", "SqrOff", "SqrOffLTP", "EoDLTP","DayHigh","DayHighTime"] else ((colorText.GREEN if x >= 0 else colorText.FAIL) + str(x) + colorText.END)
+                lambda x: x if col in ["LTP@Alert","AlertTime", "SqrOff", "SqrOffLTP", "EoDLTP","DayHigh","DayHighTime"] else ((colorText.GREEN if x >= 0 else colorText.FAIL) + str(x) + colorText.END)
             )
 
         columns = save_df.columns
         lastIndex = len(save_df)
         for col in columns:
             if col in ["Stock", "Pattern", "LTP", "SqrOffLTP","SqrOffDiff","DayHigh","DayHighDiff","AlertTime", "EoDLTP", "EoDDiff", "%Chng"]:
                 if col == "Stock":
```

### Comparing `pkscreener-0.44.20240515.376/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240515.377/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.376/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240515.377/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.376/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240515.377/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.376/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240515.377/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.376/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240515.377/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.376/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240515.377/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.376/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240515.377/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.376/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240515.377/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.376/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240515.377/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.376/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240515.377/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.376/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240515.377/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.376/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240515.377/pkscreener/classes/Utility.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 """
 import copy
 import datetime
 import glob
 import math
 import os
+import shutil
 import sys
 import textwrap
 import random
 
 os.environ["TF_CPP_MIN_LOG_LEVEL"] = "3"
 os.environ["AUTOGRAPH_VERBOSITY"] = "0"
 
@@ -869,19 +870,23 @@
                 # More than 5 % of stocks are still remaining
                 stockDict, _ = tools.downloadLatestData(stockDict,configManager,leftOutStocks,exchangeSuffix=exchangeSuffix,downloadOnly=downloadOnly)
             # return stockDict
         if downloadOnly or isTrading:
             # We don't want to download from local stale pkl file or stale file at server
             return stockDict
         
-        default_logger().info(
+        default_logger().debug(
             f"Stock data cache file:{cache_file} exists ->{str(exists)}"
         )
         stockDataLoaded = False
-        if exists and not forceRedownload:
+        copyFilePath = os.path.join(Archiver.get_user_outputs_dir(), f"copy_{cache_file}")
+        srcFilePath = os.path.join(Archiver.get_user_outputs_dir(), cache_file)
+        if os.path.exists(copyFilePath):
+            shutil.copy(copyFilePath,srcFilePath) # copy is the saved source of truth
+        if os.path.exists(srcFilePath) and not forceRedownload:
             stockDict, stockDataLoaded = tools.loadDataFromLocalPickle(stockDict,configManager, downloadOnly, defaultAnswer, exchangeSuffix, cache_file, isTrading)
         if (
             not stockDataLoaded
             and ("1d" if isIntraday else ConfigManager.default_period)
             == configManager.period
             and ("1m" if isIntraday else ConfigManager.default_duration)
             == configManager.duration
@@ -900,17 +905,16 @@
         stockDataLoaded = stockDataLoaded or (len(stockDict) > 0 and (len(stockDict) != initialLoadCount))
         if stockDataLoaded:
             tools.saveStockData(stockDict,configManager,initialLoadCount,isIntraday,downloadOnly, forceSave=stockDataLoaded)
         return stockDict
 
     def loadDataFromLocalPickle(stockDict, configManager, downloadOnly, defaultAnswer, exchangeSuffix, cache_file, isTrading):
         stockDataLoaded = False
-        with open(
-                os.path.join(Archiver.get_user_outputs_dir(), cache_file), "rb"
-            ) as f:
+        srcFilePath = os.path.join(Archiver.get_user_outputs_dir(), cache_file)
+        with open(srcFilePath, "rb") as f:
             try:
                 stockData = pickle.load(f)
                 if not downloadOnly:
                     OutputControls().printOutput(
                             colorText.BOLD
                             + colorText.GREEN
                             + f"[+] Automatically Using Cached Stock Data {'due to After-Market hours' if not PKDateUtilities.isTradingTime() else ''}!"
@@ -1084,14 +1088,20 @@
                                     if not isTrading:
                                         stockDict[stock] = df_or_dict
                             except:
                                     # Probably, the "stock" got removed from the latest download
                                     # and so, was not found in stockDict
                                 continue
                         stockDataLoaded = True
+                        copyFilePath = os.path.join(Archiver.get_user_outputs_dir(), f"copy_{cache_file}")
+                        srcFilePath = os.path.join(Archiver.get_user_outputs_dir(), cache_file)
+                        if os.path.exists(copyFilePath) and os.path.exists(srcFilePath):
+                            shutil.copy(copyFilePath,srcFilePath) # copy is the saved source of truth
+                        if not os.path.exists(copyFilePath) and os.path.exists(srcFilePath): # Let's make a copy of the original one
+                            shutil.copy(srcFilePath,copyFilePath)
                         # Remove the progress bar now!
                         sys.stdout.write("\x1b[1A")  # cursor up one line
                         sys.stdout.write("\x1b[2K")  # delete the last line
                 except Exception as e:  # pragma: no cover
                     default_logger().debug(e, exc_info=True)
                     f.close()
                     OutputControls().printOutput("[!] Download Error - " + str(e))
```

### Comparing `pkscreener-0.44.20240515.376/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240515.377/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.376/pkscreener/classes/keys.py` & `pkscreener-0.44.20240515.377/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.376/pkscreener/courbd.ttf` & `pkscreener-0.44.20240515.377/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.376/pkscreener/globals.py` & `pkscreener-0.44.20240515.377/pkscreener/globals.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,16 @@
     level3_X_Reversal_MenuDict,
     level4_X_Lorenzian_MenuDict,
     level4_X_ChartPattern_Confluence_MenuDict,
     level4_X_ChartPattern_BBands_SQZ_MenuDict,
     menus,
     MAX_SUPPORTED_MENU_OPTION,
     MAX_MENU_OPTION,
-    PIPED_SCANNERS
+    PIPED_SCANNERS,
+    PREDEFINED_SCAN_MENU_KEYS
 )
 from pkscreener.classes.OtaUpdater import OTAUpdater
 from pkscreener.classes.Portfolio import PortfolioCollection
 from pkscreener.classes.PKTask import PKTask
 from pkscreener.classes.PKScheduler import PKScheduler
 from pkscreener.classes.PKScanRunner import PKScanRunner
 from pkscreener.classes.PKMarketOpenCloseAnalyser import PKMarketOpenCloseAnalyser
@@ -789,15 +790,15 @@
             return None, None
         if predefinedOption == "1":
             Utility.tools.clearScreen(forceTop=True)
             selectedMenu = m1.find(predefinedOption)
             m2.renderForMenu(selectedMenu=selectedMenu)
             selPredefinedOption = input(colorText.BOLD + colorText.FAIL + "[+] Select option: ") or "1"
             OutputControls().printOutput(colorText.END, end="")
-            if selPredefinedOption in ["1","2","3","4","5","6","7"]:
+            if selPredefinedOption in PREDEFINED_SCAN_MENU_KEYS:
                 scannerOption = PIPED_SCANNERS[selPredefinedOption]
                 Utility.tools.clearScreen(forceTop=True)
                 if userPassedArgs.pipedmenus is not None:
                     chosenOptions = scannerOption.split("-o ")[1]
                     userPassedArgs.options = chosenOptions.replace("'","")
                     return addOrRunPipedMenus()
                 launcher = sys.argv[0]
@@ -1278,15 +1279,16 @@
                 return handleMonitorFiveEMA()
             else:
                 if str(menuOption).upper() == "C":
                     stockDictPrimary,endOfdayCandles = PKMarketOpenCloseAnalyser.getStockDataForSimulation()
                     if stockDictPrimary is None or endOfdayCandles is None:
                         OutputControls().printOutput(f"Cannot proceed! Stock data is unavailable. Please check the error logs/messages !")
                         return None, None
-                    listStockCodes = sorted(list(filter(None,list(set(stockDictPrimary.keys())))))
+                    if indexOption > 0:
+                        listStockCodes = sorted(list(filter(None,list(set(stockDictPrimary.keys())))))
                 listStockCodes = prepareStocksForScreening(testing, downloadOnly, listStockCodes, indexOption)
         except urllib.error.URLError as e:
             default_logger().debug(e, exc_info=True)
             OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.FAIL
                 + "\n\n[+] Oops! It looks like you don't have an Internet connectivity at the moment!"
@@ -1375,15 +1377,15 @@
             screenResults, saveResults, backtest_df, tasks_queue, results_queue, consumers,logging_queue = PKScanRunner.runScanWithParams(userPassedArgs,keyboardInterruptEvent,screenCounter,screenResultsCounter,stockDictPrimary,stockDictSecondary,testing, backtestPeriod, menuOption,executeOption, samplingDuration, items,screenResults, saveResults, backtest_df,scanningCb=runScanners,tasks_queue=tasks_queue, results_queue=results_queue, consumers=consumers,logging_queue=logging_queue)
             if userPassedArgs is not None and (userPassedArgs.monitor is None and "|" not in userPassedArgs.options and not userPassedArgs.options.upper().startswith("C")):
                 tasks_queue = None
                 results_queue = None
                 consumers = None
             if menuOption in ["C"]:
                 runOptionName = PKScanRunner.getFormattedChoices(userPassedArgs,selectedChoice)
-                PKMarketOpenCloseAnalyser.runOpenCloseAnalysis(stockDictPrimary,endOfdayCandles,screenResults, saveResults,runOptionName=runOptionName)
+                PKMarketOpenCloseAnalyser.runOpenCloseAnalysis(stockDictPrimary,endOfdayCandles,screenResults, saveResults,runOptionName=runOptionName,filteredListOfStocks=listStockCodes)
             if downloadOnly and menuOption in ["X"]:
                 screener.getFreshMFIStatus(stock="LatestCheckedOnDate")
                 screener.getFairValue(stock="LatestCheckedOnDate", force=True)
             if not downloadOnly and menuOption in ["X", "G", "C"]:
                 if menuOption == "G":
                     userPassedArgs.backtestdaysago = backtestPeriod
                 if screenResults is not None and len(screenResults) > 0:
@@ -2003,14 +2005,17 @@
             maxcolwidths=Utility.tools.getMaxColumnWidths(strategy_df)
         ).encode("utf-8").decode(STD_ENCODING)
         OutputControls().printOutput(addendumLabel)
         OutputControls().printOutput(tabulated_strategy)
     if screenResults is not None and len(screenResults) >= 1:
         choiceSegments = menuChoiceHierarchy.split(">")
         choiceSegments = f"{choiceSegments[-2]} > {choiceSegments[-1]}" if len(choiceSegments)>=4 else f"{choiceSegments[-1]}"
+        pipedTitle = f"{userPassedArgs.pipedtitle}|" if userPassedArgs.pipedtitle is not None else ""
+        pipedTitle = f'| Piped Results: {pipedTitle}{choiceSegments}[{len(saveResults)}]' if len(pipedTitle) > 0 else ""
+        pipedTitle = pipedTitle.replace("[","<b>[").replace("]","]</b>")
         title = f'<b>{reportTitle}{choiceSegments}</b>{"" if selectedChoice["0"] != "G" else " for Date:"+ targetDateG10k}'
         if (
             ("RUNNER" in os.environ.keys() and os.environ["RUNNER"] != "LOCAL_RUN_SCANNER")
             or "PKDevTools_Default_Log_Level" in os.environ.keys()
         ):
             if eligible:
                 # There's no need to save data locally.
@@ -2061,15 +2066,15 @@
                     caption_results = colorText.miniTabulator().tabulate(
                         caption_df,
                         headers="keys",
                         tablefmt=colorText.No_Pad_GridFormat,
                         maxcolwidths=[None,None,4,3]
                     ).encode("utf-8").decode(STD_ENCODING).replace("-K-----S-----C-----R","-K-----S----C---R").replace("%  ","% ").replace("=K=====S=====C=====R","=K=====S====C===R").replace("Vol  |","Vol|").replace("x  ","x")
                     caption_results = caption_results.replace("-E-----N-----E-----R","-E-----N----E---R").replace("=E=====N=====E=====R","=E=====N====E===R")
-                    caption = f"{caption}.Open attached image for more. Samples:<pre>{caption_results}</pre>{elapsed_text}" #<i>Author is <u><b>NOT</b> a SEBI registered financial advisor</u> and MUST NOT be deemed as one.</i>"
+                    caption = f"{caption}.Open attached image for more. Samples:<pre>{caption_results}</pre>{elapsed_text}{pipedTitle}" #<i>Author is <u><b>NOT</b> a SEBI registered financial advisor</u> and MUST NOT be deemed as one.</i>"
                 if not testing: # and not userPassedArgs.runintradayanalysis:
                     sendQuickScanResult(
                         f"{reportTitle}{menuChoiceHierarchy}",
                         user,
                         tabulated_results,
                         markdown_results,
                         caption,
```

### Comparing `pkscreener-0.44.20240515.376/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240515.377/pkscreener/pkscreener.ini`

 * *Files 21% similar despite different names*

```diff
@@ -1,66 +1,69 @@
 00000000: 5b63 6f6e 6669 675d 0d0a 6174 7274 7261  [config]..atrtra
 00000010: 696c 696e 6773 746f 7065 6d61 7065 7269  ilingstopemaperi
-00000020: 6f64 203d 2039 0d0a 6174 7274 7261 696c  od = 9..atrtrail
-00000030: 696e 6773 746f 7070 6572 696f 6420 3d20  ingstopperiod = 
-00000040: 3231 0d0a 6174 7274 7261 696c 696e 6773  21..atrtrailings
-00000050: 746f 7073 656e 7369 7469 7669 7479 203d  topsensitivity =
-00000060: 2031 2e30 0d0a 6261 636b 7465 7374 7065   1.0..backtestpe
-00000070: 7269 6f64 203d 2031 3230 0d0a 6261 636b  riod = 120..back
-00000080: 7465 7374 7065 7269 6f64 6661 6374 6f72  testperiodfactor
-00000090: 203d 2031 0d0a 6361 6368 6573 746f 636b   = 1..cachestock
-000000a0: 6461 7461 203d 2079 0d0a 6361 6c63 756c  data = y..calcul
-000000b0: 6174 6572 7369 696e 7472 6164 6179 203d  atersiintraday =
-000000c0: 206e 0d0a 6461 7973 746f 6c6f 6f6b 6261   n..daystolookba
-000000d0: 636b 203d 2032 320d 0a64 6566 6175 6c74  ck = 22..default
-000000e0: 696e 6465 7820 3d20 3132 0d0a 6465 6661  index = 12..defa
-000000f0: 756c 746d 6f6e 6974 6f72 6f70 7469 6f6e  ultmonitoroption
-00000100: 7320 3d20 583a 3132 3a39 3a32 2e35 2c7c  s = X:12:9:2.5,|
-00000110: 583a 303a 353a 303a 3430 3a69 2031 6d2c  X:0:5:0:40:i 1m,
-00000120: 7c7b 317d 583a 3132 3a32 373a 2c58 3a31  |{1}X:12:27:,X:1
-00000130: 323a 3238 2c58 3a31 323a 3233 2c7c 7b33  2:28,X:12:23,|{3
-00000140: 7d58 3a30 3a33 313a 2c58 3a31 323a 373a  }X:0:31:,X:12:7:
-00000150: 333a 2e30 313a 312c 7c7b 317d 583a 303a  3:.01:1,|{1}X:0:
-00000160: 3239 3a2c 583a 3132 3a36 3a33 2c58 3a31  29:,X:12:6:3,X:1
-00000170: 323a 363a 382c 583a 3132 3a36 3a37 3a31  2:6:8,X:12:6:7:1
-00000180: 2c58 3a31 323a 363a 392c 583a 3132 3a36  ,X:12:6:9,X:12:6
-00000190: 3a31 303a 312c 583a 3132 3a37 3a33 3a2e  :10:1,X:12:7:3:.
-000001a0: 3032 3a31 2c58 3a31 323a 373a 363a 312c  02:1,X:12:7:6:1,
-000001b0: 583a 3132 3a31 372c 583a 3132 3a32 2c58  X:12:17,X:12:2,X
-000001c0: 3a31 323a 3234 2c58 3a31 323a 3132 3a69  :12:24,X:12:12:i
-000001d0: 2035 6d2c 583a 3132 3a31 333a 6920 316d   5m,X:12:13:i 1m
-000001e0: 0d0a 6475 7261 7469 6f6e 203d 2031 640d  ..duration = 1d.
-000001f0: 0a65 6e61 626c 6570 6f72 7466 6f6c 696f  .enableportfolio
-00000200: 6361 6c63 756c 6174 696f 6e73 203d 206e  calculations = n
-00000210: 0d0a 6765 6e65 7261 6c74 696d 656f 7574  ..generaltimeout
-00000220: 203d 2032 2e30 0d0a 6c6f 6773 656e 6162   = 2.0..logsenab
-00000230: 6c65 6420 3d20 6e0d 0a6c 6f6e 6774 696d  led = n..longtim
-00000240: 656f 7574 203d 2034 2e30 0d0a 6d61 7862  eout = 4.0..maxb
-00000250: 6163 6b74 6573 7477 696e 646f 7720 3d20  acktestwindow = 
-00000260: 3330 0d0a 6d61 7864 6173 6862 6f61 7264  30..maxdashboard
-00000270: 7769 6467 6574 7370 6572 726f 7720 3d20  widgetsperrow = 
-00000280: 330d 0a6d 6178 6e65 7477 6f72 6b72 6574  3..maxnetworkret
-00000290: 7279 636f 756e 7420 3d20 3130 0d0a 6d61  rycount = 10..ma
-000002a0: 786e 756d 7265 7375 6c74 726f 7773 696e  xnumresultrowsin
-000002b0: 6d6f 6e69 746f 7220 3d20 320d 0a6d 6f72  monitor = 2..mor
-000002c0: 6e69 6e67 616e 616c 7973 6973 6361 6e64  ninganalysiscand
-000002d0: 6c65 6e75 6d62 6572 203d 2032 350d 0a6d  lenumber = 25..m
-000002e0: 6f72 6e69 6e67 616e 616c 7973 6973 6361  orninganalysisca
-000002f0: 6e64 6c65 6475 7261 7469 6f6e 203d 2031  ndleduration = 1
-00000300: 6d0d 0a6f 6e6c 7973 7461 6765 7477 6f73  m..onlystagetwos
-00000310: 746f 636b 7320 3d20 790d 0a70 6572 696f  tocks = y..perio
-00000320: 6420 3d20 3238 3064 0d0a 7368 6f77 7061  d = 280d..showpa
-00000330: 7374 7374 7261 7465 6779 6461 7461 203d  ststrategydata =
-00000340: 206e 0d0a 7368 6f77 756e 6b6e 6f77 6e74   n..showunknownt
-00000350: 7265 6e64 7320 3d20 790d 0a73 6875 6666  rends = y..shuff
-00000360: 6c65 203d 2079 0d0a 7573 6565 6d61 203d  le = y..useema =
-00000370: 206e 0d0a 0d0a 5b66 696c 7465 7273 5d0d   n....[filters].
-00000380: 0a63 6f6e 736f 6c69 6461 7469 6f6e 7065  .consolidationpe
-00000390: 7263 656e 7461 6765 203d 2031 302e 300d  rcentage = 10.0.
-000003a0: 0a6d 6178 7072 6963 6520 3d20 3530 3030  .maxprice = 5000
-000003b0: 302e 300d 0a6d 696e 696d 756d 6368 616e  0.0..minimumchan
-000003c0: 6765 7065 7263 656e 7461 6765 203d 2030  gepercentage = 0
-000003d0: 2e30 0d0a 6d69 6e69 6d75 6d76 6f6c 756d  .0..minimumvolum
-000003e0: 6520 3d20 3130 3030 300d 0a6d 696e 7072  e = 10000..minpr
-000003f0: 6963 6520 3d20 3230 2e30 0d0a 766f 6c75  ice = 20.0..volu
-00000400: 6d65 7261 7469 6f20 3d20 322e 350d 0a0d  meratio = 2.5...
-00000410: 0a                                       .
+00000020: 6f64 203d 2032 3030 0d0a 6174 7274 7261  od = 200..atrtra
+00000030: 696c 696e 6773 746f 7070 6572 696f 6420  ilingstopperiod 
+00000040: 3d20 3130 0d0a 6174 7274 7261 696c 696e  = 10..atrtrailin
+00000050: 6773 746f 7073 656e 7369 7469 7669 7479  gstopsensitivity
+00000060: 203d 2031 2e30 0d0a 6261 636b 7465 7374   = 1.0..backtest
+00000070: 7065 7269 6f64 203d 2031 3230 0d0a 6261  period = 120..ba
+00000080: 636b 7465 7374 7065 7269 6f64 6661 6374  cktestperiodfact
+00000090: 6f72 203d 2031 0d0a 6361 6368 6573 746f  or = 1..cachesto
+000000a0: 636b 6461 7461 203d 2079 0d0a 6361 6c63  ckdata = y..calc
+000000b0: 756c 6174 6572 7369 696e 7472 6164 6179  ulatersiintraday
+000000c0: 203d 206e 0d0a 6461 7973 746f 6c6f 6f6b   = n..daystolook
+000000d0: 6261 636b 203d 2032 320d 0a64 6566 6175  back = 22..defau
+000000e0: 6c74 696e 6465 7820 3d20 3132 0d0a 6465  ltindex = 12..de
+000000f0: 6661 756c 746d 6f6e 6974 6f72 6f70 7469  faultmonitoropti
+00000100: 6f6e 7320 3d20 2058 3a31 323a 393a 322e  ons =  X:12:9:2.
+00000110: 352c 583a 3132 3a32 332c 583a 3132 3a32  5,X:12:23,X:12:2
+00000120: 382c 583a 3132 3a33 312c 7c7b 317d 583a  8,X:12:31,|{1}X:
+00000130: 3132 3a32 333a 3e7c 583a 303a 3237 3a3e  12:23:>|X:0:27:>
+00000140: 7c58 3a30 3a33 313a 2c7c 7b32 7d58 3a30  |X:0:31:,|{2}X:0
+00000150: 3a33 313a 2c7c 7b33 7d58 3a30 3a32 373a  :31:,|{3}X:0:27:
+00000160: 2c58 3a31 323a 373a 333a 2e30 313a 312c  ,X:12:7:3:.01:1,
+00000170: 7c7b 357d 583a 303a 353a 303a 3430 3a2c  |{5}X:0:5:0:40:,
+00000180: 583a 3132 3a37 3a36 3a31 2c58 3a31 323a  X:12:7:6:1,X:12:
+00000190: 3131 3a2c 583a 3132 3a31 323a 6920 356d  11:,X:12:12:i 5m
+000001a0: 2c58 3a31 323a 3137 2c58 3a31 323a 3234  ,X:12:17,X:12:24
+000001b0: 2c58 3a31 323a 363a 373a 312c 583a 3132  ,X:12:6:7:1,X:12
+000001c0: 3a36 3a33 2c58 3a31 323a 363a 382c 583a  :6:3,X:12:6:8,X:
+000001d0: 3132 3a36 3a39 2c58 3a31 323a 363a 3130  12:6:9,X:12:6:10
+000001e0: 3a31 2c58 3a31 323a 373a 333a 2e30 323a  :1,X:12:7:3:.02:
+000001f0: 312c 583a 3132 3a31 333a 6920 316d 2c58  1,X:12:13:i 1m,X
+00000200: 3a31 323a 322c 7c7b 317d 583a 303a 3239  :12:2,|{1}X:0:29
+00000210: 3a0d 0a64 7572 6174 696f 6e20 3d20 3164  :..duration = 1d
+00000220: 0d0a 656e 6162 6c65 706f 7274 666f 6c69  ..enableportfoli
+00000230: 6f63 616c 6375 6c61 7469 6f6e 7320 3d20  ocalculations = 
+00000240: 6e0d 0a67 656e 6572 616c 7469 6d65 6f75  n..generaltimeou
+00000250: 7420 3d20 322e 300d 0a6c 6f67 7365 6e61  t = 2.0..logsena
+00000260: 626c 6564 203d 206e 0d0a 6c6f 6e67 7469  bled = n..longti
+00000270: 6d65 6f75 7420 3d20 342e 300d 0a6d 6178  meout = 4.0..max
+00000280: 6261 636b 7465 7374 7769 6e64 6f77 203d  backtestwindow =
+00000290: 2033 300d 0a6d 6178 6461 7368 626f 6172   30..maxdashboar
+000002a0: 6477 6964 6765 7473 7065 7272 6f77 203d  dwidgetsperrow =
+000002b0: 2035 0d0a 6d61 786e 6574 776f 726b 7265   5..maxnetworkre
+000002c0: 7472 7963 6f75 6e74 203d 2031 300d 0a6d  trycount = 10..m
+000002d0: 6178 6e75 6d72 6573 756c 7472 6f77 7369  axnumresultrowsi
+000002e0: 6e6d 6f6e 6974 6f72 203d 2033 0d0a 6d6f  nmonitor = 3..mo
+000002f0: 726e 696e 6761 6e61 6c79 7369 7363 616e  rninganalysiscan
+00000300: 646c 656e 756d 6265 7220 3d20 3235 0d0a  dlenumber = 25..
+00000310: 6d6f 726e 696e 6761 6e61 6c79 7369 7363  morninganalysisc
+00000320: 616e 646c 6564 7572 6174 696f 6e20 3d20  andleduration = 
+00000330: 316d 0d0a 6f6e 6c79 7374 6167 6574 776f  1m..onlystagetwo
+00000340: 7374 6f63 6b73 203d 2079 0d0a 7065 7269  stocks = y..peri
+00000350: 6f64 203d 2032 3830 640d 0a73 686f 7770  od = 280d..showp
+00000360: 6173 7473 7472 6174 6567 7964 6174 6120  aststrategydata 
+00000370: 3d20 6e0d 0a73 686f 7775 6e6b 6e6f 776e  = n..showunknown
+00000380: 7472 656e 6473 203d 2079 0d0a 7368 7566  trends = y..shuf
+00000390: 666c 6520 3d20 790d 0a75 7365 656d 6120  fle = y..useema 
+000003a0: 3d20 6e0d 0a0d 0a5b 6669 6c74 6572 735d  = n....[filters]
+000003b0: 0d0a 636f 6e73 6f6c 6964 6174 696f 6e70  ..consolidationp
+000003c0: 6572 6365 6e74 6167 6520 3d20 3130 2e30  ercentage = 10.0
+000003d0: 0d0a 6d61 7870 7269 6365 203d 2035 3030  ..maxprice = 500
+000003e0: 3030 2e30 0d0a 6d69 6e69 6d75 6d63 6861  00.0..minimumcha
+000003f0: 6e67 6570 6572 6365 6e74 6167 6520 3d20  ngepercentage = 
+00000400: 302e 300d 0a6d 696e 696d 756d 766f 6c75  0.0..minimumvolu
+00000410: 6d65 203d 2031 3030 3030 0d0a 6d69 6e70  me = 10000..minp
+00000420: 7269 6365 203d 2032 302e 300d 0a76 6f6c  rice = 20.0..vol
+00000430: 756d 6572 6174 696f 203d 2032 2e35 0d0a  umeratio = 2.5..
+00000440: 0d0a                                     ..
```

### Comparing `pkscreener-0.44.20240515.376/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240515.377/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.376/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240515.377/pkscreener/pkscreenercli.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,14 +242,17 @@
 argParser.add_argument(
     "--pipedmenus",
     help="Piped Menus",
     required=False,
 )
 argsv = argParser.parse_known_args()
 args = argsv[0]
+# if sys.argv[0].endswith(".py"):
+#     args.monitor = 'X'
+#     args.answerdefault = 'Y'
 results = None
 resultStocks = None
 plainResults = None
 start_time = None
 dbTimestamp = None
 elapsed_time = None
 configManager = ConfigManager.tools()
@@ -340,14 +343,17 @@
     try:
         savedPipedArgs = None
         savedPipedArgs = args.pipedmenus if args is not None and args.pipedmenus is not None else None
     except:
         pass
     argsv = argParser.parse_known_args()
     args = argsv[0]
+    # if sys.argv[0].endswith(".py"):
+    #     args.monitor = 'X'
+    #     args.answerdefault = 'Y'
     args.pipedmenus = savedPipedArgs
     if args.options is not None:
         args.options = args.options.replace("::",":")
     if args.runintradayanalysis:
         from pkscreener.classes.MenuOptions import menus
         runOptions = menus.allMenus(topLevel="C", index=12)
         optionalFinalOutcome_df = None
@@ -431,47 +437,53 @@
                     args.intraday = lastComponent.replace("i","").strip()
                     configManager.toggleConfig(candleDuration=args.intraday, clearCache=False)
                 else:
                     # We need to switch to daily scan
                     args.intraday = None
                     configManager.toggleConfig(candleDuration='1d', clearCache=False)
                 if monitorOption.startswith("|"):
-                    monitorOption = monitorOption.replace("|","")
+                    monitorOption = monitorOption[1:]
                     monitorOptions = monitorOption.split(":")
                     if monitorOptions[1] != "0":
                         monitorOptions[1] = "0"
                         monitorOption = ":".join(monitorOptions)
                     # We need to pipe the output from previous run into the next one
                     if monitorOption.startswith("{") and "}" in monitorOption:
                         srcIndex = monitorOption.split("}")[0].split("{")[-1]
                         monitorOption="".join(monitorOption.split("}")[1:])
                         try:
                             srcIndex = int(srcIndex)
                             # Let's get the previously saved result for the monitor
                             savedStocks = MarketMonitor().monitorResultStocks[str(srcIndex)]
-                            monitorOption = f"{monitorOption}:{savedStocks}"
+                            innerPipes = monitorOption.split("|")
+                            nextPipe = innerPipes[0]
+                            nextMonitor = nextPipe.split(">")[0]
+                            innerPipes[0] = f"{nextMonitor}:{savedStocks}"
+                            monitorOption = ":>|".join(innerPipes)
+                            monitorOption = monitorOption.replace("::",":").replace(":>:>",":>")
+                            # monitorOption = f"{monitorOption}:{savedStocks}:"
                         except:
                             # Probably wrong (non-integer) index passed. Let's continue anyway
                             pass
                     elif resultStocks is not None:
                         resultStocks = ",".join(resultStocks)
                         monitorOption = f"{monitorOption}:{resultStocks}"
                 args.options = monitorOption.replace("::",":")
                 # (previousCandleDuration != configManager.duration) or 
                 if (MarketMonitor().monitorIndex == 1 and args.options is not None and plainResults is not None):
                     # Load the stock data afresh for each cycle
                     refreshStockData(args.options)
-            try: 
+            try:
                 results = None
                 plainResults = None
                 resultStocks = None
                 results, plainResults = main(userArgs=args)
                 if args.pipedmenus is not None:
                     while args.pipedmenus is not None:
-                        main(userArgs=args)
+                        results, plainResults = main(userArgs=args)
                     sys.exit(0)
                 if isInterrupted():
                     closeWorkersAndExit()
                     removeMonitorFile()
                     sys.exit(0)
                 runPipedScans = True
                 while runPipedScans:
@@ -492,25 +504,33 @@
                 removeMonitorFile()
                 sys.exit(0)
             except Exception as e:
                 default_logger().debug(e, exc_info=True)
                 # Probably user cancelled an operation by choosing a cancel sub-menu somewhere
                 pass
             if plainResults is not None and not plainResults.empty:
-                plainResults = plainResults[~plainResults.index.duplicated(keep='first')]
-                results = results[~results.index.duplicated(keep='first')]
+                try:
+                    plainResults.set_index("Stock", inplace=True)
+                except:
+                    pass
+                try:
+                    results.set_index("Stock", inplace=True)
+                except:
+                    pass
+                # plainResults = plainResults[~plainResults.index.duplicated(keep='first')]
+                # results = results[~results.index.duplicated(keep='first')]
                 resultStocks = plainResults.index
             if args.monitor is not None:
                 MarketMonitor().saveMonitorResultStocks(plainResults)
                 if results is not None and len(monitorOption_org) > 0:
                     MarketMonitor().refresh(screen_df=results,screenOptions=monitorOption_org, chosenMenu=updateMenuChoiceHierarchy(),dbTimestamp=f"{dbTimestamp} | CycleTime:{elapsed_time}s",telegram=args.telegram)
 
 
 def pipeResults(prevOutput,args):
-    nextOnes = args.options.split(";")
+    nextOnes = args.options.split(">")
     hasFoundStocks = False
     if len(nextOnes) > 1:
         monitorOption = nextOnes[1]
         if len(monitorOption) == 0:
             return False
         lastComponent = monitorOption.split(":")[-1]
         if "i" in lastComponent:
@@ -526,22 +546,26 @@
             monitorOption = monitorOption.replace("|","")
             monitorOptions = monitorOption.split(":")
             if monitorOptions[1] != "0":
                 monitorOptions[1] = "0"
                 monitorOption = ":".join(monitorOptions)
             # We need to pipe the output from previous run into the next one
             if prevOutput is not None and not prevOutput.empty:
-                prevOutput_results = prevOutput[~prevOutput.index.duplicated(keep='first')]
-                prevOutput_results = prevOutput_results.index
+                try:
+                    prevOutput.set_index("Stock", inplace=True)
+                except:
+                    pass
+                # prevOutput_results = prevOutput[~prevOutput.index.duplicated(keep='first')]
+                prevOutput_results = prevOutput.index
                 hasFoundStocks = len(prevOutput_results) > 0
                 prevOutput_results = ",".join(prevOutput_results)
                 monitorOption = monitorOption.replace(":D:",":")
                 monitorOption = f"{monitorOption}:{prevOutput_results}"
         args.options = monitorOption.replace("::",":")
-        args.options = args.options + ":D:;" + ":D:;".join(nextOnes[2:])
+        args.options = args.options + ":D:>" + ":D:>".join(nextOnes[2:])
         args.options = args.options.replace("::",":")
         return True and hasFoundStocks
     return False
 
 def pkscreenercli():
     global originalStdOut
     if sys.platform.startswith("darwin"):
```

### Comparing `pkscreener-0.44.20240515.376/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240515.377/pkscreener.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240515.376
+Version: 0.44.20240515.377
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240515.376.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240515.377.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.375/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240515.376/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.375/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240515.376/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.375/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240515.376/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240515.376/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240515.377/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240515.376/setup.py` & `pkscreener-0.44.20240515.377/setup.py`

 * *Files identical despite different names*

