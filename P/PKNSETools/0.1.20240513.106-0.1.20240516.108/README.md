# Comparing `tmp/PKNSETools-0.1.20240513.106.tar.gz` & `tmp/PKNSETools-0.1.20240516.108.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PKNSETools-0.1.20240513.106.tar", last modified: Mon May 13 21:56:18 2024, max compression
+gzip compressed data, was "PKNSETools-0.1.20240516.108.tar", last modified: Thu May 16 18:16:50 2024, max compression
```

## Comparing `PKNSETools-0.1.20240513.106.tar` & `PKNSETools-0.1.20240516.108.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 21:56:18.824237 PKNSETools-0.1.20240513.106/
--rw-rw-rw-   0        0        0     2663 2024-05-13 21:56:18.824237 PKNSETools-0.1.20240513.106/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-13 21:56:18.808617 PKNSETools-0.1.20240513.106/PKNSETools/
-drwxrwxrwx   0        0        0        0 2024-05-13 21:56:18.808617 PKNSETools-0.1.20240513.106/PKNSETools/Benny/
--rw-rw-rw-   0        0        0    34274 2024-05-13 21:55:01.000000 PKNSETools-0.1.20240513.106/PKNSETools/Benny/NSE.py
--rw-rw-rw-   0        0        0     1198 2024-05-13 21:55:01.000000 PKNSETools-0.1.20240513.106/PKNSETools/Benny/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 21:56:18.824237 PKNSETools-0.1.20240513.106/PKNSETools/Nasdaq/
--rw-rw-rw-   0        0        0     3386 2024-05-13 21:55:01.000000 PKNSETools-0.1.20240513.106/PKNSETools/Nasdaq/PKNasdaqIndex.py
--rw-rw-rw-   0        0        0     1225 2024-05-13 21:55:01.000000 PKNSETools-0.1.20240513.106/PKNSETools/Nasdaq/__init__.py
--rw-rw-rw-   0        0        0     4806 2024-05-13 21:55:01.000000 PKNSETools-0.1.20240513.106/PKNSETools/PKAllStocks.py
--rw-rw-rw-   0        0        0    10770 2024-05-13 21:55:01.000000 PKNSETools-0.1.20240513.106/PKNSETools/PKCompanyGeneral.py
--rw-rw-rw-   0        0        0     3303 2024-05-13 21:55:01.000000 PKNSETools-0.1.20240513.106/PKNSETools/PKCompanyStock.py
--rw-rw-rw-   0        0        0     2635 2024-05-13 21:55:01.000000 PKNSETools-0.1.20240513.106/PKNSETools/PKConstants.py
--rw-rw-rw-   0        0        0    10388 2024-05-13 21:55:01.000000 PKNSETools-0.1.20240513.106/PKNSETools/PKIntraDay.py
--rw-rw-rw-   0        0        0    13849 2024-05-13 21:55:01.000000 PKNSETools-0.1.20240513.106/PKNSETools/PKNSEStockDataFetcher.py
--rw-rw-rw-   0        0        0       31 2024-05-13 21:56:14.000000 PKNSETools-0.1.20240513.106/PKNSETools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 21:56:18.824237 PKNSETools-0.1.20240513.106/PKNSETools/morningstartools/
--rw-rw-rw-   0        0        0     1830 2024-05-13 21:55:01.000000 PKNSETools-0.1.20240513.106/PKNSETools/morningstartools/NSEStockDB.py
--rw-rw-rw-   0        0        0     1848 2024-05-13 21:55:01.000000 PKNSETools-0.1.20240513.106/PKNSETools/morningstartools/NSEStockFairValueDB.py
--rw-rw-rw-   0        0        0     1836 2024-05-13 21:55:01.000000 PKNSETools-0.1.20240513.106/PKNSETools/morningstartools/NSEStockMFIDB.py
--rw-rw-rw-   0        0        0    61961 2024-05-13 21:55:01.000000 PKNSETools-0.1.20240513.106/PKNSETools/morningstartools/PKMorningstarDataFetcher.py
--rw-rw-rw-   0        0        0     1378 2024-05-13 21:55:01.000000 PKNSETools-0.1.20240513.106/PKNSETools/morningstartools/__init__.py
--rw-rw-rw-   0        0        0     2000 2024-05-13 21:55:01.000000 PKNSETools-0.1.20240513.106/PKNSETools/morningstartools/error.py
--rw-rw-rw-   0        0        0    40060 2024-05-13 21:55:01.000000 PKNSETools-0.1.20240513.106/PKNSETools/morningstartools/funds.py
--rw-rw-rw-   0        0        0    22038 2024-05-13 21:55:01.000000 PKNSETools-0.1.20240513.106/PKNSETools/morningstartools/search.py
--rw-rw-rw-   0        0        0    13495 2024-05-13 21:55:01.000000 PKNSETools-0.1.20240513.106/PKNSETools/morningstartools/security.py
--rw-rw-rw-   0        0        0    29916 2024-05-13 21:55:01.000000 PKNSETools-0.1.20240513.106/PKNSETools/morningstartools/stock.py
--rw-rw-rw-   0        0        0    23246 2024-05-13 21:55:01.000000 PKNSETools-0.1.20240513.106/PKNSETools/morningstartools/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-13 21:56:18.808617 PKNSETools-0.1.20240513.106/PKNSETools.egg-info/
--rw-rw-rw-   0        0        0     2663 2024-05-13 21:56:18.000000 PKNSETools-0.1.20240513.106/PKNSETools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1004 2024-05-13 21:56:18.000000 PKNSETools-0.1.20240513.106/PKNSETools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 21:56:18.000000 PKNSETools-0.1.20240513.106/PKNSETools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-13 21:56:12.000000 PKNSETools-0.1.20240513.106/PKNSETools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       79 2024-05-13 21:56:18.000000 PKNSETools-0.1.20240513.106/PKNSETools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-13 21:56:18.000000 PKNSETools-0.1.20240513.106/PKNSETools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1884 2024-05-13 21:55:01.000000 PKNSETools-0.1.20240513.106/README.md
--rw-rw-rw-   0        0        0       86 2024-05-13 21:56:18.824237 PKNSETools-0.1.20240513.106/setup.cfg
--rw-rw-rw-   0        0        0     3832 2024-05-13 21:55:01.000000 PKNSETools-0.1.20240513.106/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 18:16:50.546068 PKNSETools-0.1.20240516.108/
+-rw-rw-rw-   0        0        0     2663 2024-05-16 18:16:50.546068 PKNSETools-0.1.20240516.108/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-16 18:16:50.530445 PKNSETools-0.1.20240516.108/PKNSETools/
+drwxrwxrwx   0        0        0        0 2024-05-16 18:16:50.546068 PKNSETools-0.1.20240516.108/PKNSETools/Benny/
+-rw-rw-rw-   0        0        0    34274 2024-05-16 18:15:04.000000 PKNSETools-0.1.20240516.108/PKNSETools/Benny/NSE.py
+-rw-rw-rw-   0        0        0     1198 2024-05-16 18:15:04.000000 PKNSETools-0.1.20240516.108/PKNSETools/Benny/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 18:16:50.546068 PKNSETools-0.1.20240516.108/PKNSETools/Nasdaq/
+-rw-rw-rw-   0        0        0     3386 2024-05-16 18:15:04.000000 PKNSETools-0.1.20240516.108/PKNSETools/Nasdaq/PKNasdaqIndex.py
+-rw-rw-rw-   0        0        0     1225 2024-05-16 18:15:04.000000 PKNSETools-0.1.20240516.108/PKNSETools/Nasdaq/__init__.py
+-rw-rw-rw-   0        0        0     4806 2024-05-16 18:15:04.000000 PKNSETools-0.1.20240516.108/PKNSETools/PKAllStocks.py
+-rw-rw-rw-   0        0        0    10770 2024-05-16 18:15:04.000000 PKNSETools-0.1.20240516.108/PKNSETools/PKCompanyGeneral.py
+-rw-rw-rw-   0        0        0     3303 2024-05-16 18:15:04.000000 PKNSETools-0.1.20240516.108/PKNSETools/PKCompanyStock.py
+-rw-rw-rw-   0        0        0     2635 2024-05-16 18:15:04.000000 PKNSETools-0.1.20240516.108/PKNSETools/PKConstants.py
+-rw-rw-rw-   0        0        0    10388 2024-05-16 18:15:04.000000 PKNSETools-0.1.20240516.108/PKNSETools/PKIntraDay.py
+-rw-rw-rw-   0        0        0    16561 2024-05-16 18:15:04.000000 PKNSETools-0.1.20240516.108/PKNSETools/PKNSEStockDataFetcher.py
+-rw-rw-rw-   0        0        0       31 2024-05-16 18:16:45.000000 PKNSETools-0.1.20240516.108/PKNSETools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 18:16:50.546068 PKNSETools-0.1.20240516.108/PKNSETools/morningstartools/
+-rw-rw-rw-   0        0        0     1830 2024-05-16 18:15:04.000000 PKNSETools-0.1.20240516.108/PKNSETools/morningstartools/NSEStockDB.py
+-rw-rw-rw-   0        0        0     1848 2024-05-16 18:15:04.000000 PKNSETools-0.1.20240516.108/PKNSETools/morningstartools/NSEStockFairValueDB.py
+-rw-rw-rw-   0        0        0     1836 2024-05-16 18:15:04.000000 PKNSETools-0.1.20240516.108/PKNSETools/morningstartools/NSEStockMFIDB.py
+-rw-rw-rw-   0        0        0    61961 2024-05-16 18:15:04.000000 PKNSETools-0.1.20240516.108/PKNSETools/morningstartools/PKMorningstarDataFetcher.py
+-rw-rw-rw-   0        0        0     1378 2024-05-16 18:15:04.000000 PKNSETools-0.1.20240516.108/PKNSETools/morningstartools/__init__.py
+-rw-rw-rw-   0        0        0     2000 2024-05-16 18:15:04.000000 PKNSETools-0.1.20240516.108/PKNSETools/morningstartools/error.py
+-rw-rw-rw-   0        0        0    40060 2024-05-16 18:15:04.000000 PKNSETools-0.1.20240516.108/PKNSETools/morningstartools/funds.py
+-rw-rw-rw-   0        0        0    22038 2024-05-16 18:15:04.000000 PKNSETools-0.1.20240516.108/PKNSETools/morningstartools/search.py
+-rw-rw-rw-   0        0        0    13495 2024-05-16 18:15:04.000000 PKNSETools-0.1.20240516.108/PKNSETools/morningstartools/security.py
+-rw-rw-rw-   0        0        0    29916 2024-05-16 18:15:04.000000 PKNSETools-0.1.20240516.108/PKNSETools/morningstartools/stock.py
+-rw-rw-rw-   0        0        0    23246 2024-05-16 18:15:04.000000 PKNSETools-0.1.20240516.108/PKNSETools/morningstartools/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-16 18:16:50.546068 PKNSETools-0.1.20240516.108/PKNSETools.egg-info/
+-rw-rw-rw-   0        0        0     2663 2024-05-16 18:16:50.000000 PKNSETools-0.1.20240516.108/PKNSETools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1004 2024-05-16 18:16:50.000000 PKNSETools-0.1.20240516.108/PKNSETools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 18:16:50.000000 PKNSETools-0.1.20240516.108/PKNSETools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-16 18:16:43.000000 PKNSETools-0.1.20240516.108/PKNSETools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       79 2024-05-16 18:16:50.000000 PKNSETools-0.1.20240516.108/PKNSETools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-16 18:16:50.000000 PKNSETools-0.1.20240516.108/PKNSETools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1884 2024-05-16 18:15:04.000000 PKNSETools-0.1.20240516.108/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-16 18:16:50.546068 PKNSETools-0.1.20240516.108/setup.cfg
+-rw-rw-rw-   0        0        0     3832 2024-05-16 18:15:04.000000 PKNSETools-0.1.20240516.108/setup.py
```

### Comparing `PKNSETools-0.1.20240513.106/PKG-INFO` & `PKNSETools-0.1.20240516.108/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKNSETools
-Version: 0.1.20240513.106
+Version: 0.1.20240516.108
 Summary: A Python-based data downloader for NSE, India
 Home-page: https://github.com/pkjmesra/PKNSETools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240513.106.zip
+Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240516.108.zip
 Keywords: NSE,Stocks,Data Download
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKNSETools-0.1.20240513.106/PKNSETools/Benny/NSE.py` & `PKNSETools-0.1.20240516.108/PKNSETools/Benny/NSE.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240513.106/PKNSETools/Benny/__init__.py` & `PKNSETools-0.1.20240516.108/PKNSETools/Benny/__init__.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240513.106/PKNSETools/Nasdaq/PKNasdaqIndex.py` & `PKNSETools-0.1.20240516.108/PKNSETools/Nasdaq/PKNasdaqIndex.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240513.106/PKNSETools/Nasdaq/__init__.py` & `PKNSETools-0.1.20240516.108/PKNSETools/Nasdaq/__init__.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240513.106/PKNSETools/PKAllStocks.py` & `PKNSETools-0.1.20240516.108/PKNSETools/PKAllStocks.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240513.106/PKNSETools/PKCompanyGeneral.py` & `PKNSETools-0.1.20240516.108/PKNSETools/PKCompanyGeneral.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240513.106/PKNSETools/PKCompanyStock.py` & `PKNSETools-0.1.20240516.108/PKNSETools/PKCompanyStock.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240513.106/PKNSETools/PKConstants.py` & `PKNSETools-0.1.20240516.108/PKNSETools/PKConstants.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240513.106/PKNSETools/PKIntraDay.py` & `PKNSETools-0.1.20240516.108/PKNSETools/PKIntraDay.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240513.106/PKNSETools/PKNSEStockDataFetcher.py` & `PKNSETools-0.1.20240516.108/PKNSETools/PKNSEStockDataFetcher.py`

 * *Files 18% similar despite different names*

```diff
@@ -39,67 +39,105 @@
 from PKDevTools.classes.Fetcher import fetcher
 from PKDevTools.classes.log import default_logger
 from PKDevTools.classes.OutputControls import OutputControls
 
 from PKNSETools.Benny.NSE import NSE
 from PKDevTools.classes.Utils import random_user_agent
 
+NSE_INDEX_MAP = {
+    1: "https://archives.nseindia.com/content/indices/ind_nifty50list.csv",
+    2: "https://archives.nseindia.com/content/indices/ind_niftynext50list.csv",
+    3: "https://archives.nseindia.com/content/indices/ind_nifty100list.csv",
+    4: "https://archives.nseindia.com/content/indices/ind_nifty200list.csv",
+    5: "https://archives.nseindia.com/content/indices/ind_nifty500list.csv",
+    6: "https://archives.nseindia.com/content/indices/ind_niftysmallcap50list.csv",
+    7: "https://archives.nseindia.com/content/indices/ind_niftysmallcap100list.csv",
+    8: "https://archives.nseindia.com/content/indices/ind_niftysmallcap250list.csv",
+    9: "https://archives.nseindia.com/content/indices/ind_niftymidcap50list.csv",
+    10: "https://archives.nseindia.com/content/indices/ind_niftymidcap100list.csv",
+    11: "https://archives.nseindia.com/content/indices/ind_niftymidcap150list.csv",
+    12: "https://archives.nseindia.com/content/equities/EQUITY_L.csv",
+    14: "https://archives.nseindia.com/content/fo/fo_mktlots.csv",
+}
+REPO_INDEX_MAP = {
+    1: "https://raw.githubusercontent.com/pkjmesra/PKScreener/main/results/ind_nifty50list.csv",
+    2: "https://raw.githubusercontent.com/pkjmesra/PKScreener/main/results/ind_niftynext50list.csv",
+    3: "https://raw.githubusercontent.com/pkjmesra/PKScreener/main/results/ind_nifty100list.csv",
+    4: "https://raw.githubusercontent.com/pkjmesra/PKScreener/main/results/ind_nifty200list.csv",
+    5: "https://raw.githubusercontent.com/pkjmesra/PKScreener/main/results/ind_nifty500list.csv",
+    6: "https://raw.githubusercontent.com/pkjmesra/PKScreener/main/results/ind_niftysmallcap50list.csv",
+    7: "https://raw.githubusercontent.com/pkjmesra/PKScreener/main/results/ind_niftysmallcap100list.csv",
+    8: "https://raw.githubusercontent.com/pkjmesra/PKScreener/main/results/ind_niftysmallcap250list.csv",
+    9: "https://raw.githubusercontent.com/pkjmesra/PKScreener/main/results/ind_niftymidcap50list.csv",
+    10: "https://raw.githubusercontent.com/pkjmesra/PKScreener/main/results/ind_niftymidcap100list.csv",
+    11: "https://raw.githubusercontent.com/pkjmesra/PKScreener/main/results/ind_niftymidcap150list.csv",
+    12: "https://raw.githubusercontent.com/pkjmesra/PKScreener/main/results/EQUITY_L.csv",
+    14: "https://archives.nseindia.com/content/fo/fo_mktlots.csv",
+}
+
 # This Class Handles Fetching of Stock Data over the internet from NSE/BSE
 
 class nseStockDataFetcher(fetcher):
 
+    def savedFileContents(self, fileName=None):
+        data, filePath, modifiedDateTime = Archiver.findFileInAppResultsDirectory(fileName=fileName)
+        return data, filePath, modifiedDateTime
+
+    def fetchFileFromHostServer(self,filePath,tickerOption,fileContents,indexMap=NSE_INDEX_MAP):
+        try:
+            url = indexMap.get(tickerOption)
+            fileName = url.split("/")[-1]
+            headers = {"user-agent": random_user_agent()}
+            res = self.fetchURL(url,headers=headers,timeout=10)
+            if res is None or res.status_code != 200:
+                default_logger().debug(f"Response for tickerOption:{tickerOption}, file:{fileName}: {res}")
+            else:
+                fileContents = res.text
+                with open(filePath, "w") as f:
+                    f.write(fileContents)
+        except:
+            pass
+        return fileContents
+
     def fetchNiftyCodes(self, tickerOption):
         listStockCodes = []
-        if tickerOption == 12:
-            url = "https://archives.nseindia.com/content/equities/EQUITY_L.csv"
-            res = self.fetchURL(url)
-            if res is None or res.status_code != 200:
+        url = NSE_INDEX_MAP.get(tickerOption)
+        fileName = url.split("/")[-1]
+        fileContents, filePath, modifiedDateTime = self.savedFileContents(fileName)
+        shouldFetch = fileContents is None or (fileContents is not None and PKDateUtilities.currentDateTime().date() > modifiedDateTime.date())
+        OutputControls().printOutput(colorText.BOLD + f"[+] {(len(fileContents.splitlines())-1) if fileContents is not None else 0} stocks loaded from local cache. {'Getting Stock Codes From NSE...' if shouldFetch else ''}")
+        if shouldFetch:
+            fileContents = self.fetchFileFromHostServer(filePath,tickerOption,fileContents)
+        if fileContents is None:
+            # Try and get it from our own repo
+            fileContents = self.fetchFileFromHostServer(filePath,tickerOption,fileContents,REPO_INDEX_MAP)
+            if fileContents is None:
                 return listStockCodes
+
+        if tickerOption == 12:
             try:
-                data = pd.read_csv(StringIO(res.text))
+                data = pd.read_csv(StringIO(fileContents))
                 return list(data["SYMBOL"].values)
             except Exception as e:
                 default_logger().debug(e, exc_info=True)
                 return listStockCodes
-            
-        tickerMapping = {
-            1: "https://archives.nseindia.com/content/indices/ind_nifty50list.csv",
-            2: "https://archives.nseindia.com/content/indices/ind_niftynext50list.csv",
-            3: "https://archives.nseindia.com/content/indices/ind_nifty100list.csv",
-            4: "https://archives.nseindia.com/content/indices/ind_nifty200list.csv",
-            5: "https://archives.nseindia.com/content/indices/ind_nifty500list.csv",
-            6: "https://archives.nseindia.com/content/indices/ind_niftysmallcap50list.csv",
-            7: "https://archives.nseindia.com/content/indices/ind_niftysmallcap100list.csv",
-            8: "https://archives.nseindia.com/content/indices/ind_niftysmallcap250list.csv",
-            9: "https://archives.nseindia.com/content/indices/ind_niftymidcap50list.csv",
-            10: "https://archives.nseindia.com/content/indices/ind_niftymidcap100list.csv",
-            11: "https://archives.nseindia.com/content/indices/ind_niftymidcap150list.csv",
-            14: "https://archives.nseindia.com/content/fo/fo_mktlots.csv",
-        }
-
-        url = tickerMapping.get(tickerOption)
-
         try:
-            headers = {"user-agent": random_user_agent()}
-            res = self.fetchURL(url,headers=headers,timeout=10)
-            if res is None or res.status_code != 200:
-                return listStockCodes
-            cr = csv.reader(res.text.strip().split("\n"))
-
+            cr = csv.reader(fileContents.strip().split("\n"))
             if tickerOption == 14:
                 for i in range(5):
                     next(cr)  # skipping first line
                 for row in cr:
                     listStockCodes.append(row[1])
             else:
                 next(cr)  # skipping first line
                 for row in cr:
                     listStockCodes.append(row[2])
         except Exception as e:
             default_logger().debug(e, exc_info=True)
+            pass
 
         return listStockCodes
 
     # Fetch all stock codes from NSE
     def fetchStockCodes(self, tickerOption, stockCode=None):
         listStockCodes = []
         if tickerOption == 0:
@@ -111,15 +149,14 @@
                         + colorText.FAIL
                         + "[+] Enter Stock Code(s) for screening (Multiple codes should be seperated by ,): "
                     )
                 ).upper()
             stockCode = stockCode.replace(" ", "")
             listStockCodes = stockCode.split(",")
         else:
-            OutputControls().printOutput(colorText.BOLD + "[+] Getting Stock Codes From NSE... ")
             listStockCodes = self.fetchNiftyCodes(tickerOption)
             if len(listStockCodes) > 10:
                 OutputControls().printOutput(
                     colorText.GREEN
                     + ("=> Done! Fetched %d stock codes." % len(listStockCodes))
                     + colorText.END
                 )
@@ -252,30 +289,35 @@
             pass
         now = PKDateUtilities.currentDateTime().astimezone(tz=pytz.timezone(tzName))
         ts = datetime.datetime.timestamp(now)
         now = pd.to_datetime(ts, unit='s', utc=True).tz_convert(tzName)
         # isClosed = now < todayOpen and now < todayClose
         isOpen = now >= todayOpen and todayClose >= now
         status = "Open" if isOpen else "Closed"
-        lastPrice = round(basicInfo["last_price"],2)
-        prevClose = round(basicInfo["regular_market_previous_close"],2)
-        if not pd.notna(prevClose):
-            prevClose = md["previousClose"] if "previousClose" in md.keys() else prevClose
+        marketStatusLong = ""
+        tradeDate = ""
+        try:
+            lastPrice = round(basicInfo["last_price"],2)
+            prevClose = round(basicInfo["regular_market_previous_close"],2)
             if not pd.notna(prevClose):
-                prevClose = info["previousClose"] if "previousClose" in info.keys() else prevClose
+                prevClose = md["previousClose"] if "previousClose" in md.keys() else prevClose
                 if not pd.notna(prevClose):
-                    prevClose = info["regularMarketPreviousClose"] if "regularMarketPreviousClose" in info.keys() else prevClose
-        change = round(lastPrice - prevClose,2)
-        pctChange = round(100*change/prevClose,2)
-        tradeDate = lastTradeDate.strftime("%Y-%m-%d")
-        
-        if len(status) > 0:
-            change = ((colorText.GREEN +"▲")if change >=0 else colorText.FAIL+"▼") + str(change if pd.notna(change) else "?") + colorText.END
-            pctChange = (colorText.GREEN if pctChange >=0 else colorText.FAIL) + str(pctChange if pd.notna(pctChange) else "?") + colorText.END
-            marketStatusLong = f'{info["longName"]} | {status} | {tradeDate} | {lastPrice} | {change} ({pctChange}%)'
+                    prevClose = info["previousClose"] if "previousClose" in info.keys() else prevClose
+                    if not pd.notna(prevClose):
+                        prevClose = info["regularMarketPreviousClose"] if "regularMarketPreviousClose" in info.keys() else prevClose
+            change = round(lastPrice - prevClose,2)
+            pctChange = round(100*change/prevClose,2)
+            tradeDate = lastTradeDate.strftime("%Y-%m-%d")
+            
+            if len(status) > 0:
+                change = ((colorText.GREEN +"▲")if change >=0 else colorText.FAIL+"▼") + str(change if pd.notna(change) else "?") + colorText.END
+                pctChange = (colorText.GREEN if pctChange >=0 else colorText.FAIL) + str(pctChange if pd.notna(pctChange) else "?") + colorText.END
+                marketStatusLong = f'{info["longName"]} | {status} | {tradeDate} | {lastPrice} | {change} ({pctChange}%)'
+        except:
+            pass
         return status, marketStatusLong,tradeDate
 
 # f = nseStockDataFetcher()
 # f.capitalMarketStatus(exchange="^NSEI")
 
 
 # from yfinhanced import YFClient
```

### Comparing `PKNSETools-0.1.20240513.106/PKNSETools/morningstartools/NSEStockDB.py` & `PKNSETools-0.1.20240516.108/PKNSETools/morningstartools/NSEStockDB.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240513.106/PKNSETools/morningstartools/NSEStockFairValueDB.py` & `PKNSETools-0.1.20240516.108/PKNSETools/morningstartools/NSEStockFairValueDB.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240513.106/PKNSETools/morningstartools/NSEStockMFIDB.py` & `PKNSETools-0.1.20240516.108/PKNSETools/morningstartools/NSEStockMFIDB.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240513.106/PKNSETools/morningstartools/PKMorningstarDataFetcher.py` & `PKNSETools-0.1.20240516.108/PKNSETools/morningstartools/PKMorningstarDataFetcher.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240513.106/PKNSETools/morningstartools/__init__.py` & `PKNSETools-0.1.20240516.108/PKNSETools/morningstartools/__init__.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240513.106/PKNSETools/morningstartools/error.py` & `PKNSETools-0.1.20240516.108/PKNSETools/morningstartools/error.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240513.106/PKNSETools/morningstartools/funds.py` & `PKNSETools-0.1.20240516.108/PKNSETools/morningstartools/funds.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240513.106/PKNSETools/morningstartools/search.py` & `PKNSETools-0.1.20240516.108/PKNSETools/morningstartools/search.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240513.106/PKNSETools/morningstartools/security.py` & `PKNSETools-0.1.20240516.108/PKNSETools/morningstartools/security.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240513.106/PKNSETools/morningstartools/stock.py` & `PKNSETools-0.1.20240516.108/PKNSETools/morningstartools/stock.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240513.106/PKNSETools/morningstartools/utils.py` & `PKNSETools-0.1.20240516.108/PKNSETools/morningstartools/utils.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240513.106/PKNSETools.egg-info/PKG-INFO` & `PKNSETools-0.1.20240516.108/PKNSETools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKNSETools
-Version: 0.1.20240513.106
+Version: 0.1.20240516.108
 Summary: A Python-based data downloader for NSE, India
 Home-page: https://github.com/pkjmesra/PKNSETools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240513.106.zip
+Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240516.108.zip
 Keywords: NSE,Stocks,Data Download
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKNSETools-0.1.20240513.106/PKNSETools.egg-info/SOURCES.txt` & `PKNSETools-0.1.20240516.108/PKNSETools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240513.106/README.md` & `PKNSETools-0.1.20240516.108/README.md`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240513.106/setup.py` & `PKNSETools-0.1.20240516.108/setup.py`

 * *Files identical despite different names*

