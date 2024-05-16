# Comparing `tmp/cortex_xdr_client-1.8.8.tar.gz` & `tmp/cortex_xdr_client-1.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cortex_xdr_client-1.8.8.tar", max compression
+gzip compressed data, was "cortex_xdr_client-1.8.9.tar", max compression
```

## Comparing `cortex_xdr_client-1.8.8.tar` & `cortex_xdr_client-1.8.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1072 2024-04-03 10:21:50.021368 cortex_xdr_client-1.8.8/LICENSE
--rw-r--r--   0        0        0     3175 2024-04-03 10:21:50.021368 cortex_xdr_client-1.8.8/README.rst
--rw-r--r--   0        0        0       61 2024-04-03 10:21:50.021368 cortex_xdr_client-1.8.8/cortex_xdr_client/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 10:21:50.021368 cortex_xdr_client-1.8.8/cortex_xdr_client/api/__init__.py
--rw-r--r--   0        0        0     2059 2024-04-03 10:21:50.021368 cortex_xdr_client-1.8.8/cortex_xdr_client/api/actions_api.py
--rw-r--r--   0        0        0     3387 2024-04-03 10:21:50.021368 cortex_xdr_client-1.8.8/cortex_xdr_client/api/alerts_api.py
--rw-r--r--   0        0        0     1544 2024-04-03 10:21:50.021368 cortex_xdr_client-1.8.8/cortex_xdr_client/api/authentication.py
--rw-r--r--   0        0        0     2376 2024-04-03 10:21:50.021368 cortex_xdr_client-1.8.8/cortex_xdr_client/api/base_api.py
--rw-r--r--   0        0        0      890 2024-04-03 10:21:50.021368 cortex_xdr_client-1.8.8/cortex_xdr_client/api/download_api.py
--rw-r--r--   0        0        0    18253 2024-04-03 10:21:50.021368 cortex_xdr_client-1.8.8/cortex_xdr_client/api/endpoints_api.py
--rw-r--r--   0        0        0     5261 2024-04-03 10:21:50.021368 cortex_xdr_client-1.8.8/cortex_xdr_client/api/incidents_api.py
--rw-r--r--   0        0        0     1175 2024-04-03 10:21:50.021368 cortex_xdr_client-1.8.8/cortex_xdr_client/api/ioc_api.py
--rw-r--r--   0        0        0        0 2024-04-03 10:21:50.021368 cortex_xdr_client-1.8.8/cortex_xdr_client/api/models/__init__.py
--rw-r--r--   0        0        0      390 2024-04-03 10:21:50.021368 cortex_xdr_client-1.8.8/cortex_xdr_client/api/models/action_status.py
--rw-r--r--   0        0        0     5902 2024-04-03 10:21:50.021368 cortex_xdr_client-1.8.8/cortex_xdr_client/api/models/alerts.py
--rw-r--r--   0        0        0     2775 2024-04-03 10:21:50.021368 cortex_xdr_client-1.8.8/cortex_xdr_client/api/models/endpoints.py
--rw-r--r--   0        0        0      692 2024-04-03 10:21:50.021368 cortex_xdr_client-1.8.8/cortex_xdr_client/api/models/exceptions.py
--rw-r--r--   0        0        0     2835 2024-04-03 10:21:50.021368 cortex_xdr_client-1.8.8/cortex_xdr_client/api/models/filters.py
--rw-r--r--   0        0        0     7770 2024-04-03 10:21:50.021368 cortex_xdr_client-1.8.8/cortex_xdr_client/api/models/incidents.py
--rw-r--r--   0        0        0     2617 2024-04-03 10:21:50.021368 cortex_xdr_client-1.8.8/cortex_xdr_client/api/models/ioc.py
--rw-r--r--   0        0        0     2392 2024-04-03 10:21:50.021368 cortex_xdr_client-1.8.8/cortex_xdr_client/api/models/scripts.py
--rw-r--r--   0        0        0    12326 2024-04-03 10:21:50.021368 cortex_xdr_client-1.8.8/cortex_xdr_client/api/scripts_api.py
--rw-r--r--   0        0        0     5414 2024-04-03 10:21:50.021368 cortex_xdr_client-1.8.8/cortex_xdr_client/api/xql_api.py
--rw-r--r--   0        0        0     2497 2024-04-03 10:21:50.021368 cortex_xdr_client-1.8.8/cortex_xdr_client/client.py
--rw-r--r--   0        0        0      646 2024-04-03 10:22:05.361466 cortex_xdr_client-1.8.8/pyproject.toml
--rw-r--r--   0        0        0     3933 1970-01-01 00:00:00.000000 cortex_xdr_client-1.8.8/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-16 09:45:50.444774 cortex_xdr_client-1.8.9/LICENSE
+-rw-r--r--   0        0        0     3175 2024-05-16 09:45:50.444774 cortex_xdr_client-1.8.9/README.rst
+-rw-r--r--   0        0        0       61 2024-05-16 09:45:50.444774 cortex_xdr_client-1.8.9/cortex_xdr_client/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-16 09:45:50.448774 cortex_xdr_client-1.8.9/cortex_xdr_client/api/__init__.py
+-rw-r--r--   0        0        0     2059 2024-05-16 09:45:50.448774 cortex_xdr_client-1.8.9/cortex_xdr_client/api/actions_api.py
+-rw-r--r--   0        0        0     3387 2024-05-16 09:45:50.448774 cortex_xdr_client-1.8.9/cortex_xdr_client/api/alerts_api.py
+-rw-r--r--   0        0        0     1544 2024-05-16 09:45:50.448774 cortex_xdr_client-1.8.9/cortex_xdr_client/api/authentication.py
+-rw-r--r--   0        0        0     2360 2024-05-16 09:45:50.448774 cortex_xdr_client-1.8.9/cortex_xdr_client/api/base_api.py
+-rw-r--r--   0        0        0      890 2024-05-16 09:45:50.448774 cortex_xdr_client-1.8.9/cortex_xdr_client/api/download_api.py
+-rw-r--r--   0        0        0    18253 2024-05-16 09:45:50.448774 cortex_xdr_client-1.8.9/cortex_xdr_client/api/endpoints_api.py
+-rw-r--r--   0        0        0     5261 2024-05-16 09:45:50.448774 cortex_xdr_client-1.8.9/cortex_xdr_client/api/incidents_api.py
+-rw-r--r--   0        0        0     1175 2024-05-16 09:45:50.448774 cortex_xdr_client-1.8.9/cortex_xdr_client/api/ioc_api.py
+-rw-r--r--   0        0        0        0 2024-05-16 09:45:50.448774 cortex_xdr_client-1.8.9/cortex_xdr_client/api/models/__init__.py
+-rw-r--r--   0        0        0      390 2024-05-16 09:45:50.448774 cortex_xdr_client-1.8.9/cortex_xdr_client/api/models/action_status.py
+-rw-r--r--   0        0        0     5902 2024-05-16 09:45:50.448774 cortex_xdr_client-1.8.9/cortex_xdr_client/api/models/alerts.py
+-rw-r--r--   0        0        0     2775 2024-05-16 09:45:50.448774 cortex_xdr_client-1.8.9/cortex_xdr_client/api/models/endpoints.py
+-rw-r--r--   0        0        0      692 2024-05-16 09:45:50.448774 cortex_xdr_client-1.8.9/cortex_xdr_client/api/models/exceptions.py
+-rw-r--r--   0        0        0     2835 2024-05-16 09:45:50.448774 cortex_xdr_client-1.8.9/cortex_xdr_client/api/models/filters.py
+-rw-r--r--   0        0        0     7770 2024-05-16 09:45:50.448774 cortex_xdr_client-1.8.9/cortex_xdr_client/api/models/incidents.py
+-rw-r--r--   0        0        0     2617 2024-05-16 09:45:50.448774 cortex_xdr_client-1.8.9/cortex_xdr_client/api/models/ioc.py
+-rw-r--r--   0        0        0     2392 2024-05-16 09:45:50.448774 cortex_xdr_client-1.8.9/cortex_xdr_client/api/models/scripts.py
+-rw-r--r--   0        0        0    12326 2024-05-16 09:45:50.448774 cortex_xdr_client-1.8.9/cortex_xdr_client/api/scripts_api.py
+-rw-r--r--   0        0        0     5414 2024-05-16 09:45:50.448774 cortex_xdr_client-1.8.9/cortex_xdr_client/api/xql_api.py
+-rw-r--r--   0        0        0     2497 2024-05-16 09:45:50.448774 cortex_xdr_client-1.8.9/cortex_xdr_client/client.py
+-rw-r--r--   0        0        0      646 2024-05-16 09:46:07.292713 cortex_xdr_client-1.8.9/pyproject.toml
+-rw-r--r--   0        0        0     3933 1970-01-01 00:00:00.000000 cortex_xdr_client-1.8.9/PKG-INFO
```

### Comparing `cortex_xdr_client-1.8.8/LICENSE` & `cortex_xdr_client-1.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.8/README.rst` & `cortex_xdr_client-1.8.9/README.rst`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.8/cortex_xdr_client/api/actions_api.py` & `cortex_xdr_client-1.8.9/cortex_xdr_client/api/actions_api.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.8/cortex_xdr_client/api/alerts_api.py` & `cortex_xdr_client-1.8.9/cortex_xdr_client/api/alerts_api.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.8/cortex_xdr_client/api/authentication.py` & `cortex_xdr_client-1.8.9/cortex_xdr_client/api/authentication.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.8/cortex_xdr_client/api/base_api.py` & `cortex_xdr_client-1.8.9/cortex_xdr_client/api/base_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,15 @@
               method: str = "post",
               params: dict = None,
               json_value: object = None,
               header_params=None) -> requests.Response:
         if header_params is None:
             header_params = {}
         url = self._get_url(call_name)
-        headers = self._auth.get_headers()
-        self.extend(headers, header_params)
+        headers = self.extend(self._auth.get_headers(), header_params)
 
         return self._execute_call(url=url,
                                   method=method,
                                   params=params,
                                   headers=headers,
                                   json_value=json_value)
```

### Comparing `cortex_xdr_client-1.8.8/cortex_xdr_client/api/download_api.py` & `cortex_xdr_client-1.8.9/cortex_xdr_client/api/download_api.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.8/cortex_xdr_client/api/endpoints_api.py` & `cortex_xdr_client-1.8.9/cortex_xdr_client/api/endpoints_api.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.8/cortex_xdr_client/api/incidents_api.py` & `cortex_xdr_client-1.8.9/cortex_xdr_client/api/incidents_api.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.8/cortex_xdr_client/api/ioc_api.py` & `cortex_xdr_client-1.8.9/cortex_xdr_client/api/ioc_api.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.8/cortex_xdr_client/api/models/alerts.py` & `cortex_xdr_client-1.8.9/cortex_xdr_client/api/models/alerts.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.8/cortex_xdr_client/api/models/endpoints.py` & `cortex_xdr_client-1.8.9/cortex_xdr_client/api/models/endpoints.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.8/cortex_xdr_client/api/models/exceptions.py` & `cortex_xdr_client-1.8.9/cortex_xdr_client/api/models/exceptions.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.8/cortex_xdr_client/api/models/filters.py` & `cortex_xdr_client-1.8.9/cortex_xdr_client/api/models/filters.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.8/cortex_xdr_client/api/models/incidents.py` & `cortex_xdr_client-1.8.9/cortex_xdr_client/api/models/incidents.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.8/cortex_xdr_client/api/models/ioc.py` & `cortex_xdr_client-1.8.9/cortex_xdr_client/api/models/ioc.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.8/cortex_xdr_client/api/models/scripts.py` & `cortex_xdr_client-1.8.9/cortex_xdr_client/api/models/scripts.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.8/cortex_xdr_client/api/scripts_api.py` & `cortex_xdr_client-1.8.9/cortex_xdr_client/api/scripts_api.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.8/cortex_xdr_client/api/xql_api.py` & `cortex_xdr_client-1.8.9/cortex_xdr_client/api/xql_api.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.8/cortex_xdr_client/client.py` & `cortex_xdr_client-1.8.9/cortex_xdr_client/client.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.8/pyproject.toml` & `cortex_xdr_client-1.8.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "cortex-xdr-client"
 packages= [
     { include = "cortex_xdr_client", from="." },
 ]
-version = "v1.8.8"
+version = "v1.8.9"
 description = "API client for Cortex XDR Prevent"
 authors = ["ebarti"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/ebarti/cortex-xdr-client"
 repository = "https://github.com/ebarti/cortex-xdr-client"
```

### Comparing `cortex_xdr_client-1.8.8/PKG-INFO` & `cortex_xdr_client-1.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cortex-xdr-client
-Version: 1.8.8
+Version: 1.8.9
 Summary: API client for Cortex XDR Prevent
 Home-page: https://github.com/ebarti/cortex-xdr-client
 License: MIT
 Author: ebarti
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

