# Comparing `tmp/ccs-digitalmarketplace-apiclient-25.8.0.tar.gz` & `tmp/ccs-digitalmarketplace-apiclient-25.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccs-digitalmarketplace-apiclient-25.8.0.tar", last modified: Thu May  2 14:05:15 2024, max compression
+gzip compressed data, was "ccs-digitalmarketplace-apiclient-25.9.0.tar", last modified: Wed May  8 12:54:16 2024, max compression
```

## Comparing `ccs-digitalmarketplace-apiclient-25.8.0.tar` & `ccs-digitalmarketplace-apiclient-25.9.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:05:15.430544 ccs-digitalmarketplace-apiclient-25.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-02 14:05:03.000000 ccs-digitalmarketplace-apiclient-25.8.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-02 14:05:15.430544 ccs-digitalmarketplace-apiclient-25.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-02 14:05:03.000000 ccs-digitalmarketplace-apiclient-25.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:05:15.426544 ccs-digitalmarketplace-apiclient-25.8.0/ccs_digitalmarketplace_apiclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-02 14:05:15.000000 ccs-digitalmarketplace-apiclient-25.8.0/ccs_digitalmarketplace_apiclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-02 14:05:15.000000 ccs-digitalmarketplace-apiclient-25.8.0/ccs_digitalmarketplace_apiclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 14:05:15.000000 ccs-digitalmarketplace-apiclient-25.8.0/ccs_digitalmarketplace_apiclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-02 14:05:15.000000 ccs-digitalmarketplace-apiclient-25.8.0/ccs_digitalmarketplace_apiclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-02 14:05:15.000000 ccs-digitalmarketplace-apiclient-25.8.0/ccs_digitalmarketplace_apiclient.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:05:15.430544 ccs-digitalmarketplace-apiclient-25.8.0/dmapiclient/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-02 14:05:03.000000 ccs-digitalmarketplace-apiclient-25.8.0/dmapiclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-02 14:05:03.000000 ccs-digitalmarketplace-apiclient-25.8.0/dmapiclient/antivirus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-02 14:05:03.000000 ccs-digitalmarketplace-apiclient-25.8.0/dmapiclient/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)    13156 2024-05-02 14:05:03.000000 ccs-digitalmarketplace-apiclient-25.8.0/dmapiclient/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    47385 2024-05-02 14:05:03.000000 ccs-digitalmarketplace-apiclient-25.8.0/dmapiclient/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-02 14:05:03.000000 ccs-digitalmarketplace-apiclient-25.8.0/dmapiclient/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-02 14:05:03.000000 ccs-digitalmarketplace-apiclient-25.8.0/dmapiclient/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5645 2024-05-02 14:05:03.000000 ccs-digitalmarketplace-apiclient-25.8.0/dmapiclient/search.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-02 14:05:15.430544 ccs-digitalmarketplace-apiclient-25.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-02 14:05:03.000000 ccs-digitalmarketplace-apiclient-25.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:16.061723 ccs-digitalmarketplace-apiclient-25.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-08 12:53:51.000000 ccs-digitalmarketplace-apiclient-25.9.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-08 12:54:16.061723 ccs-digitalmarketplace-apiclient-25.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-05-08 12:53:51.000000 ccs-digitalmarketplace-apiclient-25.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:16.057723 ccs-digitalmarketplace-apiclient-25.9.0/ccs_digitalmarketplace_apiclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-08 12:54:15.000000 ccs-digitalmarketplace-apiclient-25.9.0/ccs_digitalmarketplace_apiclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-08 12:54:16.000000 ccs-digitalmarketplace-apiclient-25.9.0/ccs_digitalmarketplace_apiclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 12:54:15.000000 ccs-digitalmarketplace-apiclient-25.9.0/ccs_digitalmarketplace_apiclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-08 12:54:15.000000 ccs-digitalmarketplace-apiclient-25.9.0/ccs_digitalmarketplace_apiclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-08 12:54:15.000000 ccs-digitalmarketplace-apiclient-25.9.0/ccs_digitalmarketplace_apiclient.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:16.061723 ccs-digitalmarketplace-apiclient-25.9.0/dmapiclient/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-08 12:53:51.000000 ccs-digitalmarketplace-apiclient-25.9.0/dmapiclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-08 12:53:51.000000 ccs-digitalmarketplace-apiclient-25.9.0/dmapiclient/antivirus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-08 12:53:51.000000 ccs-digitalmarketplace-apiclient-25.9.0/dmapiclient/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13156 2024-05-08 12:53:51.000000 ccs-digitalmarketplace-apiclient-25.9.0/dmapiclient/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47385 2024-05-08 12:53:51.000000 ccs-digitalmarketplace-apiclient-25.9.0/dmapiclient/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-08 12:53:51.000000 ccs-digitalmarketplace-apiclient-25.9.0/dmapiclient/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-08 12:53:51.000000 ccs-digitalmarketplace-apiclient-25.9.0/dmapiclient/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 12:53:51.000000 ccs-digitalmarketplace-apiclient-25.9.0/dmapiclient/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5645 2024-05-08 12:53:51.000000 ccs-digitalmarketplace-apiclient-25.9.0/dmapiclient/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-08 12:54:16.061723 ccs-digitalmarketplace-apiclient-25.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-08 12:53:51.000000 ccs-digitalmarketplace-apiclient-25.9.0/setup.py
```

### Comparing `ccs-digitalmarketplace-apiclient-25.8.0/LICENCE` & `ccs-digitalmarketplace-apiclient-25.9.0/LICENCE`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-apiclient-25.8.0/README.md` & `ccs-digitalmarketplace-apiclient-25.9.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Digital Marketplace API client
 =========================
 
 ![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)
+![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)
+![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)
 
 ## What's in here?
 
 API clients for Digital Marketplace [Data API](https://github.com/Crown-Commercial-Service/ccs-digitalmarketplace-api) and
 [Search API](https://github.com/Crown-Commercial-Service/ccs-digitalmarketplace-search-api).
 
 Originally was part of [Digital Marketplace Utils](https://github.com/Crown-Commercial-Service/ccs-digitalmarketplace-utils).
```

### Comparing `ccs-digitalmarketplace-apiclient-25.8.0/dmapiclient/antivirus.py` & `ccs-digitalmarketplace-apiclient-25.9.0/dmapiclient/antivirus.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-apiclient-25.8.0/dmapiclient/audit.py` & `ccs-digitalmarketplace-apiclient-25.9.0/dmapiclient/audit.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-apiclient-25.8.0/dmapiclient/base.py` & `ccs-digitalmarketplace-apiclient-25.9.0/dmapiclient/base.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-apiclient-25.8.0/dmapiclient/data.py` & `ccs-digitalmarketplace-apiclient-25.9.0/dmapiclient/data.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-apiclient-25.8.0/dmapiclient/errors.py` & `ccs-digitalmarketplace-apiclient-25.9.0/dmapiclient/errors.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-apiclient-25.8.0/dmapiclient/search.py` & `ccs-digitalmarketplace-apiclient-25.9.0/dmapiclient/search.py`

 * *Files identical despite different names*

