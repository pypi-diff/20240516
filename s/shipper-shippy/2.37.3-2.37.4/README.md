# Comparing `tmp/shipper_shippy-2.37.3.tar.gz` & `tmp/shipper_shippy-2.37.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipper_shippy-2.37.3.tar", last modified: Mon May 13 14:53:08 2024, max compression
+gzip compressed data, was "shipper_shippy-2.37.4.tar", last modified: Thu May 16 15:17:17 2024, max compression
```

## Comparing `shipper_shippy-2.37.3.tar` & `shipper_shippy-2.37.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:53:08.974973 shipper_shippy-2.37.3/
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-13 14:53:08.974973 shipper_shippy-2.37.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-13 14:52:57.000000 shipper_shippy-2.37.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-13 14:52:57.000000 shipper_shippy-2.37.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 14:53:08.974973 shipper_shippy-2.37.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-13 14:52:57.000000 shipper_shippy-2.37.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:53:08.974973 shipper_shippy-2.37.3/shipper_shippy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-13 14:53:08.000000 shipper_shippy-2.37.3/shipper_shippy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-13 14:53:08.000000 shipper_shippy-2.37.3/shipper_shippy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 14:53:08.000000 shipper_shippy-2.37.3/shipper_shippy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-13 14:53:08.000000 shipper_shippy-2.37.3/shipper_shippy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-13 14:53:08.000000 shipper_shippy-2.37.3/shipper_shippy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-13 14:53:08.000000 shipper_shippy-2.37.3/shipper_shippy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:53:08.974973 shipper_shippy-2.37.3/shippy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 14:52:57.000000 shipper_shippy-2.37.3/shippy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12436 2024-05-13 14:52:57.000000 shipper_shippy-2.37.3/shippy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14072 2024-05-13 14:52:57.000000 shipper_shippy-2.37.3/shippy/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-13 14:52:57.000000 shipper_shippy-2.37.3/shippy/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-13 14:52:57.000000 shipper_shippy-2.37.3/shippy/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-13 14:52:57.000000 shipper_shippy-2.37.3/shippy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-13 14:52:57.000000 shipper_shippy-2.37.3/shippy/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-13 14:52:57.000000 shipper_shippy-2.37.3/shippy/server_compat_version.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-13 14:52:57.000000 shipper_shippy-2.37.3/shippy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:17:17.938259 shipper_shippy-2.37.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-16 15:17:17.938259 shipper_shippy-2.37.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-16 15:17:09.000000 shipper_shippy-2.37.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-16 15:17:09.000000 shipper_shippy-2.37.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 15:17:17.942259 shipper_shippy-2.37.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-16 15:17:09.000000 shipper_shippy-2.37.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:17:17.938259 shipper_shippy-2.37.4/shipper_shippy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-16 15:17:17.000000 shipper_shippy-2.37.4/shipper_shippy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-16 15:17:17.000000 shipper_shippy-2.37.4/shipper_shippy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 15:17:17.000000 shipper_shippy-2.37.4/shipper_shippy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-16 15:17:17.000000 shipper_shippy-2.37.4/shipper_shippy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-16 15:17:17.000000 shipper_shippy-2.37.4/shipper_shippy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-16 15:17:17.000000 shipper_shippy-2.37.4/shipper_shippy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:17:17.938259 shipper_shippy-2.37.4/shippy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 15:17:09.000000 shipper_shippy-2.37.4/shippy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12436 2024-05-16 15:17:09.000000 shipper_shippy-2.37.4/shippy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14705 2024-05-16 15:17:09.000000 shipper_shippy-2.37.4/shippy/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-16 15:17:09.000000 shipper_shippy-2.37.4/shippy/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-16 15:17:09.000000 shipper_shippy-2.37.4/shippy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-16 15:17:09.000000 shipper_shippy-2.37.4/shippy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-16 15:17:09.000000 shipper_shippy-2.37.4/shippy/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-16 15:17:09.000000 shipper_shippy-2.37.4/shippy/server_compat_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-16 15:17:09.000000 shipper_shippy-2.37.4/shippy/version.py
```

### Comparing `shipper_shippy-2.37.3/PKG-INFO` & `shipper_shippy-2.37.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipper-shippy
-Version: 2.37.3
+Version: 2.37.4
 Summary: Client-side tool to interface with shipper
 Home-page: https://github.com/shipperstack/shipper/tree/master/shippy
 Author: Eric Park
 Author-email: me@ericswpark.com
 Project-URL: Bug Tracker, https://github.com/shipperstack/shipper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shipper_shippy-2.37.3/README.md` & `shipper_shippy-2.37.4/README.md`

 * *Files identical despite different names*

### Comparing `shipper_shippy-2.37.3/setup.py` & `shipper_shippy-2.37.4/setup.py`

 * *Files identical despite different names*

### Comparing `shipper_shippy-2.37.3/shipper_shippy.egg-info/PKG-INFO` & `shipper_shippy-2.37.4/shipper_shippy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipper-shippy
-Version: 2.37.3
+Version: 2.37.4
 Summary: Client-side tool to interface with shipper
 Home-page: https://github.com/shipperstack/shipper/tree/master/shippy
 Author: Eric Park
 Author-email: me@ericswpark.com
 Project-URL: Bug Tracker, https://github.com/shipperstack/shipper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shipper_shippy-2.37.3/shippy/__main__.py` & `shipper_shippy-2.37.4/shippy/__main__.py`

 * *Files identical despite different names*

### Comparing `shipper_shippy-2.37.3/shippy/client.py` & `shipper_shippy-2.37.4/shippy/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,16 @@
     UNKNOWN_UPLOAD_START_ERROR_MSG,
     UPLOAD_SUCCESSFUL_MSG,
     WAITING_FINALIZATION_MSG,
     CHUNK_SIZE,
     INTERNAL_SERVER_ERROR_MSG,
     FOUND_PREVIOUS_BUILD_ATTEMPT_MSG,
     DISABLE_BUILD_FAILED_MSG,
+    SERVER_ERROR_WAITING_MSG,
+    SERVER_ERROR_WAIT_STATUS_MSG,
 )
 from .exceptions import LoginException, UploadException
 from .version import __version__
 from .server_compat_version import server_compat_version
 
 console = Console()
 
@@ -81,14 +83,22 @@
     with console.status(RATE_LIMIT_WAIT_STATUS_MSG.format(seconds)) as status:
         while seconds:
             time.sleep(1)
             seconds -= 1
             status.update(status=RATE_LIMIT_WAIT_STATUS_MSG.format(seconds))
 
 
+def wait_temporary_error(seconds):
+    with console.status(SERVER_ERROR_WAIT_STATUS_MSG.format(seconds)) as status:
+        while seconds:
+            time.sleep(1)
+            seconds -= 1
+            status.update(status=SERVER_ERROR_WAIT_STATUS_MSG.format(seconds))
+
+
 class Client:
     def __init__(self, server_url, token=None):
         self.server_url = server_url
         self.token = token
 
     def is_url_secure(self):
         return self.server_url[0:5] == "https"
@@ -339,14 +349,23 @@
             print(RATE_LIMIT_MSG)
             wait_rate_limit(int(re.findall(r"\d+", r.json()["detail"])[0]))
 
             return self._request(
                 type=type, url=url, headers=headers, data=data, files=files
             )
 
+        # Check for temporary server-side errors
+        if int(r.status_code / 100) == 5:
+            print(SERVER_ERROR_WAITING_MSG)
+            wait_temporary_error(30)
+
+            return self._request(
+                type=type, url=url, headers=headers, data=data, files=files
+            )
+
         return r
 
     def _post(self, url, headers=None, data=None):
         return self._request("POST", url, headers, data)
 
     def _get(self, url, headers=None, data=None):
         return self._request("GET", url, headers, data)
```

### Comparing `shipper_shippy-2.37.3/shippy/config.py` & `shipper_shippy-2.37.4/shippy/config.py`

 * *Files identical despite different names*

### Comparing `shipper_shippy-2.37.3/shippy/constants.py` & `shipper_shippy-2.37.4/shippy/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,14 +54,20 @@
 
 RATE_LIMIT_MSG = "shippy has been rate limited."
 RATE_LIMIT_WAIT_STATUS_MSG = (
     "Waiting to resume after being rate limited. shippy will "
     "resume uploading in {} seconds."
 )
 
+SERVER_ERROR_WAITING_MSG = "The server is temporarily unavailable."
+SERVER_ERROR_WAIT_STATUS_MSG = (
+    "Waiting to resume as the server is temporarily unavailable. "
+    "shippy will automatically retry in {} seconds."
+)
+
 WAITING_FINALIZATION_MSG = (
     "Waiting for the server to process the uploaded build. "
     "This may take around 30 seconds..."
 )
 
 BUILD_DISABLED_MSG = "Build {} has been disabled."
```

### Comparing `shipper_shippy-2.37.3/shippy/helper.py` & `shipper_shippy-2.37.4/shippy/helper.py`

 * *Files identical despite different names*

