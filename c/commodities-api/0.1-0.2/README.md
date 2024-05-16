# Comparing `tmp/commodities_api-0.1.tar.gz` & `tmp/commodities_api-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commodities_api-0.1.tar", last modified: Wed May 15 18:45:54 2024, max compression
+gzip compressed data, was "commodities_api-0.2.tar", last modified: Wed May 15 20:04:04 2024, max compression
```

## Comparing `commodities_api-0.1.tar` & `commodities_api-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 18:45:54.652338 commodities_api-0.1/
--rw-rw-rw-   0        0        0     4268 2024-05-15 18:45:54.651337 commodities_api-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3615 2024-05-15 18:17:51.000000 commodities_api-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 18:45:54.621369 commodities_api-0.1/commodities_api/
--rw-rw-rw-   0        0        0       55 2024-05-15 18:18:31.000000 commodities_api-0.1/commodities_api/__init__.py
--rw-rw-rw-   0        0        0     1727 2024-05-15 18:20:03.000000 commodities_api-0.1/commodities_api/client.py
-drwxrwxrwx   0        0        0        0 2024-05-15 18:45:54.649337 commodities_api-0.1/commodities_api.egg-info/
--rw-rw-rw-   0        0        0     4268 2024-05-15 18:45:54.000000 commodities_api-0.1/commodities_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      228 2024-05-15 18:45:54.000000 commodities_api-0.1/commodities_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 18:45:54.000000 commodities_api-0.1/commodities_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-15 18:45:54.000000 commodities_api-0.1/commodities_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 18:45:54.652338 commodities_api-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1011 2024-05-15 18:31:47.000000 commodities_api-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 20:04:04.266563 commodities_api-0.2/
+-rw-rw-rw-   0        0        0     4518 2024-05-15 20:04:04.265560 commodities_api-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3865 2024-05-15 19:05:43.000000 commodities_api-0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 20:04:04.232904 commodities_api-0.2/commodities_api/
+-rw-rw-rw-   0        0        0       55 2024-05-15 18:18:31.000000 commodities_api-0.2/commodities_api/__init__.py
+-rw-rw-rw-   0        0        0     1727 2024-05-15 18:20:03.000000 commodities_api-0.2/commodities_api/client.py
+drwxrwxrwx   0        0        0        0 2024-05-15 20:04:04.263690 commodities_api-0.2/commodities_api.egg-info/
+-rw-rw-rw-   0        0        0     4518 2024-05-15 20:04:04.000000 commodities_api-0.2/commodities_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      228 2024-05-15 20:04:04.000000 commodities_api-0.2/commodities_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 20:04:04.000000 commodities_api-0.2/commodities_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-15 20:04:04.000000 commodities_api-0.2/commodities_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 20:04:04.266563 commodities_api-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1011 2024-05-15 20:03:45.000000 commodities_api-0.2/setup.py
```

### Comparing `commodities_api-0.1/PKG-INFO` & `commodities_api-0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commodities_api
-Version: 0.1
+Version: 0.2
 Summary: A Python package to get the latest commodities from the Commodities-API
 Home-page: https://github.com/Zyla-Labs/pypi-commodities-api
 Author: Zyla Labs
 Author-email: hello@zylalabs.com
 Keywords: commodities-api,precious Commodities api,Commodities api,Commodities,precious Commodities,gold,silver,Platinum,Palladium,Ruthenium,Rhodium,forex data,rates,money,usd,eur,btc,forex api,gbp to usd,gbp to eur,eur to usd,api,currency api,exchange rate api,get currency rates api,currency rates php,usd to eur api,copper,nickel,aluminium,TIN,Zinc
 Description-Content-Type: text/markdown
 
@@ -100,7 +100,20 @@
             "WHEAT": "per metric ton",
             "SUGAR": "per lb"
         }
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
```

### Comparing `commodities_api-0.1/README.md` & `commodities_api-0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -90,7 +90,20 @@
             "WHEAT": "per metric ton",
             "SUGAR": "per lb"
         }
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
```

### Comparing `commodities_api-0.1/commodities_api/client.py` & `commodities_api-0.2/commodities_api/client.py`

 * *Files identical despite different names*

### Comparing `commodities_api-0.1/commodities_api.egg-info/PKG-INFO` & `commodities_api-0.2/commodities_api.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commodities-api
-Version: 0.1
+Version: 0.2
 Summary: A Python package to get the latest commodities from the Commodities-API
 Home-page: https://github.com/Zyla-Labs/pypi-commodities-api
 Author: Zyla Labs
 Author-email: hello@zylalabs.com
 Keywords: commodities-api,precious Commodities api,Commodities api,Commodities,precious Commodities,gold,silver,Platinum,Palladium,Ruthenium,Rhodium,forex data,rates,money,usd,eur,btc,forex api,gbp to usd,gbp to eur,eur to usd,api,currency api,exchange rate api,get currency rates api,currency rates php,usd to eur api,copper,nickel,aluminium,TIN,Zinc
 Description-Content-Type: text/markdown
 
@@ -100,7 +100,20 @@
             "WHEAT": "per metric ton",
             "SUGAR": "per lb"
         }
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
```

### Comparing `commodities_api-0.1/setup.py` & `commodities_api-0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md","r") as f:
     description = f.read()
 
 setup(
     name='commodities_api',
-    version='0.1',
+    version='0.2',
     description = 'A Python package to get the latest commodities from the Commodities-API',
     author = 'Zyla Labs',
     author_email = 'hello@zylalabs.com',
     url = 'https://github.com/Zyla-Labs/pypi-commodities-api',
     keywords = ['commodities-api', 'precious Commodities api',  'Commodities api', 'Commodities', 'precious Commodities' , 'gold' , 'silver', 'Platinum', 'Palladium', 'Ruthenium', 'Rhodium', 'forex data', 'rates', 'money', 'usd', 'eur', 'btc', 'forex api', 'gbp to usd', 'gbp to eur', 'eur to usd', 'api', 'currency api', 'exchange rate api', 'get currency rates api', 'currency rates php', 'usd to eur api','copper','nickel','aluminium','TIN', 'Zinc'],
     packages=find_packages(),
     install_requires=[
```

