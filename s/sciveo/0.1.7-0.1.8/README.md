# Comparing `tmp/sciveo-0.1.7.tar.gz` & `tmp/sciveo-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sciveo-0.1.7.tar", last modified: Sun Apr 21 12:24:13 2024, max compression
+gzip compressed data, was "sciveo-0.1.8.tar", last modified: Mon May  6 11:13:19 2024, max compression
```

## Comparing `sciveo-0.1.7.tar` & `sciveo-0.1.8.tar`

### file list

```diff
@@ -1,48 +1,51 @@
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-21 12:24:13.653784 sciveo-0.1.7/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     6753 2024-04-21 12:24:13.653586 sciveo-0.1.7/PKG-INFO
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     6601 2024-04-19 15:11:15.000000 sciveo-0.1.7/README.md
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-21 12:24:13.569367 sciveo-0.1.7/sciveo/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1428 2024-04-17 12:51:40.000000 sciveo-0.1.7/sciveo/__init__.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-21 12:24:13.619179 sciveo-0.1.7/sciveo/api/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:04:12.000000 sciveo-0.1.7/sciveo/api/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1788 2024-04-16 17:39:04.000000 sciveo-0.1.7/sciveo/api/base.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1815 2024-04-05 16:37:24.000000 sciveo-0.1.7/sciveo/api/upload.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-21 12:24:13.623110 sciveo-0.1.7/sciveo/common/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:03:59.000000 sciveo-0.1.7/sciveo/common/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     2043 2024-03-14 17:02:24.000000 sciveo-0.1.7/sciveo/common/configuration.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1583 2024-03-14 17:02:24.000000 sciveo-0.1.7/sciveo/common/model.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     3842 2024-04-07 18:52:23.000000 sciveo-0.1.7/sciveo/common/optimizers.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)    10567 2024-03-19 14:47:24.000000 sciveo-0.1.7/sciveo/common/sampling.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-21 12:24:13.637089 sciveo-0.1.7/sciveo/common/tools/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:07:07.000000 sciveo-0.1.7/sciveo/common/tools/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1647 2024-04-17 12:51:40.000000 sciveo-0.1.7/sciveo/common/tools/daemon.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1053 2023-11-17 12:42:35.000000 sciveo-0.1.7/sciveo/common/tools/formating.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1654 2024-04-21 12:16:37.000000 sciveo-0.1.7/sciveo/common/tools/hardware.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1071 2023-11-15 15:21:05.000000 sciveo-0.1.7/sciveo/common/tools/logger.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1333 2024-04-17 12:51:40.000000 sciveo-0.1.7/sciveo/common/tools/synchronized.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1087 2024-04-17 12:51:40.000000 sciveo-0.1.7/sciveo/common/tools/timers.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-21 12:24:13.647061 sciveo-0.1.7/sciveo/content/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:14:23.000000 sciveo-0.1.7/sciveo/content/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      827 2024-03-14 17:02:24.000000 sciveo-0.1.7/sciveo/content/dataset.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     5859 2024-04-07 18:52:23.000000 sciveo-0.1.7/sciveo/content/experiment.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     3129 2024-04-07 18:52:23.000000 sciveo-0.1.7/sciveo/content/project.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     2015 2024-03-19 14:47:07.000000 sciveo-0.1.7/sciveo/content/runner.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-21 12:24:13.650354 sciveo-0.1.7/sciveo/monitoring/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2024-04-07 18:52:23.000000 sciveo-0.1.7/sciveo/monitoring/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     5898 2024-04-21 12:22:43.000000 sciveo-0.1.7/sciveo/monitoring/monitor.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     3790 2024-04-21 07:50:35.000000 sciveo-0.1.7/sciveo/monitoring/network.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1671 2024-04-17 12:51:40.000000 sciveo-0.1.7/sciveo/monitoring/start.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)       23 2024-04-21 12:24:10.000000 sciveo-0.1.7/sciveo/version.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-21 12:24:13.616927 sciveo-0.1.7/sciveo.egg-info/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     6753 2024-04-21 12:24:13.000000 sciveo-0.1.7/sciveo.egg-info/PKG-INFO
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      965 2024-04-21 12:24:13.000000 sciveo-0.1.7/sciveo.egg-info/SOURCES.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        1 2024-04-21 12:24:13.000000 sciveo-0.1.7/sciveo.egg-info/dependency_links.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      112 2024-04-21 12:24:13.000000 sciveo-0.1.7/sciveo.egg-info/requires.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        7 2024-04-21 12:24:13.000000 sciveo-0.1.7/sciveo.egg-info/top_level.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)       38 2024-04-21 12:24:13.653845 sciveo-0.1.7/setup.cfg
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      778 2024-04-17 12:51:40.000000 sciveo-0.1.7/setup.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-21 12:24:13.653228 sciveo-0.1.7/test/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      521 2024-03-14 17:02:24.000000 sciveo-0.1.7/test/test_configuration.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     3256 2024-04-10 18:44:45.000000 sciveo-0.1.7/test/test_monitoring.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1554 2024-03-19 14:47:07.000000 sciveo-0.1.7/test/test_runner.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     9045 2024-03-19 14:47:24.000000 sciveo-0.1.7/test/test_sampling.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-05-06 11:13:19.841565 sciveo-0.1.8/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     6829 2024-05-06 11:13:19.841400 sciveo-0.1.8/PKG-INFO
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     6677 2024-05-06 11:12:30.000000 sciveo-0.1.8/README.md
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-05-06 11:13:19.817572 sciveo-0.1.8/sciveo/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1428 2024-04-17 12:51:40.000000 sciveo-0.1.8/sciveo/__init__.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-05-06 11:13:19.825704 sciveo-0.1.8/sciveo/api/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:04:12.000000 sciveo-0.1.8/sciveo/api/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1873 2024-05-06 10:10:30.000000 sciveo-0.1.8/sciveo/api/base.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1815 2024-04-05 16:37:24.000000 sciveo-0.1.8/sciveo/api/upload.py
+-rwxr-xr-x   0 sgeorgiev   (501) staff       (20)     1192 2024-05-06 10:11:13.000000 sciveo-0.1.8/sciveo/cli.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-05-06 11:13:19.828107 sciveo-0.1.8/sciveo/common/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:03:59.000000 sciveo-0.1.8/sciveo/common/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     2043 2024-03-14 17:02:24.000000 sciveo-0.1.8/sciveo/common/configuration.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1583 2024-03-14 17:02:24.000000 sciveo-0.1.8/sciveo/common/model.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     3842 2024-04-07 18:52:23.000000 sciveo-0.1.8/sciveo/common/optimizers.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)    10567 2024-03-19 14:47:24.000000 sciveo-0.1.8/sciveo/common/sampling.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-05-06 11:13:19.831650 sciveo-0.1.8/sciveo/common/tools/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:07:07.000000 sciveo-0.1.8/sciveo/common/tools/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1744 2024-05-06 10:29:34.000000 sciveo-0.1.8/sciveo/common/tools/configuration.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1647 2024-04-17 12:51:40.000000 sciveo-0.1.8/sciveo/common/tools/daemon.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1053 2023-11-17 12:42:35.000000 sciveo-0.1.8/sciveo/common/tools/formating.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1654 2024-04-21 12:16:37.000000 sciveo-0.1.8/sciveo/common/tools/hardware.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1145 2024-05-06 10:13:15.000000 sciveo-0.1.8/sciveo/common/tools/logger.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1333 2024-04-17 12:51:40.000000 sciveo-0.1.8/sciveo/common/tools/synchronized.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1087 2024-04-17 12:51:40.000000 sciveo-0.1.8/sciveo/common/tools/timers.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-05-06 11:13:19.833562 sciveo-0.1.8/sciveo/content/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:14:23.000000 sciveo-0.1.8/sciveo/content/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      827 2024-03-14 17:02:24.000000 sciveo-0.1.8/sciveo/content/dataset.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     5859 2024-04-07 18:52:23.000000 sciveo-0.1.8/sciveo/content/experiment.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     3129 2024-04-07 18:52:23.000000 sciveo-0.1.8/sciveo/content/project.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     2015 2024-03-19 14:47:07.000000 sciveo-0.1.8/sciveo/content/runner.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-05-06 11:13:19.835942 sciveo-0.1.8/sciveo/monitoring/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2024-04-07 18:52:23.000000 sciveo-0.1.8/sciveo/monitoring/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     5903 2024-04-21 12:33:00.000000 sciveo-0.1.8/sciveo/monitoring/monitor.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     3790 2024-04-21 07:50:35.000000 sciveo-0.1.8/sciveo/monitoring/network.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1671 2024-04-17 12:51:40.000000 sciveo-0.1.8/sciveo/monitoring/start.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)       23 2024-05-06 05:53:05.000000 sciveo-0.1.8/sciveo/version.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-05-06 11:13:19.824403 sciveo-0.1.8/sciveo.egg-info/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     6829 2024-05-06 11:13:19.000000 sciveo-0.1.8/sciveo.egg-info/PKG-INFO
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1049 2024-05-06 11:13:19.000000 sciveo-0.1.8/sciveo.egg-info/SOURCES.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        1 2024-05-06 11:13:19.000000 sciveo-0.1.8/sciveo.egg-info/dependency_links.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)       43 2024-05-06 11:13:19.000000 sciveo-0.1.8/sciveo.egg-info/entry_points.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      112 2024-05-06 11:13:19.000000 sciveo-0.1.8/sciveo.egg-info/requires.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        7 2024-05-06 11:13:19.000000 sciveo-0.1.8/sciveo.egg-info/top_level.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)       38 2024-05-06 11:13:19.841624 sciveo-0.1.8/setup.cfg
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      901 2024-05-06 09:54:04.000000 sciveo-0.1.8/setup.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-05-06 11:13:19.840989 sciveo-0.1.8/test/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      521 2024-03-14 17:02:24.000000 sciveo-0.1.8/test/test_configuration.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     3256 2024-04-10 18:44:45.000000 sciveo-0.1.8/test/test_monitoring.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1554 2024-03-19 14:47:07.000000 sciveo-0.1.8/test/test_runner.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     9045 2024-03-19 14:47:24.000000 sciveo-0.1.8/test/test_sampling.py
```

### Comparing `sciveo-0.1.7/PKG-INFO` & `sciveo-0.1.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sciveo
-Version: 0.1.7
+Version: 0.1.8
 Description-Content-Type: text/markdown
 Provides-Extra: mon
 Provides-Extra: net
 Provides-Extra: all
 
 # SCIVEO - ML/AI and Scientific tools
 
@@ -45,18 +45,20 @@
 
 The library has local and remote mode. The local one is ready to use, but for the remote one you will need a sciveo.com account.
 
 When have sciveo account:
 ```shell
 export SCIVEO_SECRET_ACCESS_KEY='my_sciveo_user_auth_token'
 ```
+or create a file like ~/.sciveo/some_file_name where put:
+secret_access_key=my_sciveo_user_auth_token
 
 When using sciveo Monitoring just run, using suitable python environment
 ```shell
-python -c "import sciveo; sciveo.monitor(period=120)"
+sciveo monitor --period 120
 ```
 
 Monitoring started along with other python code.
 ```python
 import sciveo
 
 # Non blocking monitoring, so continue the code execution after it.
```

### Comparing `sciveo-0.1.7/README.md` & `sciveo-0.1.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -37,18 +37,20 @@
 
 The library has local and remote mode. The local one is ready to use, but for the remote one you will need a sciveo.com account.
 
 When have sciveo account:
 ```shell
 export SCIVEO_SECRET_ACCESS_KEY='my_sciveo_user_auth_token'
 ```
+or create a file like ~/.sciveo/some_file_name where put:
+secret_access_key=my_sciveo_user_auth_token
 
 When using sciveo Monitoring just run, using suitable python environment
 ```shell
-python -c "import sciveo; sciveo.monitor(period=120)"
+sciveo monitor --period 120
 ```
 
 Monitoring started along with other python code.
 ```python
 import sciveo
 
 # Non blocking monitoring, so continue the code execution after it.
```

### Comparing `sciveo-0.1.7/sciveo/__init__.py` & `sciveo-0.1.8/sciveo/__init__.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.7/sciveo/api/base.py` & `sciveo-0.1.8/sciveo/api/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,22 +11,25 @@
 
 import os
 import json
 from urllib import request, parse
 from urllib.error import HTTPError
 
 from sciveo.common.tools.logger import *
+from sciveo.common.tools.configuration import GlobalConfiguration
 
 
 class APIRemoteClient:
   def __init__(self, base_url=None, ver=1):
+    self.config = GlobalConfiguration.get()
+    self.auth_token = None
     if base_url is None:
-      base_url = os.environ.get("SCIVEO_API_BASE_URL", "https://sciveo.com")
+      base_url = self.config["api_base_url"]
     self.base_url = f"{base_url}/api/v{ver}/"
-    self.headers = { "Auth-Token": os.environ.get('SCIVEO_SECRET_ACCESS_KEY', "") }
+    self.headers = { "Auth-Token": self.config['secret_access_key'] }
     debug(type(self).__name__, f"base url: {self.base_url}")
 
   def POST_SCI(self, content_type, data, timeout=30):
     return self.POST(f"sci/{content_type}/", data, timeout)
 
   def POST(self, url, data, timeout=30):
     url = f"{self.base_url}{url}"
@@ -40,15 +43,15 @@
     except HTTPError as e:
       error(e, url, data)
     except Exception as e:
       error(e, url, data)
     return result
 
   def GET(self, url, timeout=30):
-    url = f"{self.base_url}{url}&auth_token={os.environ['SCIVEO_SECRET_ACCESS_KEY']}"
+    url = f"{self.base_url}{url}&auth_token={self.config['secret_access_key']}"
     result = False
     try:
       # debug("GET", url)
       resp = request.urlopen(request.Request(url, headers=self.headers), timeout=timeout)
       result = json.loads(resp.read())
       # debug("GET", resp.status, result)
     except HTTPError as e:
```

### Comparing `sciveo-0.1.7/sciveo/api/upload.py` & `sciveo-0.1.8/sciveo/api/upload.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.7/sciveo/common/configuration.py` & `sciveo-0.1.8/sciveo/common/configuration.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.7/sciveo/common/model.py` & `sciveo-0.1.8/sciveo/common/model.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.7/sciveo/common/optimizers.py` & `sciveo-0.1.8/sciveo/common/optimizers.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.7/sciveo/common/sampling.py` & `sciveo-0.1.8/sciveo/common/sampling.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.7/sciveo/common/tools/daemon.py` & `sciveo-0.1.8/sciveo/common/tools/daemon.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.7/sciveo/common/tools/formating.py` & `sciveo-0.1.8/sciveo/common/tools/formating.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.7/sciveo/common/tools/hardware.py` & `sciveo-0.1.8/sciveo/common/tools/hardware.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.7/sciveo/common/tools/logger.py` & `sciveo-0.1.8/sciveo/common/tools/logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,16 +9,19 @@
 # 2023
 #
 
 import os
 import logging
 import threading
 
+from sciveo.common.tools.configuration import GlobalConfiguration
 
-log_min_level = os.environ.setdefault('SCI_LOG_MIN_LEVEL', "DEBUG")
+
+config = GlobalConfiguration.get()
+log_min_level = config["LOG_MIN_LEVEL"]
 
 def get_logger(name):
   logger = logging.getLogger(name)
 
   if not logger.handlers:
     logger.setLevel(logging.getLevelName(log_min_level))
     formatter = logging.Formatter('%(asctime)s [%(thread)d] [%(levelname)s] %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
```

### Comparing `sciveo-0.1.7/sciveo/common/tools/synchronized.py` & `sciveo-0.1.8/sciveo/common/tools/synchronized.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.7/sciveo/common/tools/timers.py` & `sciveo-0.1.8/sciveo/common/tools/timers.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.7/sciveo/content/dataset.py` & `sciveo-0.1.8/sciveo/content/dataset.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.7/sciveo/content/experiment.py` & `sciveo-0.1.8/sciveo/content/experiment.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.7/sciveo/content/project.py` & `sciveo-0.1.8/sciveo/content/project.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.7/sciveo/content/runner.py` & `sciveo-0.1.8/sciveo/content/runner.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.7/sciveo/monitoring/monitor.py` & `sciveo-0.1.8/sciveo/monitoring/monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
       pass
 
   def get_temperatures(self):
     try:
       temperatures = psutil.sensors_temperatures()
       for k, v in temperatures.items():
         self.data["TEMP"][k] = [t.current for t in v]
-    except Exception:
+    except Exception as e:
       pass
 
   def get_memory(self):
     try:
       memory = psutil.virtual_memory()
       self.data["RAM"]["used"] = memory.used
       self.data["RAM"]["total"] = memory.total
```

### Comparing `sciveo-0.1.7/sciveo/monitoring/network.py` & `sciveo-0.1.8/sciveo/monitoring/network.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.7/sciveo/monitoring/start.py` & `sciveo-0.1.8/sciveo/monitoring/start.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.7/sciveo.egg-info/PKG-INFO` & `sciveo-0.1.8/sciveo.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sciveo
-Version: 0.1.7
+Version: 0.1.8
 Description-Content-Type: text/markdown
 Provides-Extra: mon
 Provides-Extra: net
 Provides-Extra: all
 
 # SCIVEO - ML/AI and Scientific tools
 
@@ -45,18 +45,20 @@
 
 The library has local and remote mode. The local one is ready to use, but for the remote one you will need a sciveo.com account.
 
 When have sciveo account:
 ```shell
 export SCIVEO_SECRET_ACCESS_KEY='my_sciveo_user_auth_token'
 ```
+or create a file like ~/.sciveo/some_file_name where put:
+secret_access_key=my_sciveo_user_auth_token
 
 When using sciveo Monitoring just run, using suitable python environment
 ```shell
-python -c "import sciveo; sciveo.monitor(period=120)"
+sciveo monitor --period 120
 ```
 
 Monitoring started along with other python code.
 ```python
 import sciveo
 
 # Non blocking monitoring, so continue the code execution after it.
```

### Comparing `sciveo-0.1.7/sciveo.egg-info/SOURCES.txt` & `sciveo-0.1.8/sciveo.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 README.md
 setup.py
 sciveo/__init__.py
+sciveo/cli.py
 sciveo/version.py
 sciveo.egg-info/PKG-INFO
 sciveo.egg-info/SOURCES.txt
 sciveo.egg-info/dependency_links.txt
+sciveo.egg-info/entry_points.txt
 sciveo.egg-info/requires.txt
 sciveo.egg-info/top_level.txt
 sciveo/api/__init__.py
 sciveo/api/base.py
 sciveo/api/upload.py
 sciveo/common/__init__.py
 sciveo/common/configuration.py
 sciveo/common/model.py
 sciveo/common/optimizers.py
 sciveo/common/sampling.py
 sciveo/common/tools/__init__.py
+sciveo/common/tools/configuration.py
 sciveo/common/tools/daemon.py
 sciveo/common/tools/formating.py
 sciveo/common/tools/hardware.py
 sciveo/common/tools/logger.py
 sciveo/common/tools/synchronized.py
 sciveo/common/tools/timers.py
 sciveo/content/__init__.py
```

### Comparing `sciveo-0.1.7/setup.py` & `sciveo-0.1.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,8 +30,14 @@
         'netifaces>=0.0.0',
       ],
       'all': [
         'psutil>=0.0.0',
         'netifaces>=0.0.0',
       ]
     },
+    py_modules=['sciveo'],
+    entry_points={
+      'console_scripts': [
+        'sciveo=sciveo.cli:main',
+      ],
+    },
 )
```

### Comparing `sciveo-0.1.7/test/test_configuration.py` & `sciveo-0.1.8/test/test_configuration.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.7/test/test_monitoring.py` & `sciveo-0.1.8/test/test_monitoring.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.7/test/test_runner.py` & `sciveo-0.1.8/test/test_runner.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.7/test/test_sampling.py` & `sciveo-0.1.8/test/test_sampling.py`

 * *Files identical despite different names*

