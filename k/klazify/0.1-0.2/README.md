# Comparing `tmp/klazify-0.1.tar.gz` & `tmp/klazify-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klazify-0.1.tar", last modified: Thu May 16 16:05:12 2024, max compression
+gzip compressed data, was "klazify-0.2.tar", last modified: Thu May 16 16:14:25 2024, max compression
```

## Comparing `klazify-0.1.tar` & `klazify-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 16:05:12.461605 klazify-0.1/
--rw-rw-rw-   0        0        0     3596 2024-05-16 16:05:12.458041 klazify-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2954 2024-05-16 16:04:51.000000 klazify-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 16:05:12.406480 klazify-0.1/klazify.egg-info/
--rw-rw-rw-   0        0        0     3596 2024-05-16 16:05:12.000000 klazify-0.1/klazify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2024-05-16 16:05:12.000000 klazify-0.1/klazify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 16:05:12.000000 klazify-0.1/klazify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-16 16:05:12.000000 klazify-0.1/klazify.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-16 16:05:12.447476 klazify-0.1/klazify_api/
--rw-rw-rw-   0        0        0       43 2024-05-16 15:49:48.000000 klazify-0.1/klazify_api/__init__.py
--rw-rw-rw-   0        0        0     2153 2024-05-16 16:00:51.000000 klazify-0.1/klazify_api/client.py
--rw-rw-rw-   0        0        0       42 2024-05-16 16:05:12.463660 klazify-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1000 2024-05-16 15:52:24.000000 klazify-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 16:14:25.189865 klazify-0.2/
+-rw-rw-rw-   0        0        0     3604 2024-05-16 16:14:25.188683 klazify-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2962 2024-05-16 16:11:51.000000 klazify-0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 16:14:25.172680 klazify-0.2/klazify.egg-info/
+-rw-rw-rw-   0        0        0     3604 2024-05-16 16:14:24.000000 klazify-0.2/klazify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2024-05-16 16:14:24.000000 klazify-0.2/klazify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 16:14:24.000000 klazify-0.2/klazify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-16 16:14:24.000000 klazify-0.2/klazify.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 16:14:25.185685 klazify-0.2/klazify_api/
+-rw-rw-rw-   0        0        0       47 2024-05-16 16:13:44.000000 klazify-0.2/klazify_api/__init__.py
+-rw-rw-rw-   0        0        0     2153 2024-05-16 16:00:51.000000 klazify-0.2/klazify_api/client.py
+-rw-rw-rw-   0        0        0       42 2024-05-16 16:14:25.189865 klazify-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1000 2024-05-16 16:14:00.000000 klazify-0.2/setup.py
```

### Comparing `klazify-0.1/PKG-INFO` & `klazify-0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klazify
-Version: 0.1
+Version: 0.2
 Summary: The most accurate Content Classification API. All-in-one domain data source
 Home-page: https://github.com/Zyla-Labs/pypi-klazify-api
 Author: Klazify
 Author-email: hello@klazify.com
 Keywords: commodities-api,precious Commodities api,Commodities api,Commodities,precious Commodities,gold,silver,Platinum,Palladium,Ruthenium,Rhodium,forex data,rates,money,usd,eur,btc,forex api,gbp to usd,gbp to eur,eur to usd,api,currency api,exchange rate api,get currency rates api,currency rates php,usd to eur api,copper,nickel,aluminium,TIN,Zinc
 Description-Content-Type: text/markdown
 
@@ -66,25 +66,25 @@
 The Klazify Python SDK is a wrapper around the [requests](https://docs.python-requests.org/en/master/) library. Klazify supports a GET request for now.
 
 Sign-up to Klazify to [get your API key](https://www.klazify.com/register) and some credits to get started.
 
 ### Making the GET request
 
 ```python
->>> from klazify import KlazifyApiClient
+>>> from klazify_api import KlazifyApiClient
 
 >>> client = KlazifyApiClient(access_key='REPLACE-WITH-YOUR-ACCESS-KEY')
 
 >>> response = client.categorize_url("URL")
 ```
 
 ### Request Example
 
 ```python
->>> from klazify import KlazifyApiClient
+>>> from klazify_api import KlazifyApiClient
 
 >>> client = KlazifyApiClient(access_key='REPLACE-WITH-YOUR-ACCESS-KEY')
 
 >>> response = client.categorize_url("https://www.nike.com.ar")
 ```
 
 ### Response Example
```

### Comparing `klazify-0.1/README.md` & `klazify-0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -56,25 +56,25 @@
 The Klazify Python SDK is a wrapper around the [requests](https://docs.python-requests.org/en/master/) library. Klazify supports a GET request for now.
 
 Sign-up to Klazify to [get your API key](https://www.klazify.com/register) and some credits to get started.
 
 ### Making the GET request
 
 ```python
->>> from klazify import KlazifyApiClient
+>>> from klazify_api import KlazifyApiClient
 
 >>> client = KlazifyApiClient(access_key='REPLACE-WITH-YOUR-ACCESS-KEY')
 
 >>> response = client.categorize_url("URL")
 ```
 
 ### Request Example
 
 ```python
->>> from klazify import KlazifyApiClient
+>>> from klazify_api import KlazifyApiClient
 
 >>> client = KlazifyApiClient(access_key='REPLACE-WITH-YOUR-ACCESS-KEY')
 
 >>> response = client.categorize_url("https://www.nike.com.ar")
 ```
 
 ### Response Example
```

### Comparing `klazify-0.1/klazify.egg-info/PKG-INFO` & `klazify-0.2/klazify.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klazify
-Version: 0.1
+Version: 0.2
 Summary: The most accurate Content Classification API. All-in-one domain data source
 Home-page: https://github.com/Zyla-Labs/pypi-klazify-api
 Author: Klazify
 Author-email: hello@klazify.com
 Keywords: commodities-api,precious Commodities api,Commodities api,Commodities,precious Commodities,gold,silver,Platinum,Palladium,Ruthenium,Rhodium,forex data,rates,money,usd,eur,btc,forex api,gbp to usd,gbp to eur,eur to usd,api,currency api,exchange rate api,get currency rates api,currency rates php,usd to eur api,copper,nickel,aluminium,TIN,Zinc
 Description-Content-Type: text/markdown
 
@@ -66,25 +66,25 @@
 The Klazify Python SDK is a wrapper around the [requests](https://docs.python-requests.org/en/master/) library. Klazify supports a GET request for now.
 
 Sign-up to Klazify to [get your API key](https://www.klazify.com/register) and some credits to get started.
 
 ### Making the GET request
 
 ```python
->>> from klazify import KlazifyApiClient
+>>> from klazify_api import KlazifyApiClient
 
 >>> client = KlazifyApiClient(access_key='REPLACE-WITH-YOUR-ACCESS-KEY')
 
 >>> response = client.categorize_url("URL")
 ```
 
 ### Request Example
 
 ```python
->>> from klazify import KlazifyApiClient
+>>> from klazify_api import KlazifyApiClient
 
 >>> client = KlazifyApiClient(access_key='REPLACE-WITH-YOUR-ACCESS-KEY')
 
 >>> response = client.categorize_url("https://www.nike.com.ar")
 ```
 
 ### Response Example
```

### Comparing `klazify-0.1/klazify_api/client.py` & `klazify-0.2/klazify_api/client.py`

 * *Files identical despite different names*

### Comparing `klazify-0.1/setup.py` & `klazify-0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md","r") as f:
     description = f.read()
 
 setup(
     name='klazify',
-    version='0.1',
+    version='0.2',
     description = 'The most accurate Content Classification API. All-in-one domain data source',
     author = 'Klazify',
     author_email = 'hello@klazify.com',
     url = 'https://github.com/Zyla-Labs/pypi-klazify-api',
     keywords = ['commodities-api', 'precious Commodities api',  'Commodities api', 'Commodities', 'precious Commodities' , 'gold' , 'silver', 'Platinum', 'Palladium', 'Ruthenium', 'Rhodium', 'forex data', 'rates', 'money', 'usd', 'eur', 'btc', 'forex api', 'gbp to usd', 'gbp to eur', 'eur to usd', 'api', 'currency api', 'exchange rate api', 'get currency rates api', 'currency rates php', 'usd to eur api','copper','nickel','aluminium','TIN', 'Zinc'],
     packages=find_packages(),
     install_requires=[
```

