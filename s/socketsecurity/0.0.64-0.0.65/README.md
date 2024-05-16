# Comparing `tmp/socketsecurity-0.0.64.tar.gz` & `tmp/socketsecurity-0.0.65.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socketsecurity-0.0.64.tar", last modified: Thu May 16 11:06:14 2024, max compression
+gzip compressed data, was "socketsecurity-0.0.65.tar", last modified: Thu May 16 11:30:48 2024, max compression
```

## Comparing `socketsecurity-0.0.64.tar` & `socketsecurity-0.0.65.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 11:06:14.151124 socketsecurity-0.0.64/
--rw-r--r--   0 douglascoburn   (501) staff       (20)      771 2024-05-16 11:06:14.150951 socketsecurity-0.0.64/PKG-INFO
--rw-r--r--   0 douglascoburn   (501) staff       (20)       21 2024-05-15 04:22:36.000000 socketsecurity-0.0.64/README.md
--rw-r--r--   0 douglascoburn   (501) staff       (20)     1025 2024-05-16 11:05:43.000000 socketsecurity-0.0.64/pyproject.toml
--rw-r--r--   0 douglascoburn   (501) staff       (20)       38 2024-05-16 11:06:14.151164 socketsecurity-0.0.64/setup.cfg
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 11:06:14.140087 socketsecurity-0.0.64/socketsecurity/
--rw-r--r--   0 douglascoburn   (501) staff       (20)       98 2024-05-16 10:04:37.000000 socketsecurity-0.0.64/socketsecurity/__init__.py
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 11:06:14.150542 socketsecurity-0.0.64/socketsecurity/core/
--rw-r--r--   0 douglascoburn   (501) staff       (20)    26034 2024-05-16 11:05:47.000000 socketsecurity-0.0.64/socketsecurity/core/__init__.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)     9282 2024-05-16 08:29:16.000000 socketsecurity-0.0.64/socketsecurity/core/classes.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)      626 2024-04-29 13:52:20.000000 socketsecurity-0.0.64/socketsecurity/core/exceptions.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)    11342 2024-05-16 07:53:25.000000 socketsecurity-0.0.64/socketsecurity/core/github.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)    11041 2024-05-16 11:03:01.000000 socketsecurity-0.0.64/socketsecurity/core/gitlab.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)    68147 2024-05-16 10:03:15.000000 socketsecurity-0.0.64/socketsecurity/core/issues.py
--rw-r--r--   0 douglascoburn   (501) staff       (20) 17442610 2024-05-06 19:45:31.000000 socketsecurity-0.0.64/socketsecurity/core/licenses.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)    11849 2024-05-15 05:15:37.000000 socketsecurity-0.0.64/socketsecurity/core/messages.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)     5975 2024-05-16 10:18:06.000000 socketsecurity-0.0.64/socketsecurity/socketcli.py
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 11:06:14.150756 socketsecurity-0.0.64/socketsecurity.egg-info/
--rw-r--r--   0 douglascoburn   (501) staff       (20)      771 2024-05-16 11:06:14.000000 socketsecurity-0.0.64/socketsecurity.egg-info/PKG-INFO
--rw-r--r--   0 douglascoburn   (501) staff       (20)      560 2024-05-16 11:06:14.000000 socketsecurity-0.0.64/socketsecurity.egg-info/SOURCES.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)        1 2024-05-16 11:06:14.000000 socketsecurity-0.0.64/socketsecurity.egg-info/dependency_links.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)       59 2024-05-16 11:06:14.000000 socketsecurity-0.0.64/socketsecurity.egg-info/entry_points.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)       38 2024-05-16 11:06:14.000000 socketsecurity-0.0.64/socketsecurity.egg-info/requires.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)       15 2024-05-16 11:06:14.000000 socketsecurity-0.0.64/socketsecurity.egg-info/top_level.txt
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 11:30:48.952468 socketsecurity-0.0.65/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      771 2024-05-16 11:30:48.952289 socketsecurity-0.0.65/PKG-INFO
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       21 2024-05-15 04:22:36.000000 socketsecurity-0.0.65/README.md
+-rw-r--r--   0 douglascoburn   (501) staff       (20)     1025 2024-05-16 11:30:38.000000 socketsecurity-0.0.65/pyproject.toml
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       38 2024-05-16 11:30:48.952507 socketsecurity-0.0.65/setup.cfg
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 11:30:48.941606 socketsecurity-0.0.65/socketsecurity/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       98 2024-05-16 10:04:37.000000 socketsecurity-0.0.65/socketsecurity/__init__.py
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 11:30:48.951261 socketsecurity-0.0.65/socketsecurity/core/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    26186 2024-05-16 11:30:14.000000 socketsecurity-0.0.65/socketsecurity/core/__init__.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)     9282 2024-05-16 08:29:16.000000 socketsecurity-0.0.65/socketsecurity/core/classes.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      785 2024-05-16 11:28:29.000000 socketsecurity-0.0.65/socketsecurity/core/exceptions.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    11342 2024-05-16 07:53:25.000000 socketsecurity-0.0.65/socketsecurity/core/github.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    11041 2024-05-16 11:03:01.000000 socketsecurity-0.0.65/socketsecurity/core/gitlab.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    68147 2024-05-16 10:03:15.000000 socketsecurity-0.0.65/socketsecurity/core/issues.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20) 17442610 2024-05-06 19:45:31.000000 socketsecurity-0.0.65/socketsecurity/core/licenses.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    11849 2024-05-15 05:15:37.000000 socketsecurity-0.0.65/socketsecurity/core/messages.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)     5975 2024-05-16 10:18:06.000000 socketsecurity-0.0.65/socketsecurity/socketcli.py
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 11:30:48.952082 socketsecurity-0.0.65/socketsecurity.egg-info/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      771 2024-05-16 11:30:48.000000 socketsecurity-0.0.65/socketsecurity.egg-info/PKG-INFO
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      560 2024-05-16 11:30:48.000000 socketsecurity-0.0.65/socketsecurity.egg-info/SOURCES.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)        1 2024-05-16 11:30:48.000000 socketsecurity-0.0.65/socketsecurity.egg-info/dependency_links.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       59 2024-05-16 11:30:48.000000 socketsecurity-0.0.65/socketsecurity.egg-info/entry_points.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       38 2024-05-16 11:30:48.000000 socketsecurity-0.0.65/socketsecurity.egg-info/requires.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       15 2024-05-16 11:30:48.000000 socketsecurity-0.0.65/socketsecurity.egg-info/top_level.txt
```

### Comparing `socketsecurity-0.0.64/PKG-INFO` & `socketsecurity-0.0.65/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketsecurity
-Version: 0.0.64
+Version: 0.0.65
 Summary: Socket Security CLI for CI/CD
 Author-email: Douglas Coburn <douglas@socket.dev>
 Maintainer-email: Douglas Coburn <douglas@socket.dev>
 Project-URL: Homepage, https://socket.dev
 Keywords: socketsecurity,socket.dev,sca,oss,security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `socketsecurity-0.0.64/pyproject.toml` & `socketsecurity-0.0.65/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "socketsecurity"
-version = "0.0.64"
+version = "0.0.65"
 requires-python = ">= 3.9"
 dependencies = [
     'requests',
     'mdutils',
     'prettytable',
     'argparse'
 ]
```

### Comparing `socketsecurity-0.0.64/socketsecurity/core/__init__.py` & `socketsecurity-0.0.65/socketsecurity/core/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import logging
 import requests
 from urllib.parse import urlencode
 import base64
 import json
-from socketsecurity.core.exceptions import APIFailure, APIKeyMissing, APIAccessDenied, APIInsufficientQuota, APIResourceNotFound
+from socketsecurity.core.exceptions import (
+    APIFailure, APIKeyMissing, APIAccessDenied, APIInsufficientQuota, APIResourceNotFound, APICloudflareError
+)
 from socketsecurity.core.licenses import Licenses
 from socketsecurity.core.issues import AllIssues
 from socketsecurity.core.classes import (
     Report,
     Issue,
     Package,
     Alert,
@@ -19,15 +21,15 @@
 )
 import platform
 from glob import glob
 import time
 
 
 __author__ = 'socket.dev'
-__version__ = '0.0.64'
+__version__ = '0.0.65'
 __all__ = [
     "Core",
     "log",
     "__version__"
 ]
 
 
@@ -106,17 +108,20 @@
         raise APIAccessDenied("Unauthorized")
     elif response.status_code == 403:
         raise APIInsufficientQuota("Insufficient max_quota for API method")
     elif response.status_code == 404:
         raise APIResourceNotFound(f"Path not found {path}")
     elif response.status_code == 429:
         raise APIInsufficientQuota("Insufficient quota for API route")
+    elif response.status_code == 524:
+        raise APICloudflareError
     else:
         msg = {
-            "status_code": 524,
+            "status_code": response.status_code,
+            "error": response.text,
             "UnexpectedError": "There was an unexpected error using the API"
         }
         raise APIFailure(msg)
 
 
 class Core:
     token: str
```

### Comparing `socketsecurity-0.0.64/socketsecurity/core/classes.py` & `socketsecurity-0.0.65/socketsecurity/core/classes.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.64/socketsecurity/core/exceptions.py` & `socketsecurity-0.0.65/socketsecurity/core/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 __all__ = [
     "APIFailure",
     "APIKeyMissing",
     "APIAccessDenied",
     "APIInsufficientQuota",
-    "APIResourceNotFound"
+    "APIResourceNotFound",
+    "APICloudflareError"
 ]
 
 
+class APICloudflareError(Exception):
+    """Raised when there is an error using the API related to cloudflare"""
+    pass
+
+
 class APIKeyMissing(Exception):
     """Raised when the api key is not passed and the headers are empty"""
+    pass
 
 
 class APIFailure(Exception):
     """Raised when there is an error using the API"""
     pass
```

### Comparing `socketsecurity-0.0.64/socketsecurity/core/github.py` & `socketsecurity-0.0.65/socketsecurity/core/github.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.64/socketsecurity/core/gitlab.py` & `socketsecurity-0.0.65/socketsecurity/core/gitlab.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.64/socketsecurity/core/issues.py` & `socketsecurity-0.0.65/socketsecurity/core/issues.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.64/socketsecurity/core/licenses.py` & `socketsecurity-0.0.65/socketsecurity/core/licenses.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.64/socketsecurity/core/messages.py` & `socketsecurity-0.0.65/socketsecurity/core/messages.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.64/socketsecurity/socketcli.py` & `socketsecurity-0.0.65/socketsecurity/socketcli.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.64/socketsecurity.egg-info/PKG-INFO` & `socketsecurity-0.0.65/socketsecurity.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketsecurity
-Version: 0.0.64
+Version: 0.0.65
 Summary: Socket Security CLI for CI/CD
 Author-email: Douglas Coburn <douglas@socket.dev>
 Maintainer-email: Douglas Coburn <douglas@socket.dev>
 Project-URL: Homepage, https://socket.dev
 Keywords: socketsecurity,socket.dev,sca,oss,security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `socketsecurity-0.0.64/socketsecurity.egg-info/SOURCES.txt` & `socketsecurity-0.0.65/socketsecurity.egg-info/SOURCES.txt`

 * *Files identical despite different names*
