# Comparing `tmp/payok_aio-0.1.5.tar.gz` & `tmp/payok_aio-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "payok_aio-0.1.5.tar", max compression
+gzip compressed data, was "payok_aio-0.1.6.tar", max compression
```

## Comparing `payok_aio-0.1.5.tar` & `payok_aio-0.1.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35149 2024-05-16 12:27:58.411893 payok_aio-0.1.5/LICENSE
--rw-r--r--   0        0        0     3412 2024-05-16 12:27:58.411893 payok_aio-0.1.5/README.md
--rw-r--r--   0        0        0       22 2024-05-16 12:27:58.411893 payok_aio-0.1.5/payok_aio/__init__.py
--rw-r--r--   0        0        0     4242 2024-05-16 12:27:58.411893 payok_aio-0.1.5/payok_aio/api.py
--rw-r--r--   0        0        0     5036 2024-05-16 12:27:58.411893 payok_aio-0.1.5/payok_aio/const.py
--rw-r--r--   0        0        0     1665 2024-05-16 12:27:58.411893 payok_aio-0.1.5/payok_aio/exceptions.py
--rw-r--r--   0        0        0      586 2024-05-16 12:27:58.411893 payok_aio-0.1.5/payok_aio/models.py
--rw-r--r--   0        0        0     1709 2024-05-16 12:27:58.411893 payok_aio-0.1.5/payok_aio/utils.py
--rw-r--r--   0        0        0      375 2024-05-16 12:27:58.411893 payok_aio-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3972 1970-01-01 00:00:00.000000 payok_aio-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-16 12:35:54.648453 payok_aio-0.1.6/LICENSE
+-rw-r--r--   0        0        0     3412 2024-05-16 12:35:54.648453 payok_aio-0.1.6/README.md
+-rw-r--r--   0        0        0       22 2024-05-16 12:35:54.648453 payok_aio-0.1.6/payok_aio/__init__.py
+-rw-r--r--   0        0        0     4245 2024-05-16 12:35:54.648453 payok_aio-0.1.6/payok_aio/api.py
+-rw-r--r--   0        0        0     5036 2024-05-16 12:35:54.648453 payok_aio-0.1.6/payok_aio/const.py
+-rw-r--r--   0        0        0     1665 2024-05-16 12:35:54.648453 payok_aio-0.1.6/payok_aio/exceptions.py
+-rw-r--r--   0        0        0      586 2024-05-16 12:35:54.648453 payok_aio-0.1.6/payok_aio/models.py
+-rw-r--r--   0        0        0     1709 2024-05-16 12:35:54.648453 payok_aio-0.1.6/payok_aio/utils.py
+-rw-r--r--   0        0        0      375 2024-05-16 12:35:54.652453 payok_aio-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3972 1970-01-01 00:00:00.000000 payok_aio-0.1.6/PKG-INFO
```

### Comparing `payok_aio-0.1.5/LICENSE` & `payok_aio-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `payok_aio-0.1.5/README.md` & `payok_aio-0.1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Payok API Client
 
 Python асинхронный клиент для взаимодействия с Payok API. Позволяет получать баланс, транзакции и создавать платежные формы.
 
 ## Установка
 
 ```bash
-pip install payok_aio
+pip install payok-aio
 ```
 
 ## Примеры использования
 
 ```python
 import asyncio
 from payok_aio import Payok
```

### Comparing `payok_aio-0.1.5/payok_aio/api.py` & `payok_aio-0.1.6/payok_aio/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from hashlib import md5
 from typing import List, Optional, Union
 from urllib.parse import urlencode
-from const import Currencies, HTTPMethods
-from utils import AsyncRequestSession
-from models import Balance, Transaction
+from .const import Currencies, HTTPMethods
+from .utils import AsyncRequestSession
+from .models import Balance, Transaction
 
 
 class Payok:
     API_HOST = 'https://payok.io'
     API_DOCS = 'https://payok.io/cabinet/documentation/doc_main.php'
 
     def __init__(
```

### Comparing `payok_aio-0.1.5/payok_aio/const.py` & `payok_aio-0.1.6/payok_aio/const.py`

 * *Files identical despite different names*

### Comparing `payok_aio-0.1.5/payok_aio/exceptions.py` & `payok_aio-0.1.6/payok_aio/exceptions.py`

 * *Files identical despite different names*

### Comparing `payok_aio-0.1.5/payok_aio/models.py` & `payok_aio-0.1.6/payok_aio/models.py`

 * *Files identical despite different names*

### Comparing `payok_aio-0.1.5/payok_aio/utils.py` & `payok_aio-0.1.6/payok_aio/utils.py`

 * *Files identical despite different names*

### Comparing `payok_aio-0.1.5/PKG-INFO` & `payok_aio-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payok-aio
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: BazZziliuS
 Author-email: bazzzil123@gmail.com
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -23,15 +23,15 @@
 # Payok API Client
 
 Python асинхронный клиент для взаимодействия с Payok API. Позволяет получать баланс, транзакции и создавать платежные формы.
 
 ## Установка
 
 ```bash
-pip install payok_aio
+pip install payok-aio
 ```
 
 ## Примеры использования
 
 ```python
 import asyncio
 from payok_aio import Payok
```

