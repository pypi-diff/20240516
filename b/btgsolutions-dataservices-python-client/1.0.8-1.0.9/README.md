# Comparing `tmp/btgsolutions-dataservices-python-client-1.0.8.tar.gz` & `tmp/btgsolutions-dataservices-python-client-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btgsolutions-dataservices-python-client-1.0.8.tar", last modified: Fri Feb 23 21:35:12 2024, max compression
+gzip compressed data, was "btgsolutions-dataservices-python-client-1.0.9.tar", last modified: Fri Mar 15 19:38:15 2024, max compression
```

## Comparing `btgsolutions-dataservices-python-client-1.0.8.tar` & `btgsolutions-dataservices-python-client-1.0.9.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-02-23 21:35:12.607536 btgsolutions-dataservices-python-client-1.0.8/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1057 2023-10-16 17:42:51.000000 btgsolutions-dataservices-python-client-1.0.8/LICENSE
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       24 2023-10-16 17:42:51.000000 btgsolutions-dataservices-python-client-1.0.8/MANIFEST.in
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     7153 2024-02-23 21:35:12.603536 btgsolutions-dataservices-python-client-1.0.8/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6727 2024-02-23 21:34:05.000000 btgsolutions-dataservices-python-client-1.0.8/README.md
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-02-23 21:35:12.599536 btgsolutions-dataservices-python-client-1.0.8/btgsolutions_dataservices/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       93 2023-10-16 17:42:51.000000 btgsolutions-dataservices-python-client-1.0.8/btgsolutions_dataservices/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     5542 2024-01-22 20:24:39.000000 btgsolutions-dataservices-python-client-1.0.8/btgsolutions_dataservices/config.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      599 2023-10-16 17:42:51.000000 btgsolutions-dataservices-python-client-1.0.8/btgsolutions_dataservices/exceptions.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-02-23 21:35:12.603536 btgsolutions-dataservices-python-client-1.0.8/btgsolutions_dataservices/rest/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      279 2023-10-16 17:42:51.000000 btgsolutions-dataservices-python-client-1.0.8/btgsolutions_dataservices/rest/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1363 2023-10-16 20:18:29.000000 btgsolutions-dataservices-python-client-1.0.8/btgsolutions_dataservices/rest/authenticator.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     8188 2024-02-23 20:56:22.000000 btgsolutions-dataservices-python-client-1.0.8/btgsolutions_dataservices/rest/bulk_data.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    11205 2023-10-16 20:18:29.000000 btgsolutions-dataservices-python-client-1.0.8/btgsolutions_dataservices/rest/hfn.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6203 2023-10-23 19:02:30.000000 btgsolutions-dataservices-python-client-1.0.8/btgsolutions_dataservices/rest/historical_candles.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     5752 2023-10-16 20:18:29.000000 btgsolutions-dataservices-python-client-1.0.8/btgsolutions_dataservices/rest/intraday_candles.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1866 2023-10-16 17:42:51.000000 btgsolutions-dataservices-python-client-1.0.8/btgsolutions_dataservices/rest/intraday_tick_data.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7508 2023-10-16 20:18:29.000000 btgsolutions-dataservices-python-client-1.0.8/btgsolutions_dataservices/rest/quotes.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-02-23 21:35:12.603536 btgsolutions-dataservices-python-client-1.0.8/btgsolutions_dataservices/websocket/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      120 2024-01-22 20:24:39.000000 btgsolutions-dataservices-python-client-1.0.8/btgsolutions_dataservices/websocket/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6253 2024-01-22 20:24:39.000000 btgsolutions-dataservices-python-client-1.0.8/btgsolutions_dataservices/websocket/hfn_websocket_client.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    11056 2024-01-22 20:24:39.000000 btgsolutions-dataservices-python-client-1.0.8/btgsolutions_dataservices/websocket/market_data_websocket_client.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      270 2023-10-16 17:42:51.000000 btgsolutions-dataservices-python-client-1.0.8/btgsolutions_dataservices/websocket/websocket_default_functions.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-02-23 21:35:12.603536 btgsolutions-dataservices-python-client-1.0.8/btgsolutions_dataservices_python_client.egg-info/
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     7153 2024-02-23 21:35:12.000000 btgsolutions-dataservices-python-client-1.0.8/btgsolutions_dataservices_python_client.egg-info/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1097 2024-02-23 21:35:12.000000 btgsolutions-dataservices-python-client-1.0.8/btgsolutions_dataservices_python_client.egg-info/SOURCES.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2024-02-23 21:35:12.000000 btgsolutions-dataservices-python-client-1.0.8/btgsolutions_dataservices_python_client.egg-info/dependency_links.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      110 2024-02-23 21:35:12.000000 btgsolutions-dataservices-python-client-1.0.8/btgsolutions_dataservices_python_client.egg-info/requires.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       26 2024-02-23 21:35:12.000000 btgsolutions-dataservices-python-client-1.0.8/btgsolutions_dataservices_python_client.egg-info/top_level.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      109 2024-01-22 20:24:39.000000 btgsolutions-dataservices-python-client-1.0.8/requirements.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2024-02-23 21:35:12.607536 btgsolutions-dataservices-python-client-1.0.8/setup.cfg
--rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     1272 2024-02-23 21:34:35.000000 btgsolutions-dataservices-python-client-1.0.8/setup.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-03-15 19:38:15.982653 btgsolutions-dataservices-python-client-1.0.9/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1057 2023-09-15 01:09:18.000000 btgsolutions-dataservices-python-client-1.0.9/LICENSE
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       24 2023-09-15 01:09:18.000000 btgsolutions-dataservices-python-client-1.0.9/MANIFEST.in
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     7357 2024-03-15 19:38:15.982653 btgsolutions-dataservices-python-client-1.0.9/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6939 2024-03-15 19:24:02.000000 btgsolutions-dataservices-python-client-1.0.9/README.md
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-03-15 19:38:15.978653 btgsolutions-dataservices-python-client-1.0.9/btgsolutions_dataservices/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       93 2023-11-30 22:44:50.000000 btgsolutions-dataservices-python-client-1.0.9/btgsolutions_dataservices/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     5542 2024-01-11 14:50:37.000000 btgsolutions-dataservices-python-client-1.0.9/btgsolutions_dataservices/config.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      599 2023-09-15 01:09:18.000000 btgsolutions-dataservices-python-client-1.0.9/btgsolutions_dataservices/exceptions.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-03-15 19:38:15.978653 btgsolutions-dataservices-python-client-1.0.9/btgsolutions_dataservices/rest/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      326 2024-03-15 19:29:50.000000 btgsolutions-dataservices-python-client-1.0.9/btgsolutions_dataservices/rest/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1363 2023-09-15 01:09:18.000000 btgsolutions-dataservices-python-client-1.0.9/btgsolutions_dataservices/rest/authenticator.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     8188 2024-03-05 15:06:36.000000 btgsolutions-dataservices-python-client-1.0.9/btgsolutions_dataservices/rest/bulk_data.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    11205 2023-09-15 16:33:08.000000 btgsolutions-dataservices-python-client-1.0.9/btgsolutions_dataservices/rest/hfn.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6203 2023-10-25 13:32:35.000000 btgsolutions-dataservices-python-client-1.0.9/btgsolutions_dataservices/rest/historical_candles.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     5752 2023-09-15 01:09:18.000000 btgsolutions-dataservices-python-client-1.0.9/btgsolutions_dataservices/rest/intraday_candles.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1866 2023-09-21 20:14:41.000000 btgsolutions-dataservices-python-client-1.0.9/btgsolutions_dataservices/rest/intraday_tick_data.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7508 2023-12-13 19:27:18.000000 btgsolutions-dataservices-python-client-1.0.9/btgsolutions_dataservices/rest/quotes.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2950 2024-03-15 19:32:07.000000 btgsolutions-dataservices-python-client-1.0.9/btgsolutions_dataservices/rest/ticker_last_event.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-03-15 19:38:15.978653 btgsolutions-dataservices-python-client-1.0.9/btgsolutions_dataservices/websocket/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      120 2023-12-01 05:20:40.000000 btgsolutions-dataservices-python-client-1.0.9/btgsolutions_dataservices/websocket/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6253 2024-01-11 15:05:42.000000 btgsolutions-dataservices-python-client-1.0.9/btgsolutions_dataservices/websocket/hfn_websocket_client.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    11056 2024-01-11 15:04:41.000000 btgsolutions-dataservices-python-client-1.0.9/btgsolutions_dataservices/websocket/market_data_websocket_client.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      270 2023-09-15 01:09:18.000000 btgsolutions-dataservices-python-client-1.0.9/btgsolutions_dataservices/websocket/websocket_default_functions.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-03-15 19:38:15.982653 btgsolutions-dataservices-python-client-1.0.9/btgsolutions_dataservices_python_client.egg-info/
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     7357 2024-03-15 19:38:15.000000 btgsolutions-dataservices-python-client-1.0.9/btgsolutions_dataservices_python_client.egg-info/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1149 2024-03-15 19:38:15.000000 btgsolutions-dataservices-python-client-1.0.9/btgsolutions_dataservices_python_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2024-03-15 19:38:15.000000 btgsolutions-dataservices-python-client-1.0.9/btgsolutions_dataservices_python_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      110 2024-03-15 19:38:15.000000 btgsolutions-dataservices-python-client-1.0.9/btgsolutions_dataservices_python_client.egg-info/requires.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       26 2024-03-15 19:38:15.000000 btgsolutions-dataservices-python-client-1.0.9/btgsolutions_dataservices_python_client.egg-info/top_level.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      109 2023-12-13 19:00:19.000000 btgsolutions-dataservices-python-client-1.0.9/requirements.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2024-03-15 19:38:15.982653 btgsolutions-dataservices-python-client-1.0.9/setup.cfg
+-rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     1272 2024-03-15 19:28:49.000000 btgsolutions-dataservices-python-client-1.0.9/setup.py
```

### Comparing `btgsolutions-dataservices-python-client-1.0.8/LICENSE` & `btgsolutions-dataservices-python-client-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `btgsolutions-dataservices-python-client-1.0.8/PKG-INFO` & `btgsolutions-dataservices-python-client-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btgsolutions-dataservices-python-client
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python package containing several classes and data for extracting and manipulating market and trading data.
 Home-page: https://github.com/BTG-Pactual-Solutions/btgsolutions-dataservices-python-client
 Author: BTG Solutions Data Services powered by BTG Pactual Solutions
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas<2.0,>=1.3.5
@@ -165,14 +165,22 @@
 
 ```python
 import btgsolutions_dataservices as btg
 quotes = btg.Quotes(api_key='YOUR_API_KEY')
 quotes.get_quote(market_type = 'stocks', tickers = ['PETR4', 'VALE3'])
 ```
 
+## Example - Ticker Last Event
+
+```python
+import btgsolutions_dataservices as btg
+last_event = btg.TickerLastEvent(api_key='YOUR_API_KEY')
+last_event.get_trades(data_type='equities', ticker='VALE3')
+```
+
 ## Example BulkData - Available Tickers
 ```python
 import btgsolutions_dataservices as btg
 bulk_data = btg.BulkData(api_key='YOUR_API_KEY')
 bulk_data.get_available_tickers(date='2023-07-03', data_type='trades', prefix='PETR')
 ```
```

### Comparing `btgsolutions-dataservices-python-client-1.0.8/README.md` & `btgsolutions-dataservices-python-client-1.0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -150,14 +150,22 @@
 
 ```python
 import btgsolutions_dataservices as btg
 quotes = btg.Quotes(api_key='YOUR_API_KEY')
 quotes.get_quote(market_type = 'stocks', tickers = ['PETR4', 'VALE3'])
 ```
 
+## Example - Ticker Last Event
+
+```python
+import btgsolutions_dataservices as btg
+last_event = btg.TickerLastEvent(api_key='YOUR_API_KEY')
+last_event.get_trades(data_type='equities', ticker='VALE3')
+```
+
 ## Example BulkData - Available Tickers
 ```python
 import btgsolutions_dataservices as btg
 bulk_data = btg.BulkData(api_key='YOUR_API_KEY')
 bulk_data.get_available_tickers(date='2023-07-03', data_type='trades', prefix='PETR')
 ```
```

### Comparing `btgsolutions-dataservices-python-client-1.0.8/btgsolutions_dataservices/config.py` & `btgsolutions-dataservices-python-client-1.0.9/btgsolutions_dataservices/config.py`

 * *Files identical despite different names*

### Comparing `btgsolutions-dataservices-python-client-1.0.8/btgsolutions_dataservices/exceptions.py` & `btgsolutions-dataservices-python-client-1.0.9/btgsolutions_dataservices/exceptions.py`

 * *Files identical despite different names*

### Comparing `btgsolutions-dataservices-python-client-1.0.8/btgsolutions_dataservices/rest/authenticator.py` & `btgsolutions-dataservices-python-client-1.0.9/btgsolutions_dataservices/rest/authenticator.py`

 * *Files identical despite different names*

### Comparing `btgsolutions-dataservices-python-client-1.0.8/btgsolutions_dataservices/rest/bulk_data.py` & `btgsolutions-dataservices-python-client-1.0.9/btgsolutions_dataservices/rest/bulk_data.py`

 * *Files identical despite different names*

### Comparing `btgsolutions-dataservices-python-client-1.0.8/btgsolutions_dataservices/rest/hfn.py` & `btgsolutions-dataservices-python-client-1.0.9/btgsolutions_dataservices/rest/hfn.py`

 * *Files identical despite different names*

### Comparing `btgsolutions-dataservices-python-client-1.0.8/btgsolutions_dataservices/rest/historical_candles.py` & `btgsolutions-dataservices-python-client-1.0.9/btgsolutions_dataservices/rest/historical_candles.py`

 * *Files identical despite different names*

### Comparing `btgsolutions-dataservices-python-client-1.0.8/btgsolutions_dataservices/rest/intraday_candles.py` & `btgsolutions-dataservices-python-client-1.0.9/btgsolutions_dataservices/rest/intraday_candles.py`

 * *Files identical despite different names*

### Comparing `btgsolutions-dataservices-python-client-1.0.8/btgsolutions_dataservices/rest/intraday_tick_data.py` & `btgsolutions-dataservices-python-client-1.0.9/btgsolutions_dataservices/rest/intraday_tick_data.py`

 * *Files identical despite different names*

### Comparing `btgsolutions-dataservices-python-client-1.0.8/btgsolutions_dataservices/rest/quotes.py` & `btgsolutions-dataservices-python-client-1.0.9/btgsolutions_dataservices/rest/quotes.py`

 * *Files identical despite different names*

### Comparing `btgsolutions-dataservices-python-client-1.0.8/btgsolutions_dataservices/websocket/hfn_websocket_client.py` & `btgsolutions-dataservices-python-client-1.0.9/btgsolutions_dataservices/websocket/hfn_websocket_client.py`

 * *Files identical despite different names*

### Comparing `btgsolutions-dataservices-python-client-1.0.8/btgsolutions_dataservices/websocket/market_data_websocket_client.py` & `btgsolutions-dataservices-python-client-1.0.9/btgsolutions_dataservices/websocket/market_data_websocket_client.py`

 * *Files identical despite different names*

### Comparing `btgsolutions-dataservices-python-client-1.0.8/btgsolutions_dataservices_python_client.egg-info/PKG-INFO` & `btgsolutions-dataservices-python-client-1.0.9/btgsolutions_dataservices_python_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btgsolutions-dataservices-python-client
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python package containing several classes and data for extracting and manipulating market and trading data.
 Home-page: https://github.com/BTG-Pactual-Solutions/btgsolutions-dataservices-python-client
 Author: BTG Solutions Data Services powered by BTG Pactual Solutions
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas<2.0,>=1.3.5
@@ -165,14 +165,22 @@
 
 ```python
 import btgsolutions_dataservices as btg
 quotes = btg.Quotes(api_key='YOUR_API_KEY')
 quotes.get_quote(market_type = 'stocks', tickers = ['PETR4', 'VALE3'])
 ```
 
+## Example - Ticker Last Event
+
+```python
+import btgsolutions_dataservices as btg
+last_event = btg.TickerLastEvent(api_key='YOUR_API_KEY')
+last_event.get_trades(data_type='equities', ticker='VALE3')
+```
+
 ## Example BulkData - Available Tickers
 ```python
 import btgsolutions_dataservices as btg
 bulk_data = btg.BulkData(api_key='YOUR_API_KEY')
 bulk_data.get_available_tickers(date='2023-07-03', data_type='trades', prefix='PETR')
 ```
```

### Comparing `btgsolutions-dataservices-python-client-1.0.8/btgsolutions_dataservices_python_client.egg-info/SOURCES.txt` & `btgsolutions-dataservices-python-client-1.0.9/btgsolutions_dataservices_python_client.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 btgsolutions_dataservices/rest/authenticator.py
 btgsolutions_dataservices/rest/bulk_data.py
 btgsolutions_dataservices/rest/hfn.py
 btgsolutions_dataservices/rest/historical_candles.py
 btgsolutions_dataservices/rest/intraday_candles.py
 btgsolutions_dataservices/rest/intraday_tick_data.py
 btgsolutions_dataservices/rest/quotes.py
+btgsolutions_dataservices/rest/ticker_last_event.py
 btgsolutions_dataservices/websocket/__init__.py
 btgsolutions_dataservices/websocket/hfn_websocket_client.py
 btgsolutions_dataservices/websocket/market_data_websocket_client.py
 btgsolutions_dataservices/websocket/websocket_default_functions.py
 btgsolutions_dataservices_python_client.egg-info/PKG-INFO
 btgsolutions_dataservices_python_client.egg-info/SOURCES.txt
 btgsolutions_dataservices_python_client.egg-info/dependency_links.txt
```

### Comparing `btgsolutions-dataservices-python-client-1.0.8/setup.py` & `btgsolutions-dataservices-python-client-1.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         with open(requirementPath) as f:
             install_requires = f.read().splitlines()
 
 description = "Python package containing several classes and data for extracting and manipulating market and trading data."
 
 setup(
     name='btgsolutions-dataservices-python-client',
-    version='1.0.8',
+    version='1.0.9',
     description=description,
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="BTG Solutions Data Services powered by BTG Pactual Solutions",
     packages=find_packages(),
     url="https://github.com/BTG-Pactual-Solutions/btgsolutions-dataservices-python-client",
     install_requires=install_requires,
```

