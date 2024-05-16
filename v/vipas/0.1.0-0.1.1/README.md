# Comparing `tmp/vipas-0.1.0.tar.gz` & `tmp/vipas-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vipas-0.1.0.tar", last modified: Wed May 15 18:10:36 2024, max compression
+gzip compressed data, was "vipas-0.1.1.tar", last modified: Thu May 16 12:26:38 2024, max compression
```

## Comparing `vipas-0.1.0.tar` & `vipas-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-15 18:10:36.020362 vipas-0.1.0/
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     2487 2024-04-30 05:46:43.000000 vipas-0.1.0/LICENSE.md
--rw-r--r--   0 aditya    (1001) aditya    (1001)      360 2024-05-15 18:10:36.020362 vipas-0.1.0/PKG-INFO
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     1598 2024-05-01 12:56:58.000000 vipas-0.1.0/README.md
--rw-rw-r--   0 aditya    (1001) aditya    (1001)       91 2024-05-14 08:16:21.000000 vipas-0.1.0/pyproject.toml
--rw-rw-r--   0 aditya    (1001) aditya    (1001)      443 2024-05-15 18:10:36.020362 vipas-0.1.0/setup.cfg
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     1273 2024-05-15 16:38:12.000000 vipas-0.1.0/setup.py
-drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-15 18:10:36.016362 vipas-0.1.0/test/
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     2818 2024-05-14 08:16:21.000000 vipas-0.1.0/test/test_model_client.py
-drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-15 18:10:36.020362 vipas-0.1.0/vipas/
--rw-rw-r--   0 aditya    (1001) aditya    (1001)      725 2024-04-30 15:42:34.000000 vipas-0.1.0/vipas/__init__.py
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     2084 2024-05-02 09:27:49.000000 vipas-0.1.0/vipas/_rest.py
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     4145 2024-05-15 18:08:55.000000 vipas-0.1.0/vipas/config.py
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     3555 2024-05-01 08:36:27.000000 vipas-0.1.0/vipas/exceptions.py
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     6279 2024-05-14 08:16:21.000000 vipas-0.1.0/vipas/model.py
-drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-15 18:10:36.020362 vipas-0.1.0/vipas.egg-info/
--rw-r--r--   0 aditya    (1001) aditya    (1001)      360 2024-05-15 18:10:36.000000 vipas-0.1.0/vipas.egg-info/PKG-INFO
--rw-rw-r--   0 aditya    (1001) aditya    (1001)      308 2024-05-15 18:10:36.000000 vipas-0.1.0/vipas.egg-info/SOURCES.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)        1 2024-05-15 18:10:36.000000 vipas-0.1.0/vipas.egg-info/dependency_links.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)       65 2024-05-15 18:10:36.000000 vipas-0.1.0/vipas.egg-info/requires.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)        6 2024-05-15 18:10:36.000000 vipas-0.1.0/vipas.egg-info/top_level.txt
+drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-16 12:26:38.408251 vipas-0.1.1/
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     2487 2024-04-30 05:46:43.000000 vipas-0.1.1/LICENSE.md
+-rw-r--r--   0 aditya    (1001) aditya    (1001)      360 2024-05-16 12:26:38.408251 vipas-0.1.1/PKG-INFO
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     1598 2024-05-01 12:56:58.000000 vipas-0.1.1/README.md
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)       91 2024-05-14 08:16:21.000000 vipas-0.1.1/pyproject.toml
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)      443 2024-05-16 12:26:38.412251 vipas-0.1.1/setup.cfg
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     1273 2024-05-16 10:24:06.000000 vipas-0.1.1/setup.py
+drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-16 12:26:38.400251 vipas-0.1.1/test/
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     2818 2024-05-14 08:16:21.000000 vipas-0.1.1/test/test_model_client.py
+drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-16 12:26:38.404251 vipas-0.1.1/vipas/
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)      725 2024-04-30 15:42:34.000000 vipas-0.1.1/vipas/__init__.py
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     2084 2024-05-02 09:27:49.000000 vipas-0.1.1/vipas/_rest.py
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     4145 2024-05-15 18:08:55.000000 vipas-0.1.1/vipas/config.py
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     3555 2024-05-01 08:36:27.000000 vipas-0.1.1/vipas/exceptions.py
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     6864 2024-05-16 12:24:58.000000 vipas-0.1.1/vipas/model.py
+drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-16 12:26:38.408251 vipas-0.1.1/vipas.egg-info/
+-rw-r--r--   0 aditya    (1001) aditya    (1001)      360 2024-05-16 12:26:38.000000 vipas-0.1.1/vipas.egg-info/PKG-INFO
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)      308 2024-05-16 12:26:38.000000 vipas-0.1.1/vipas.egg-info/SOURCES.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)        1 2024-05-16 12:26:38.000000 vipas-0.1.1/vipas.egg-info/dependency_links.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)       65 2024-05-16 12:26:38.000000 vipas-0.1.1/vipas.egg-info/requires.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)        6 2024-05-16 12:26:38.000000 vipas-0.1.1/vipas.egg-info/top_level.txt
```

### Comparing `vipas-0.1.0/LICENSE.md` & `vipas-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `vipas-0.1.0/README.md` & `vipas-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `vipas-0.1.0/setup.py` & `vipas-0.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "vipas"
-VERSION = "0.1.0"
+VERSION = "0.1.1"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3",
     "pydantic",
     "typing-extensions",
     "ratelimit",
     "pybreaker",
```

### Comparing `vipas-0.1.0/test/test_model_client.py` & `vipas-0.1.1/test/test_model_client.py`

 * *Files identical despite different names*

### Comparing `vipas-0.1.0/vipas/__init__.py` & `vipas-0.1.1/vipas/__init__.py`

 * *Files identical despite different names*

### Comparing `vipas-0.1.0/vipas/_rest.py` & `vipas-0.1.1/vipas/_rest.py`

 * *Files identical despite different names*

### Comparing `vipas-0.1.0/vipas/config.py` & `vipas-0.1.1/vipas/config.py`

 * *Files identical despite different names*

### Comparing `vipas-0.1.0/vipas/exceptions.py` & `vipas-0.1.1/vipas/exceptions.py`

 * *Files identical despite different names*

### Comparing `vipas-0.1.0/vipas/model.py` & `vipas-0.1.1/vipas/model.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,28 +12,28 @@
   other intellectual property laws. You may not modify, reproduce, perform,
   display, create derivative works from, repurpose, or distribute this code or any portion of it
   without the express prior written permission of Vipas.AI.
   
   For more information, contact Vipas.AI at legal@vipas.ai
 
 """  # noqa: E501
+import os
 import pybreaker
 from typing import Tuple, Optional, List, Dict, Any
 from pydantic import Field, StrictStr
 from typing_extensions import Annotated
 from ratelimit import limits, sleep_and_retry
 
 from vipas.config import Config
 from vipas import _rest
 from vipas.exceptions import (
     ClientException
 )
 
 RequestSerialized = Tuple[str, str, Dict[str, str], Optional[any]]
-breaker = pybreaker.CircuitBreaker(fail_max=5, reset_timeout=60) # timeout is in seconds
 
 class ModelClient:
     """
         Model client for Vipas API proxy service.
         :param config: .Configuration object for this client
     """
     def __init__(
@@ -42,18 +42,30 @@
     ) -> None:
         # use default configuration if none is provided
         if configuration is None:
             configuration = Config.get_default()
         self.configuration = configuration
 
         self.rest_client = _rest.RESTClientObject(configuration)
+        self._configure_decorators()
+
+    def _configure_decorators(self):
+        vps_env_type = os.getenv('VPS_ENV_TYPE')
+        if vps_env_type == 'vipas-streamlit':
+            self.rate_limit = lambda func: func  # No-op decorator
+            self.breaker = pybreaker.CircuitBreaker(fail_max=20, reset_timeout=60)  # 20 failures per minute
+        else:
+            self.breaker = pybreaker.CircuitBreaker(fail_max=10, reset_timeout=60)  # 10 failures per minute
+            self.rate_limit = limits(calls=20, period=60)  # 20 calls per minute
+        
+        # Apply decorators dynamically
+        self.predict = self.breaker(self.predict)
+        self.predict = self.rate_limit(self.predict)
+        self.predict = sleep_and_retry(self.predict)
 
-    @breaker
-    @sleep_and_retry
-    @limits(calls=10, period=60)# period is in seconds 
     def predict(
         self,
         model_id: Annotated[StrictStr, Field(description="Unique identifier for the model from which the prediction is requested")],
         input_data: Annotated[Any, Field(description="Input for the prediction")],
     ) -> dict:
         """
             Get Model Prediction
```

