# Comparing `tmp/payok_aio-0.1.4.tar.gz` & `tmp/payok_aio-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "payok_aio-0.1.4.tar", max compression
+gzip compressed data, was "payok_aio-0.1.5.tar", max compression
```

## Comparing `payok_aio-0.1.4.tar` & `payok_aio-0.1.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35149 2024-03-02 04:23:19.906236 payok_aio-0.1.4/LICENSE
--rw-r--r--   0        0        0     3164 2024-03-02 04:23:19.906236 payok_aio-0.1.4/README.md
--rw-r--r--   0        0        0       22 2024-03-02 04:23:19.906236 payok_aio-0.1.4/payok-aio/__init__.py
--rw-r--r--   0        0        0     4242 2024-03-02 04:23:19.906236 payok_aio-0.1.4/payok-aio/api.py
--rw-r--r--   0        0        0     5036 2024-03-02 04:23:19.906236 payok_aio-0.1.4/payok-aio/const.py
--rw-r--r--   0        0        0     1665 2024-03-02 04:23:19.906236 payok_aio-0.1.4/payok-aio/exceptions.py
--rw-r--r--   0        0        0      586 2024-03-02 04:23:19.906236 payok_aio-0.1.4/payok-aio/models.py
--rw-r--r--   0        0        0     1709 2024-03-02 04:23:19.906236 payok_aio-0.1.4/payok-aio/utils.py
--rw-r--r--   0        0        0      375 2024-03-02 04:23:19.906236 payok_aio-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3724 1970-01-01 00:00:00.000000 payok_aio-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-16 12:27:58.411893 payok_aio-0.1.5/LICENSE
+-rw-r--r--   0        0        0     3412 2024-05-16 12:27:58.411893 payok_aio-0.1.5/README.md
+-rw-r--r--   0        0        0       22 2024-05-16 12:27:58.411893 payok_aio-0.1.5/payok_aio/__init__.py
+-rw-r--r--   0        0        0     4242 2024-05-16 12:27:58.411893 payok_aio-0.1.5/payok_aio/api.py
+-rw-r--r--   0        0        0     5036 2024-05-16 12:27:58.411893 payok_aio-0.1.5/payok_aio/const.py
+-rw-r--r--   0        0        0     1665 2024-05-16 12:27:58.411893 payok_aio-0.1.5/payok_aio/exceptions.py
+-rw-r--r--   0        0        0      586 2024-05-16 12:27:58.411893 payok_aio-0.1.5/payok_aio/models.py
+-rw-r--r--   0        0        0     1709 2024-05-16 12:27:58.411893 payok_aio-0.1.5/payok_aio/utils.py
+-rw-r--r--   0        0        0      375 2024-05-16 12:27:58.411893 payok_aio-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3972 1970-01-01 00:00:00.000000 payok_aio-0.1.5/PKG-INFO
```

### Comparing `payok_aio-0.1.4/LICENSE` & `payok_aio-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `payok_aio-0.1.4/README.md` & `payok_aio-0.1.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/payok-aio)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/payok_aio)
 ![PyPI - Version](https://img.shields.io/pypi/v/payok_aio)
+[![wakatime](https://wakatime.com/badge/user/d1734201-6222-408c-98a4-642d2b764ecb/project/018dfcb0-b754-4ee2-98d0-437403cb0bf1.svg)](https://wakatime.com/badge/user/d1734201-6222-408c-98a4-642d2b764ecb/project/018dfcb0-b754-4ee2-98d0-437403cb0bf1)
 
 # Payok API Client
 
 Python асинхронный клиент для взаимодействия с Payok API. Позволяет получать баланс, транзакции и создавать платежные формы.
 
 ## Установка
```

### Comparing `payok_aio-0.1.4/payok-aio/api.py` & `payok_aio-0.1.5/payok_aio/api.py`

 * *Files identical despite different names*

### Comparing `payok_aio-0.1.4/payok-aio/const.py` & `payok_aio-0.1.5/payok_aio/const.py`

 * *Files identical despite different names*

### Comparing `payok_aio-0.1.4/payok-aio/exceptions.py` & `payok_aio-0.1.5/payok_aio/exceptions.py`

 * *Files identical despite different names*

### Comparing `payok_aio-0.1.4/payok-aio/models.py` & `payok_aio-0.1.5/payok_aio/models.py`

 * *Files identical despite different names*

### Comparing `payok_aio-0.1.4/payok-aio/utils.py` & `payok_aio-0.1.5/payok_aio/utils.py`

 * *Files identical despite different names*

### Comparing `payok_aio-0.1.4/PKG-INFO` & `payok_aio-0.1.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payok-aio
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: BazZziliuS
 Author-email: bazzzil123@gmail.com
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -14,14 +14,15 @@
 Requires-Dist: certifi (>=2024.2.2,<2025.0.0)
 Requires-Dist: pydantic (>=2.6.3,<3.0.0)
 Description-Content-Type: text/markdown
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/payok-aio)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/payok_aio)
 ![PyPI - Version](https://img.shields.io/pypi/v/payok_aio)
+[![wakatime](https://wakatime.com/badge/user/d1734201-6222-408c-98a4-642d2b764ecb/project/018dfcb0-b754-4ee2-98d0-437403cb0bf1.svg)](https://wakatime.com/badge/user/d1734201-6222-408c-98a4-642d2b764ecb/project/018dfcb0-b754-4ee2-98d0-437403cb0bf1)
 
 # Payok API Client
 
 Python асинхронный клиент для взаимодействия с Payok API. Позволяет получать баланс, транзакции и создавать платежные формы.
 
 ## Установка
```

