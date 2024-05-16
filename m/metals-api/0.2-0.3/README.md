# Comparing `tmp/metals_api-0.2.tar.gz` & `tmp/metals_api-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metals_api-0.2.tar", last modified: Tue May 14 20:25:20 2024, max compression
+gzip compressed data, was "metals_api-0.3.tar", last modified: Wed May 15 20:08:06 2024, max compression
```

## Comparing `metals_api-0.2.tar` & `metals_api-0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 20:25:20.606725 metals_api-0.2/
--rw-rw-rw-   0        0        0     4585 2024-05-14 20:25:20.605726 metals_api-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3969 2024-05-14 20:15:22.000000 metals_api-0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 20:25:20.536726 metals_api-0.2/metals_api/
--rw-rw-rw-   0        0        0       79 2024-05-14 18:40:20.000000 metals_api-0.2/metals_api/__init__.py
--rw-rw-rw-   0        0        0     1707 2024-05-14 20:22:28.000000 metals_api-0.2/metals_api/client.py
-drwxrwxrwx   0        0        0        0 2024-05-14 20:25:20.603726 metals_api-0.2/metals_api.egg-info/
--rw-rw-rw-   0        0        0     4585 2024-05-14 20:25:20.000000 metals_api-0.2/metals_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2024-05-14 20:25:20.000000 metals_api-0.2/metals_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 20:25:20.000000 metals_api-0.2/metals_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-14 20:25:20.000000 metals_api-0.2/metals_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 20:25:20.607728 metals_api-0.2/setup.cfg
--rw-rw-rw-   0        0        0      971 2024-05-14 20:13:44.000000 metals_api-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 20:08:06.938546 metals_api-0.3/
+-rw-rw-rw-   0        0        0     4837 2024-05-15 20:08:06.937547 metals_api-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4221 2024-05-15 20:07:12.000000 metals_api-0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 20:08:06.912548 metals_api-0.3/metals_api/
+-rw-rw-rw-   0        0        0       45 2024-05-15 20:07:24.000000 metals_api-0.3/metals_api/__init__.py
+-rw-rw-rw-   0        0        0     1707 2024-05-14 20:22:28.000000 metals_api-0.3/metals_api/client.py
+drwxrwxrwx   0        0        0        0 2024-05-15 20:08:06.936546 metals_api-0.3/metals_api.egg-info/
+-rw-rw-rw-   0        0        0     4837 2024-05-15 20:08:06.000000 metals_api-0.3/metals_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2024-05-15 20:08:06.000000 metals_api-0.3/metals_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 20:08:06.000000 metals_api-0.3/metals_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-15 20:08:06.000000 metals_api-0.3/metals_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 20:08:06.939548 metals_api-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      971 2024-05-15 20:07:16.000000 metals_api-0.3/setup.py
```

### Comparing `metals_api-0.2/PKG-INFO` & `metals_api-0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metals_api
-Version: 0.2
+Version: 0.3
 Summary: A Python package to get the latest metals prices from the Metals-API
 Home-page: https://github.com/Zyla-Labs/pypi-metals-api
 Author: Zyla Labs
 Author-email: hello@zylalabs.com
 Keywords: metals-api,precious metals api,metals api,metals, precious metals,gold,silver,Platinum,Palladium,Ruthenium,Rhodium,forex data,rates,money,usd,eur,btc,forex api,gbp to usd,gbp to eur,eur to usd,api,currency api,exchange rate api,get currency rates api,currency rates php,usd to eur api,copper,nickel,aluminium,TIN,Zinc
 Description-Content-Type: text/markdown
 
@@ -99,7 +99,21 @@
         "USDXAG": 28.579913118878963,
         "USDXAU": 2352.8445214994495,
         "USDXPT": 1021.79819906694
     }
 }
 ```
 
+### AVAILABLE METHODS
+
+```python
+>>> get_latest(base: str, symbols: List[str])
+```
+
+```python
+>>> get_historical(date:str, base:str, symbols: List[str])
+```
+
+```python
+>>> get_time_series(start_date: str, end_date: str, symbol: str)
+```
+
```

### Comparing `metals_api-0.2/README.md` & `metals_api-0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -89,7 +89,21 @@
         "USDXAG": 28.579913118878963,
         "USDXAU": 2352.8445214994495,
         "USDXPT": 1021.79819906694
     }
 }
 ```
 
+### AVAILABLE METHODS
+
+```python
+>>> get_latest(base: str, symbols: List[str])
+```
+
+```python
+>>> get_historical(date:str, base:str, symbols: List[str])
+```
+
+```python
+>>> get_time_series(start_date: str, end_date: str, symbol: str)
+```
+
```

### Comparing `metals_api-0.2/metals_api/client.py` & `metals_api-0.3/metals_api/client.py`

 * *Files identical despite different names*

### Comparing `metals_api-0.2/metals_api.egg-info/PKG-INFO` & `metals_api-0.3/metals_api.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metals-api
-Version: 0.2
+Version: 0.3
 Summary: A Python package to get the latest metals prices from the Metals-API
 Home-page: https://github.com/Zyla-Labs/pypi-metals-api
 Author: Zyla Labs
 Author-email: hello@zylalabs.com
 Keywords: metals-api,precious metals api,metals api,metals, precious metals,gold,silver,Platinum,Palladium,Ruthenium,Rhodium,forex data,rates,money,usd,eur,btc,forex api,gbp to usd,gbp to eur,eur to usd,api,currency api,exchange rate api,get currency rates api,currency rates php,usd to eur api,copper,nickel,aluminium,TIN,Zinc
 Description-Content-Type: text/markdown
 
@@ -99,7 +99,21 @@
         "USDXAG": 28.579913118878963,
         "USDXAU": 2352.8445214994495,
         "USDXPT": 1021.79819906694
     }
 }
 ```
 
+### AVAILABLE METHODS
+
+```python
+>>> get_latest(base: str, symbols: List[str])
+```
+
+```python
+>>> get_historical(date:str, base:str, symbols: List[str])
+```
+
+```python
+>>> get_time_series(start_date: str, end_date: str, symbol: str)
+```
+
```

### Comparing `metals_api-0.2/setup.py` & `metals_api-0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md","r") as f:
     description = f.read()
 
 setup(
     name='metals_api',
-    version='0.2',
+    version='0.3',
     description = 'A Python package to get the latest metals prices from the Metals-API',
     author = 'Zyla Labs',
     author_email = 'hello@zylalabs.com',
     url = 'https://github.com/Zyla-Labs/pypi-metals-api',
     keywords = ['metals-api', 'precious metals api',  'metals api', 'metals, precious metals' , 'gold' , 'silver', 'Platinum', 'Palladium', 'Ruthenium', 'Rhodium', 'forex data', 'rates', 'money', 'usd', 'eur', 'btc', 'forex api', 'gbp to usd', 'gbp to eur', 'eur to usd', 'api', 'currency api', 'exchange rate api', 'get currency rates api', 'currency rates php', 'usd to eur api','copper','nickel','aluminium','TIN', 'Zinc'],
     packages=find_packages(),
     install_requires=[
```

