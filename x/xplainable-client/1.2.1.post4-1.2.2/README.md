# Comparing `tmp/xplainable-client-1.2.1.post4.tar.gz` & `tmp/xplainable_client-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xplainable-client-1.2.1.post4.tar", last modified: Tue Feb 13 07:46:36 2024, max compression
+gzip compressed data, was "xplainable_client-1.2.2.tar", last modified: Thu May 16 09:20:25 2024, max compression
```

## Comparing `xplainable-client-1.2.1.post4.tar` & `xplainable_client-1.2.2.tar`

### file list

```diff
@@ -1,22 +1,33 @@
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-02-13 07:46:36.411973 xplainable-client-1.2.1.post4/
--rw-r--r--   0 jtuppack   (501) staff       (20)     4718 2024-02-13 07:46:36.411763 xplainable-client-1.2.1.post4/PKG-INFO
--rw-r--r--   0 jtuppack   (501) staff       (20)     3924 2024-02-13 07:45:39.000000 xplainable-client-1.2.1.post4/README.md
--rw-r--r--   0 jtuppack   (501) staff       (20)      864 2024-02-13 07:46:21.000000 xplainable-client-1.2.1.post4/pyproject.toml
--rw-r--r--   0 jtuppack   (501) staff       (20)       38 2024-02-13 07:46:36.412011 xplainable-client-1.2.1.post4/setup.cfg
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-02-13 07:46:36.410130 xplainable-client-1.2.1.post4/xplainable_client/
--rw-r--r--   0 jtuppack   (501) staff       (20)       45 2024-02-11 23:48:01.000000 xplainable-client-1.2.1.post4/xplainable_client/__init__.py
--rw-r--r--   0 jtuppack   (501) staff       (20)    30161 2024-02-12 08:36:49.000000 xplainable-client-1.2.1.post4/xplainable_client/client.py
--rw-r--r--   0 jtuppack   (501) staff       (20)      885 2024-02-11 21:16:19.000000 xplainable-client-1.2.1.post4/xplainable_client/datasets.py
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-02-13 07:46:36.411356 xplainable-client-1.2.1.post4/xplainable_client/utils/
--rw-r--r--   0 jtuppack   (501) staff       (20)        0 2024-02-12 08:30:29.000000 xplainable-client-1.2.1.post4/xplainable_client/utils/__init__.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     1291 2024-02-11 21:43:09.000000 xplainable-client-1.2.1.post4/xplainable_client/utils/encoders.py
--rw-r--r--   0 jtuppack   (501) staff       (20)      180 2024-02-11 21:51:39.000000 xplainable-client-1.2.1.post4/xplainable_client/utils/exceptions.py
--rw-r--r--   0 jtuppack   (501) staff       (20)      980 2024-02-11 21:45:45.000000 xplainable-client-1.2.1.post4/xplainable_client/utils/helpers.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     6426 2024-02-12 08:36:49.000000 xplainable-client-1.2.1.post4/xplainable_client/utils/metrics.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     3042 2024-02-11 21:51:47.000000 xplainable-client-1.2.1.post4/xplainable_client/utils/model_parsers.py
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-02-13 07:46:36.411520 xplainable-client-1.2.1.post4/xplainable_client.egg-info/
--rw-r--r--   0 jtuppack   (501) staff       (20)     4718 2024-02-13 07:46:36.000000 xplainable-client-1.2.1.post4/xplainable_client.egg-info/PKG-INFO
--rw-r--r--   0 jtuppack   (501) staff       (20)      537 2024-02-13 07:46:36.000000 xplainable-client-1.2.1.post4/xplainable_client.egg-info/SOURCES.txt
--rw-r--r--   0 jtuppack   (501) staff       (20)        1 2024-02-13 07:46:36.000000 xplainable-client-1.2.1.post4/xplainable_client.egg-info/dependency_links.txt
--rw-r--r--   0 jtuppack   (501) staff       (20)      145 2024-02-13 07:46:36.000000 xplainable-client-1.2.1.post4/xplainable_client.egg-info/requires.txt
--rw-r--r--   0 jtuppack   (501) staff       (20)       29 2024-02-13 07:46:36.000000 xplainable-client-1.2.1.post4/xplainable_client.egg-info/top_level.txt
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-16 09:20:25.807161 xplainable_client-1.2.2/
+-rw-r--r--   0 jtuppack   (501) staff       (20)     4705 2024-05-16 09:20:25.806912 xplainable_client-1.2.2/PKG-INFO
+-rw-r--r--   0 jtuppack   (501) staff       (20)     3924 2024-02-21 21:39:20.000000 xplainable_client-1.2.2/README.md
+-rw-r--r--   0 jtuppack   (501) staff       (20)      855 2024-05-16 09:18:33.000000 xplainable_client-1.2.2/pyproject.toml
+-rw-r--r--   0 jtuppack   (501) staff       (20)       38 2024-05-16 09:20:25.807206 xplainable_client-1.2.2/setup.cfg
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-16 09:20:25.799899 xplainable_client-1.2.2/xplainable_client/
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-16 09:20:25.803639 xplainable_client-1.2.2/xplainable_client/client/
+-rw-r--r--   0 jtuppack   (501) staff       (20)     1082 2024-05-16 09:16:42.000000 xplainable_client-1.2.2/xplainable_client/client/__init__.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)      123 2024-05-16 09:16:42.000000 xplainable_client-1.2.2/xplainable_client/client/_client_cog_base.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     7365 2024-05-16 09:16:42.000000 xplainable_client-1.2.2/xplainable_client/client/_collections.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     1245 2024-05-16 09:16:42.000000 xplainable_client-1.2.2/xplainable_client/client/_datasets.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)    14645 2024-05-16 09:16:42.000000 xplainable_client-1.2.2/xplainable_client/client/_deployments.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     1219 2024-05-16 09:16:42.000000 xplainable_client-1.2.2/xplainable_client/client/_gpt.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     1234 2024-05-16 09:16:42.000000 xplainable_client-1.2.2/xplainable_client/client/_inference.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     8313 2024-05-16 09:16:42.000000 xplainable_client-1.2.2/xplainable_client/client/_misc.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)    17210 2024-05-16 09:16:42.000000 xplainable_client-1.2.2/xplainable_client/client/_models.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     9371 2024-05-16 09:16:42.000000 xplainable_client-1.2.2/xplainable_client/client/_preprocessing.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     3919 2024-05-16 09:16:42.000000 xplainable_client-1.2.2/xplainable_client/client/_session.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-16 09:20:25.803970 xplainable_client-1.2.2/xplainable_client/models/
+-rw-r--r--   0 jtuppack   (501) staff       (20)     4057 2024-03-04 22:40:48.000000 xplainable_client-1.2.2/xplainable_client/models/ebm.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-16 09:20:25.806211 xplainable_client-1.2.2/xplainable_client/utils/
+-rw-r--r--   0 jtuppack   (501) staff       (20)        0 2024-02-12 08:30:29.000000 xplainable_client-1.2.2/xplainable_client/utils/__init__.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     1291 2024-02-11 21:43:09.000000 xplainable_client-1.2.2/xplainable_client/utils/encoders.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)      180 2024-02-11 21:51:39.000000 xplainable_client-1.2.2/xplainable_client/utils/exceptions.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)      980 2024-02-11 21:45:45.000000 xplainable_client-1.2.2/xplainable_client/utils/helpers.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     6426 2024-02-12 08:36:49.000000 xplainable_client-1.2.2/xplainable_client/utils/metrics.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     3042 2024-02-11 21:51:47.000000 xplainable_client-1.2.2/xplainable_client/utils/model_parsers.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-16 09:20:25.806607 xplainable_client-1.2.2/xplainable_client.egg-info/
+-rw-r--r--   0 jtuppack   (501) staff       (20)     4705 2024-05-16 09:20:25.000000 xplainable_client-1.2.2/xplainable_client.egg-info/PKG-INFO
+-rw-r--r--   0 jtuppack   (501) staff       (20)      905 2024-05-16 09:20:25.000000 xplainable_client-1.2.2/xplainable_client.egg-info/SOURCES.txt
+-rw-r--r--   0 jtuppack   (501) staff       (20)        1 2024-05-16 09:20:25.000000 xplainable_client-1.2.2/xplainable_client.egg-info/dependency_links.txt
+-rw-r--r--   0 jtuppack   (501) staff       (20)      138 2024-05-16 09:20:25.000000 xplainable_client-1.2.2/xplainable_client.egg-info/requires.txt
+-rw-r--r--   0 jtuppack   (501) staff       (20)       29 2024-05-16 09:20:25.000000 xplainable_client-1.2.2/xplainable_client.egg-info/top_level.txt
```

### Comparing `xplainable-client-1.2.1.post4/PKG-INFO` & `xplainable_client-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: xplainable-client
-Version: 1.2.1.post4
+Version: 1.2.2
 Summary: The client for persisting and deploying models to Xplainable cloud.
 Author-email: xplainable pty ltd <contact@xplainable.io>
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: ipywidgets==8.0.6
-Requires-Dist: numpy==1.21.1
+Requires-Dist: numpy>=1.20.3
 Requires-Dist: pandas<=1.9.0,>=1.5.2
 Requires-Dist: pyperclip==1.8.2
 Requires-Dist: Requests==2.31.0
 Requires-Dist: scikit_learn
 Requires-Dist: setuptools
 Requires-Dist: urllib3==2.2.0
-Requires-Dist: xplainable==1.2.1
+Requires-Dist: xplainable
 
 
 <div align="center">
 <img src="https://raw.githubusercontent.com/xplainable/xplainable/main/docs/assets/logo/xplainable-logo.png">
 <h1 align="center">xplainable</h1>
 <h3 align="center">Real-time explainable machine learning for business optimisation</h3>
```

### Comparing `xplainable-client-1.2.1.post4/README.md` & `xplainable_client-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `xplainable-client-1.2.1.post4/pyproject.toml` & `xplainable_client-1.2.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages]
 find = {} 
 
 [project]
 name = "xplainable-client"
-version = "1.2.1-4"
+version = "1.2.2"
 authors = [
   { name="xplainable pty ltd", email="contact@xplainable.io" },
 ]
 description = "The client for persisting and deploying models to Xplainable cloud."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
@@ -22,16 +22,16 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent"
 ]
 
 dependencies = [
 "ipywidgets==8.0.6",
-"numpy==1.21.1",
+"numpy>=1.20.3",
 "pandas>=1.5.2,<=1.9.0",
 "pyperclip==1.8.2",
 "Requests==2.31.0",
 "scikit_learn",
 "setuptools",
 "urllib3==2.2.0",
-"xplainable==1.2.1"
+"xplainable"
 ]
```

### Comparing `xplainable-client-1.2.1.post4/xplainable_client/datasets.py` & `xplainable_client-1.2.2/xplainable_client/client/_datasets.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,51 @@
+from ._client_cog_base import *
+
 import requests
 import pandas as pd
 
-def list_datasets():
 
-    response = requests.get('https://api.xplainable.io/v1/public-datasets')
-    
-    if response.status_code != 200:
-        raise ValueError(f'Unable to list datasets. Check your connection and try again.')
-    
-    return  response.json()
-
-def _get_url_path(name):
-    _base = 'xplainablepublic'
-    _type = 'blob.core.windows.net'
-    _loc = 'asset-repository/datasets'
-
-    return f'https://{_base}.{_type}/{_loc}/{name}/data.csv'
-
-def load_dataset(name):
-
-    if name not in list_datasets():
-        raise ValueError(f'{name} is not available. Run xp.list_datasets() to see available datasets.')
-    
-    try:
-        url = _get_url_path(name)
-        df = pd.read_csv(url)
-
-        return df
-    
-    except Exception as e:
-        raise ValueError(f'Unable to load dataset {name}. Check your connection and try again.')
+class Datasets(Client_Cog):
+
+    # upload_dataset
+
+    def list_datasets(self):
+
+        response = requests.get('https://api.xplainable.io/v1/public-datasets')
+        
+        if response.status_code != 200:
+            raise ValueError(f'Unable to list datasets. Check your connection and try again.')
+        
+        return response.json()
+
+    def _get_url_path(self, name):
+        _base = 'xplainablepublic'
+        _type = 'blob.core.windows.net'
+        _loc = 'asset-repository/datasets'
+
+        return f'https://{_base}.{_type}/{_loc}/{name}/data.csv'
+
+    def load_dataset(self, name):
+
+        datasets = self.list_datasets()
+
+        if name not in datasets:
+            raise ValueError(f'{name} is not available. Run xp.list_datasets() to see available datasets.')
+        
+        try:
+            url = self._get_url_path(name)
+            df = pd.read_csv(url)
+
+            return df
+        
+        except Exception as e:
+            raise ValueError(f'Unable to load dataset {name}. Check your connection and try again.')
+        
+    # update_dataset
+
+    # detele_dataset
+
+    # list_dataset_children
+
+    # preview_dataset
+
+    # list_pub_datasets
```

### Comparing `xplainable-client-1.2.1.post4/xplainable_client/utils/encoders.py` & `xplainable_client-1.2.2/xplainable_client/utils/encoders.py`

 * *Files identical despite different names*

### Comparing `xplainable-client-1.2.1.post4/xplainable_client/utils/helpers.py` & `xplainable_client-1.2.2/xplainable_client/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `xplainable-client-1.2.1.post4/xplainable_client/utils/metrics.py` & `xplainable_client-1.2.2/xplainable_client/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `xplainable-client-1.2.1.post4/xplainable_client/utils/model_parsers.py` & `xplainable_client-1.2.2/xplainable_client/utils/model_parsers.py`

 * *Files identical despite different names*

### Comparing `xplainable-client-1.2.1.post4/xplainable_client.egg-info/PKG-INFO` & `xplainable_client-1.2.2/xplainable_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: xplainable-client
-Version: 1.2.1.post4
+Version: 1.2.2
 Summary: The client for persisting and deploying models to Xplainable cloud.
 Author-email: xplainable pty ltd <contact@xplainable.io>
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: ipywidgets==8.0.6
-Requires-Dist: numpy==1.21.1
+Requires-Dist: numpy>=1.20.3
 Requires-Dist: pandas<=1.9.0,>=1.5.2
 Requires-Dist: pyperclip==1.8.2
 Requires-Dist: Requests==2.31.0
 Requires-Dist: scikit_learn
 Requires-Dist: setuptools
 Requires-Dist: urllib3==2.2.0
-Requires-Dist: xplainable==1.2.1
+Requires-Dist: xplainable
 
 
 <div align="center">
 <img src="https://raw.githubusercontent.com/xplainable/xplainable/main/docs/assets/logo/xplainable-logo.png">
 <h1 align="center">xplainable</h1>
 <h3 align="center">Real-time explainable machine learning for business optimisation</h3>
```

