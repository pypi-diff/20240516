# Comparing `tmp/prefect_azure-0.3.8.tar.gz` & `tmp/prefect_azure-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect_azure-0.3.8.tar", last modified: Wed Apr 24 14:11:06 2024, max compression
+gzip compressed data, was "prefect_azure-0.3.9.tar", last modified: Fri Apr 26 15:03:56 2024, max compression
```

## Comparing `prefect_azure-0.3.8.tar` & `prefect_azure-0.3.9.tar`

### file list

```diff
@@ -1,39 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:11:06.384748 prefect_azure-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-04-24 14:11:06.384748 prefect_azure-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-24 14:10:54.000000 prefect_azure-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:11:06.380747 prefect_azure-0.3.8/prefect_azure/
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-24 14:10:54.000000 prefect_azure-0.3.8/prefect_azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-24 14:11:06.000000 prefect_azure-0.3.8/prefect_azure/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    25910 2024-04-24 14:10:54.000000 prefect_azure-0.3.8/prefect_azure/blob_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    36429 2024-04-24 14:10:54.000000 prefect_azure-0.3.8/prefect_azure/container_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-04-24 14:10:54.000000 prefect_azure-0.3.8/prefect_azure/cosmos_db.py
--rw-r--r--   0 runner    (1001) docker     (127)    21828 2024-04-24 14:10:54.000000 prefect_azure-0.3.8/prefect_azure/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:11:06.380747 prefect_azure-0.3.8/prefect_azure/deployments/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 14:10:54.000000 prefect_azure-0.3.8/prefect_azure/deployments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7519 2024-04-24 14:10:54.000000 prefect_azure-0.3.8/prefect_azure/deployments/steps.py
--rw-r--r--   0 runner    (1001) docker     (127)     9880 2024-04-24 14:10:54.000000 prefect_azure-0.3.8/prefect_azure/ml_datastore.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 14:10:54.000000 prefect_azure-0.3.8/prefect_azure/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:11:06.380747 prefect_azure-0.3.8/prefect_azure/workers/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-24 14:10:54.000000 prefect_azure-0.3.8/prefect_azure/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39029 2024-04-24 14:10:54.000000 prefect_azure-0.3.8/prefect_azure/workers/container_instance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:11:06.384748 prefect_azure-0.3.8/prefect_azure.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-04-24 14:11:06.000000 prefect_azure-0.3.8/prefect_azure.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-24 14:11:06.000000 prefect_azure-0.3.8/prefect_azure.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 14:11:06.000000 prefect_azure-0.3.8/prefect_azure.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-24 14:11:06.000000 prefect_azure-0.3.8/prefect_azure.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-24 14:11:06.000000 prefect_azure-0.3.8/prefect_azure.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-24 14:11:06.000000 prefect_azure-0.3.8/prefect_azure.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-24 14:10:54.000000 prefect_azure-0.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 14:11:06.384748 prefect_azure-0.3.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:11:06.380747 prefect_azure-0.3.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-04-24 14:10:54.000000 prefect_azure-0.3.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:11:06.384748 prefect_azure-0.3.8/tests/deployments/
--rw-r--r--   0 runner    (1001) docker     (127)    14605 2024-04-24 14:10:54.000000 prefect_azure-0.3.8/tests/deployments/test_steps.py
--rw-r--r--   0 runner    (1001) docker     (127)    37383 2024-04-24 14:10:54.000000 prefect_azure-0.3.8/tests/test_aci_infrastructure.py
--rw-r--r--   0 runner    (1001) docker     (127)    39151 2024-04-24 14:10:54.000000 prefect_azure-0.3.8/tests/test_aci_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)    10360 2024-04-24 14:10:54.000000 prefect_azure-0.3.8/tests/test_blob_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-24 14:10:54.000000 prefect_azure-0.3.8/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-24 14:10:54.000000 prefect_azure-0.3.8/tests/test_cosmos_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-04-24 14:10:54.000000 prefect_azure-0.3.8/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-04-24 14:10:54.000000 prefect_azure-0.3.8/tests/test_ml_datastore.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-24 14:10:54.000000 prefect_azure-0.3.8/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:56.337059 prefect_azure-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6317 2024-04-26 15:03:56.333059 prefect_azure-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:56.329059 prefect_azure-0.3.9/prefect_azure/
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/prefect_azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-26 15:03:55.000000 prefect_azure-0.3.9/prefect_azure/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25910 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/prefect_azure/blob_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36429 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/prefect_azure/container_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/prefect_azure/cosmos_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21828 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/prefect_azure/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:56.329059 prefect_azure-0.3.9/prefect_azure/deployments/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/prefect_azure/deployments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7519 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/prefect_azure/deployments/steps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9880 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/prefect_azure/ml_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/prefect_azure/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:56.329059 prefect_azure-0.3.9/prefect_azure/workers/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/prefect_azure/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39029 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/prefect_azure/workers/container_instance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:56.333059 prefect_azure-0.3.9/prefect_azure.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6317 2024-04-26 15:03:56.000000 prefect_azure-0.3.9/prefect_azure.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-26 15:03:56.000000 prefect_azure-0.3.9/prefect_azure.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:03:56.000000 prefect_azure-0.3.9/prefect_azure.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-26 15:03:56.000000 prefect_azure-0.3.9/prefect_azure.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-26 15:03:56.000000 prefect_azure-0.3.9/prefect_azure.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-26 15:03:56.000000 prefect_azure-0.3.9/prefect_azure.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:03:56.337059 prefect_azure-0.3.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:56.333059 prefect_azure-0.3.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:56.333059 prefect_azure-0.3.9/tests/deployments/
+-rw-r--r--   0 runner    (1001) docker     (127)    14605 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/tests/deployments/test_steps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37383 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/tests/test_aci_infrastructure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39151 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/tests/test_aci_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10360 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/tests/test_blob_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/tests/test_cosmos_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/tests/test_ml_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/tests/test_version.py
```

### Comparing `prefect_azure-0.3.8/PKG-INFO` & `prefect_azure-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-azure
-Version: 0.3.8
+Version: 0.3.9
 Summary: Prefect integrations with Microsoft Azure services
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-azure
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: azure_identity>=1.10
 Requires-Dist: azure_mgmt_containerinstance>=10.0
 Requires-Dist: azure-mgmt-resource>=21.2
 Requires-Dist: prefect>=2.14.10
 Provides-Extra: blob-storage
 Requires-Dist: azure-storage-blob; extra == "blob-storage"
```

### Comparing `prefect_azure-0.3.8/README.md` & `prefect_azure-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `prefect_azure-0.3.8/prefect_azure/__init__.py` & `prefect_azure-0.3.9/prefect_azure/__init__.py`

 * *Files identical despite different names*

### Comparing `prefect_azure-0.3.8/prefect_azure/blob_storage.py` & `prefect_azure-0.3.9/prefect_azure/blob_storage.py`

 * *Files identical despite different names*

### Comparing `prefect_azure-0.3.8/prefect_azure/container_instance.py` & `prefect_azure-0.3.9/prefect_azure/container_instance.py`

 * *Files identical despite different names*

### Comparing `prefect_azure-0.3.8/prefect_azure/cosmos_db.py` & `prefect_azure-0.3.9/prefect_azure/cosmos_db.py`

 * *Files identical despite different names*

### Comparing `prefect_azure-0.3.8/prefect_azure/credentials.py` & `prefect_azure-0.3.9/prefect_azure/credentials.py`

 * *Files identical despite different names*

### Comparing `prefect_azure-0.3.8/prefect_azure/deployments/steps.py` & `prefect_azure-0.3.9/prefect_azure/deployments/steps.py`

 * *Files identical despite different names*

### Comparing `prefect_azure-0.3.8/prefect_azure/ml_datastore.py` & `prefect_azure-0.3.9/prefect_azure/ml_datastore.py`

 * *Files identical despite different names*

### Comparing `prefect_azure-0.3.8/prefect_azure/workers/container_instance.py` & `prefect_azure-0.3.9/prefect_azure/workers/container_instance.py`

 * *Files identical despite different names*

### Comparing `prefect_azure-0.3.8/prefect_azure.egg-info/PKG-INFO` & `prefect_azure-0.3.9/prefect_azure.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-azure
-Version: 0.3.8
+Version: 0.3.9
 Summary: Prefect integrations with Microsoft Azure services
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-azure
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: azure_identity>=1.10
 Requires-Dist: azure_mgmt_containerinstance>=10.0
 Requires-Dist: azure-mgmt-resource>=21.2
 Requires-Dist: prefect>=2.14.10
 Provides-Extra: blob-storage
 Requires-Dist: azure-storage-blob; extra == "blob-storage"
```

### Comparing `prefect_azure-0.3.8/prefect_azure.egg-info/SOURCES.txt` & `prefect_azure-0.3.9/prefect_azure.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+LICENSE
+MANIFEST.in
 README.md
 pyproject.toml
 prefect_azure/__init__.py
 prefect_azure/_version.py
 prefect_azure/blob_storage.py
 prefect_azure/container_instance.py
 prefect_azure/cosmos_db.py
```

### Comparing `prefect_azure-0.3.8/pyproject.toml` & `prefect_azure-0.3.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `prefect_azure-0.3.8/tests/conftest.py` & `prefect_azure-0.3.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `prefect_azure-0.3.8/tests/deployments/test_steps.py` & `prefect_azure-0.3.9/tests/deployments/test_steps.py`

 * *Files identical despite different names*

### Comparing `prefect_azure-0.3.8/tests/test_aci_infrastructure.py` & `prefect_azure-0.3.9/tests/test_aci_infrastructure.py`

 * *Files identical despite different names*

### Comparing `prefect_azure-0.3.8/tests/test_aci_worker.py` & `prefect_azure-0.3.9/tests/test_aci_worker.py`

 * *Files identical despite different names*

### Comparing `prefect_azure-0.3.8/tests/test_blob_storage.py` & `prefect_azure-0.3.9/tests/test_blob_storage.py`

 * *Files identical despite different names*

### Comparing `prefect_azure-0.3.8/tests/test_block_standards.py` & `prefect_azure-0.3.9/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect_azure-0.3.8/tests/test_cosmos_db.py` & `prefect_azure-0.3.9/tests/test_cosmos_db.py`

 * *Files identical despite different names*

### Comparing `prefect_azure-0.3.8/tests/test_credentials.py` & `prefect_azure-0.3.9/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `prefect_azure-0.3.8/tests/test_ml_datastore.py` & `prefect_azure-0.3.9/tests/test_ml_datastore.py`

 * *Files identical despite different names*

