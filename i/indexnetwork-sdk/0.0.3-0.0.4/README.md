# Comparing `tmp/indexnetwork_sdk-0.0.3.tar.gz` & `tmp/indexnetwork_sdk-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indexnetwork_sdk-0.0.3.tar", last modified: Mon Apr 29 15:57:02 2024, max compression
+gzip compressed data, was "indexnetwork_sdk-0.0.4.tar", last modified: Fri May  3 11:10:54 2024, max compression
```

## Comparing `indexnetwork_sdk-0.0.3.tar` & `indexnetwork_sdk-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:57:02.307584 indexnetwork_sdk-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-29 15:57:02.307584 indexnetwork_sdk-0.0.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:57:02.307584 indexnetwork_sdk-0.0.3/indexclient/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-29 15:56:52.000000 indexnetwork_sdk-0.0.3/indexclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5843 2024-04-29 15:56:52.000000 indexnetwork_sdk-0.0.3/indexclient/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-29 15:56:52.000000 indexnetwork_sdk-0.0.3/indexclient/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-29 15:56:52.000000 indexnetwork_sdk-0.0.3/indexclient/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-29 15:56:52.000000 indexnetwork_sdk-0.0.3/indexclient/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:57:02.307584 indexnetwork_sdk-0.0.3/indexnetwork_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-29 15:57:02.000000 indexnetwork_sdk-0.0.3/indexnetwork_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-29 15:57:02.000000 indexnetwork_sdk-0.0.3/indexnetwork_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 15:57:02.000000 indexnetwork_sdk-0.0.3/indexnetwork_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-29 15:57:02.000000 indexnetwork_sdk-0.0.3/indexnetwork_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-29 15:57:02.000000 indexnetwork_sdk-0.0.3/indexnetwork_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 15:57:02.307584 indexnetwork_sdk-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-29 15:56:52.000000 indexnetwork_sdk-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:10:54.769355 indexnetwork_sdk-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-03 11:10:35.000000 indexnetwork_sdk-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-05-03 11:10:54.765354 indexnetwork_sdk-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-03 11:10:35.000000 indexnetwork_sdk-0.0.4/README.MD
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:10:54.765354 indexnetwork_sdk-0.0.4/indexclient/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-03 11:10:35.000000 indexnetwork_sdk-0.0.4/indexclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-05-03 11:10:36.000000 indexnetwork_sdk-0.0.4/indexclient/chroma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5843 2024-05-03 11:10:36.000000 indexnetwork_sdk-0.0.4/indexclient/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-03 11:10:36.000000 indexnetwork_sdk-0.0.4/indexclient/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-03 11:10:36.000000 indexnetwork_sdk-0.0.4/indexclient/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-05-03 11:10:36.000000 indexnetwork_sdk-0.0.4/indexclient/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:10:54.765354 indexnetwork_sdk-0.0.4/indexnetwork_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-05-03 11:10:54.000000 indexnetwork_sdk-0.0.4/indexnetwork_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-03 11:10:54.000000 indexnetwork_sdk-0.0.4/indexnetwork_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 11:10:54.000000 indexnetwork_sdk-0.0.4/indexnetwork_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-03 11:10:54.000000 indexnetwork_sdk-0.0.4/indexnetwork_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-03 11:10:54.000000 indexnetwork_sdk-0.0.4/indexnetwork_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 11:10:54.769355 indexnetwork_sdk-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-03 11:10:36.000000 indexnetwork_sdk-0.0.4/setup.py
```

### Comparing `indexnetwork_sdk-0.0.3/indexclient/client.py` & `indexnetwork_sdk-0.0.4/indexclient/client.py`

 * *Files identical despite different names*

### Comparing `indexnetwork_sdk-0.0.3/indexclient/types.py` & `indexnetwork_sdk-0.0.4/indexclient/types.py`

 * *Files identical despite different names*

### Comparing `indexnetwork_sdk-0.0.3/indexclient/utils.py` & `indexnetwork_sdk-0.0.4/indexclient/utils.py`

 * *Files identical despite different names*

### Comparing `indexnetwork_sdk-0.0.3/indexnetwork_sdk.egg-info/requires.txt` & `indexnetwork_sdk-0.0.4/indexnetwork_sdk.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `indexnetwork_sdk-0.0.3/setup.py` & `indexnetwork_sdk-0.0.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from setuptools import setup, find_packages
 
 setup(
   name='indexnetwork-sdk',
-  version='0.0.3',
+  version='0.0.4',
   description='Index Network SDK',
-  long_description="Index Network Client SDK",
+  long_description=open(os.path.join(os.path.dirname(os.path.abspath(__file__)), 'README.MD')).read(),
   long_description_content_type='text/markdown',
   author='Index',
   author_email='accounts@index.network',
   url='https://github.com/indexnetwork/index',
   packages=find_packages(),
   include_package_data=True,
   package_data={
```

