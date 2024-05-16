# Comparing `tmp/timeseer-0.5.1.tar.gz` & `tmp/timeseer-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeseer-0.5.1.tar", last modified: Wed May 15 07:25:52 2024, max compression
+gzip compressed data, was "timeseer-0.5.2.tar", last modified: Thu May 16 08:16:56 2024, max compression
```

## Comparing `timeseer-0.5.1.tar` & `timeseer-0.5.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:25:52.600958 timeseer-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)    10595 2024-05-15 07:25:52.600958 timeseer-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10169 2024-05-15 07:25:44.000000 timeseer-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-15 07:25:44.000000 timeseer-0.5.1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:25:52.596958 timeseer-0.5.1/internal/
--rw-r--r--   0 runner    (1001) docker     (127)     8587 2024-05-15 07:25:44.000000 timeseer-0.5.1/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15688 2024-05-15 07:25:44.000000 timeseer-0.5.1/internal/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    21829 2024-05-15 07:25:44.000000 timeseer-0.5.1/internal/data_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-15 07:25:44.000000 timeseer-0.5.1/internal/data_sets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-15 07:25:44.000000 timeseer-0.5.1/internal/data_substitutions.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-15 07:25:44.000000 timeseer-0.5.1/internal/data_uploader_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-05-15 07:25:44.000000 timeseer-0.5.1/internal/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     7100 2024-05-15 07:25:44.000000 timeseer-0.5.1/internal/filters_arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6176 2024-05-15 07:25:44.000000 timeseer-0.5.1/internal/filters_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-05-15 07:25:44.000000 timeseer-0.5.1/internal/flows.py
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-15 07:25:44.000000 timeseer-0.5.1/internal/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-05-15 07:25:44.000000 timeseer-0.5.1/internal/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-15 07:25:44.000000 timeseer-0.5.1/internal/sources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:25:52.596958 timeseer-0.5.1/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 07:25:44.000000 timeseer-0.5.1/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-05-15 07:25:44.000000 timeseer-0.5.1/metadata/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-15 07:25:44.000000 timeseer-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 07:25:52.600958 timeseer-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-15 07:25:44.000000 timeseer-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:25:52.596958 timeseer-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-05-15 07:25:44.000000 timeseer-0.5.1/tests/test_filter_event_frames.py
--rw-r--r--   0 runner    (1001) docker     (127)    16990 2024-05-15 07:25:44.000000 timeseer-0.5.1/tests/test_filter_series_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)    15903 2024-05-15 07:25:44.000000 timeseer-0.5.1/tests/test_filter_series_pyarrow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:25:52.600958 timeseer-0.5.1/timeseer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10595 2024-05-15 07:25:52.000000 timeseer-0.5.1/timeseer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-15 07:25:52.000000 timeseer-0.5.1/timeseer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 07:25:52.000000 timeseer-0.5.1/timeseer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-15 07:25:52.000000 timeseer-0.5.1/timeseer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-15 07:25:52.000000 timeseer-0.5.1/timeseer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:16:56.410255 timeseer-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    10574 2024-05-16 08:16:56.406255 timeseer-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10148 2024-05-16 08:16:46.000000 timeseer-0.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-16 08:16:46.000000 timeseer-0.5.2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:16:56.406255 timeseer-0.5.2/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)     8977 2024-05-16 08:16:46.000000 timeseer-0.5.2/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17334 2024-05-16 08:16:46.000000 timeseer-0.5.2/internal/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21829 2024-05-16 08:16:46.000000 timeseer-0.5.2/internal/data_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-16 08:16:46.000000 timeseer-0.5.2/internal/data_sets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-16 08:16:46.000000 timeseer-0.5.2/internal/data_substitutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-16 08:16:46.000000 timeseer-0.5.2/internal/data_uploader_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-05-16 08:16:46.000000 timeseer-0.5.2/internal/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7100 2024-05-16 08:16:46.000000 timeseer-0.5.2/internal/filters_arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6176 2024-05-16 08:16:46.000000 timeseer-0.5.2/internal/filters_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-05-16 08:16:46.000000 timeseer-0.5.2/internal/flows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-16 08:16:46.000000 timeseer-0.5.2/internal/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-05-16 08:16:46.000000 timeseer-0.5.2/internal/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-16 08:16:46.000000 timeseer-0.5.2/internal/sources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:16:56.406255 timeseer-0.5.2/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 08:16:46.000000 timeseer-0.5.2/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-05-16 08:16:46.000000 timeseer-0.5.2/metadata/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-16 08:16:46.000000 timeseer-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 08:16:56.410255 timeseer-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-16 08:16:46.000000 timeseer-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:16:56.406255 timeseer-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-05-16 08:16:46.000000 timeseer-0.5.2/tests/test_filter_event_frames.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16990 2024-05-16 08:16:46.000000 timeseer-0.5.2/tests/test_filter_series_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15903 2024-05-16 08:16:46.000000 timeseer-0.5.2/tests/test_filter_series_pyarrow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:16:56.406255 timeseer-0.5.2/timeseer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10574 2024-05-16 08:16:56.000000 timeseer-0.5.2/timeseer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-16 08:16:56.000000 timeseer-0.5.2/timeseer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 08:16:56.000000 timeseer-0.5.2/timeseer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-16 08:16:56.000000 timeseer-0.5.2/timeseer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-16 08:16:56.000000 timeseer-0.5.2/timeseer.egg-info/top_level.txt
```

### Comparing `timeseer-0.5.1/PKG-INFO` & `timeseer-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeseer
-Version: 0.5.1
+Version: 0.5.2
 Summary: Python SDK for Timeseer.AI
 Author-email: "Timeseer.AI" <pypi@timeseer.ai>
 License: Copyright Timeseer.AI 2023
 Project-URL: Homepage, https://timeseer.ai/
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -24,15 +24,15 @@
 
 ```
 (venv) $ pip install timeseer
 ```
 
 ### Connecting
 
-The Timeseer.AI Client relies on [Apache Arrow Flight](https://arrow.apache.org/docs/format/Flight.html) for highly efficient data transfers.
+The Timeseer.AI Client uses the Timeseer REST API and uses Apache Arrow where possible to make data transfers efficient.
 
 Communications are protected by an API key.
 An API key can be generated within Timeseer under `Configure > API keys`.
 Each API key has a name and a secret value that is shown only once.
 
 The API key is used to create a connection to a Timeseer instance running at a specific host and port:
```

### Comparing `timeseer-0.5.1/README.md` & `timeseer-0.5.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 ```
 (venv) $ pip install timeseer
 ```
 
 ### Connecting
 
-The Timeseer.AI Client relies on [Apache Arrow Flight](https://arrow.apache.org/docs/format/Flight.html) for highly efficient data transfers.
+The Timeseer.AI Client uses the Timeseer REST API and uses Apache Arrow where possible to make data transfers efficient.
 
 Communications are protected by an API key.
 An API key can be generated within Timeseer under `Configure > API keys`.
 Each API key has a name and a secret value that is shown only once.
 
 The API key is used to create a connection to a Timeseer instance running at a specific host and port:
```

### Comparing `timeseer-0.5.1/__init__.py` & `timeseer-0.5.2/__init__.py`

 * *Files identical despite different names*

### Comparing `timeseer-0.5.1/internal/__init__.py` & `timeseer-0.5.2/internal/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,25 @@
 class TimeseerClientException(Exception):
     """Base class for Timeseer client exceptions.
 
     Use this to catch any exception that originates in the client.
     """
 
 
+class UnauthorizedException(TimeseerClientException):
+    """Raised when a request is not authorized to proceed with the given credentials."""
+
+
+class TransportException(TimeseerClientException):
+    """Raised when an unexpected error happened on the transport layer."""
+
+    def __init__(self, status_code: int, message: str):
+        super().__init__(f"HTTP status {status_code}: {message}")
+
+
 class AugmentationException(TimeseerClientException):
     """Exception raised when augmentation strategy fails."""
 
 
 class UnknownAugmentationStrategyException(TimeseerClientException):
     """Raised when the augmentation strategy is not known."""
 
@@ -51,15 +62,15 @@
 
 class ServerReturnedException(TimeseerClientException):
     """Raised when the server returns an error in the response body."""
 
     def __init__(self, error: str):
         TimeseerClientException.__init__(
             self,
-            f'Exception returned from the server: "{error}"',
+            f'Exception returned by server: "{error}"',
         )
 
 
 class MissingTimezoneException(TimeseerClientException):
     """Raised when a specified timeout is exceeded."""
```

### Comparing `timeseer-0.5.1/internal/client.py` & `timeseer-0.5.2/internal/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Timeseer Client provides the low-level connection to Timeseer."""
 
+import base64
 import json
 import ssl
 from dataclasses import dataclass
 from datetime import datetime, timezone
 from http.client import (
     HTTPConnection as HTTPClientConnection,
 )
@@ -20,14 +21,16 @@
 
 import pyarrow as pa
 from kukur import Metadata, SeriesSearch, SeriesSelector
 from kukur.base import SourceStructure
 
 from timeseer_client.internal import (
     ServerReturnedException,
+    TransportException,
+    UnauthorizedException,
     parse_json_exception_message,
     parse_json_response,
 )
 from timeseer_client.internal.flows import (
     evaluate_flow,
     wait_for_flow_evaluation,
 )
@@ -57,33 +60,33 @@
     __use_https: bool = False
 
     def __init__(
         self,
         api_key: Tuple[str, str] = ("", ""),
         host: str = "localhost",
         port: int = 443,
-        use_tls: Union[bool, TLSOptions] = False,
+        use_tls: Optional[Union[bool, TLSOptions]] = None,
     ):
         """Create a new Client.
 
         Creating a client does not open a connection.
 
         Args:
             api_key: the api key to use when connecting. This is a tuple of (key name, key).
             host: the hostname where the Timeseer instance is running. Defaults to ``localhost``.
-            port: the port where the Timeseer instance is running. Defaults to ``8081``.
+            port: the port where the Timeseer instance is running. Defaults to ``443``.
             use_tls: set to True to use a TLS-secured connection, or pass TLSOptions for more configuration.
         """
         self._host = host
         self._port = port
         self._api_key = api_key
         self._api_prefix = "/public/api/v1/"
 
         self._tls_options = None
-        if use_tls is True:
+        if (use_tls is None and port == 443) or use_tls is True:
             self._tls_options = TLSOptions()
         elif use_tls:
             self._tls_options = use_tls
 
         self.__use_https = self._tls_options is not None
 
         if self._tls_options is not None:
@@ -92,14 +95,44 @@
                 self.__context.check_hostname = False
                 self.__context.verify_mode = ssl.CERT_NONE
             if self._tls_options.root_certs:
                 self.__context.load_verify_locations(
                     cadata=self._tls_options.root_certs
                 )
 
+    @classmethod
+    def for_tls(
+        cls,
+        host: str,
+        *,
+        port: int = 443,
+        api_key: Tuple[str, str] = ("", ""),
+        tls_options: Optional[TLSOptions] = None,
+    ) -> "Client":
+        """Create a new Client that uses TLS to secure the connection.
+
+        The CA certificates of the operating system will be used.
+        Additional certificates can be provided using `tls_options`.
+
+        Args:
+            host: the hostname where Timeseer instance is running.
+            port: the port where the Timeseer instance is running. Defaults to ``443``.
+            api_key: the api key to use when connecting. This is a tuple of (key name, key).
+            tls_options: TLS configuration options.
+        """
+        use_tls: Union[bool, TLSOptions] = True
+        if tls_options is not None:
+            use_tls = tls_options
+        return cls(
+            api_key=api_key,
+            host=host,
+            port=port,
+            use_tls=use_tls,
+        )
+
     def wait_for_available(self, *, timeout: float = 30.0):
         """Wait for the client to be available.
 
         This will block until the client is available or the timeout is reached.
 
         Args:
             timeout: the number of seconds to wait for the client to become available.
@@ -373,14 +406,22 @@
         formatted_url = self._api_prefix + url
         if query is not None and len(query) > 0:
             query_params = [
                 f"{url_quote(key)}={url_quote(value)}" for key, value in query.items()
             ]
             formatted_url = f"{formatted_url}?{'&'.join(query_params)}"
 
+        if self._api_key != ("", ""):
+            if headers is None:
+                headers = {}
+            auth = base64.b64encode(
+                f"{self._api_key[0]}:{self._api_key[1]}".encode("utf-8")
+            )
+            headers["Authorization"] = f"Basic {auth.decode()}"
+
         return _request(connection, method, formatted_url, headers, body)
 
     def _get_connection(self) -> HTTPConnection:
         if self.__use_https:
             return HTTPSClientConnection(self._host, self._port, context=self.__context)
         return HTTPClientConnection(self._host, self._port)
 
@@ -423,16 +464,20 @@
         kwargs["headers"] = headers
     if body is not None:
         kwargs["body"] = body
     connection.request(method, url, **kwargs)
     response = connection.getresponse()
     location_header = response.getheader("location")
     if location_header is None:
+        if response.status == 401:
+            raise UnauthorizedException()
         if response.status not in [200, 201, 204]:
-            raise ServerReturnedException(parse_json_exception_message(response))
+            if "application/json" in response.getheader("Content-Type", ""):
+                raise ServerReturnedException(parse_json_exception_message(response))
+            raise TransportException(response.status, response.read().decode("utf-8"))
         return response
 
     response.read()
     location = urljoin(url, location_header)
     return _request(connection, method, location, headers, body)
```

### Comparing `timeseer-0.5.1/internal/data_services.py` & `timeseer-0.5.2/internal/data_services.py`

 * *Files identical despite different names*

### Comparing `timeseer-0.5.1/internal/data_sets.py` & `timeseer-0.5.2/internal/data_sets.py`

 * *Files identical despite different names*

### Comparing `timeseer-0.5.1/internal/data_substitutions.py` & `timeseer-0.5.2/internal/data_substitutions.py`

 * *Files identical despite different names*

### Comparing `timeseer-0.5.1/internal/data_uploader_pandas.py` & `timeseer-0.5.2/internal/data_uploader_pandas.py`

 * *Files identical despite different names*

### Comparing `timeseer-0.5.1/internal/filters.py` & `timeseer-0.5.2/internal/filters.py`

 * *Files identical despite different names*

### Comparing `timeseer-0.5.1/internal/filters_arrow.py` & `timeseer-0.5.2/internal/filters_arrow.py`

 * *Files identical despite different names*

### Comparing `timeseer-0.5.1/internal/filters_pandas.py` & `timeseer-0.5.2/internal/filters_pandas.py`

 * *Files identical despite different names*

### Comparing `timeseer-0.5.1/internal/flows.py` & `timeseer-0.5.2/internal/flows.py`

 * *Files identical despite different names*

### Comparing `timeseer-0.5.1/internal/profile.py` & `timeseer-0.5.2/internal/profile.py`

 * *Files identical despite different names*

### Comparing `timeseer-0.5.1/internal/resources.py` & `timeseer-0.5.2/internal/resources.py`

 * *Files identical despite different names*

### Comparing `timeseer-0.5.1/internal/sources.py` & `timeseer-0.5.2/internal/sources.py`

 * *Files identical despite different names*

### Comparing `timeseer-0.5.1/metadata/fields.py` & `timeseer-0.5.2/metadata/fields.py`

 * *Files identical despite different names*

### Comparing `timeseer-0.5.1/pyproject.toml` & `timeseer-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `timeseer-0.5.1/tests/test_filter_event_frames.py` & `timeseer-0.5.2/tests/test_filter_event_frames.py`

 * *Files identical despite different names*

### Comparing `timeseer-0.5.1/tests/test_filter_series_pandas.py` & `timeseer-0.5.2/tests/test_filter_series_pandas.py`

 * *Files identical despite different names*

### Comparing `timeseer-0.5.1/tests/test_filter_series_pyarrow.py` & `timeseer-0.5.2/tests/test_filter_series_pyarrow.py`

 * *Files identical despite different names*

### Comparing `timeseer-0.5.1/timeseer.egg-info/PKG-INFO` & `timeseer-0.5.2/timeseer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeseer
-Version: 0.5.1
+Version: 0.5.2
 Summary: Python SDK for Timeseer.AI
 Author-email: "Timeseer.AI" <pypi@timeseer.ai>
 License: Copyright Timeseer.AI 2023
 Project-URL: Homepage, https://timeseer.ai/
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -24,15 +24,15 @@
 
 ```
 (venv) $ pip install timeseer
 ```
 
 ### Connecting
 
-The Timeseer.AI Client relies on [Apache Arrow Flight](https://arrow.apache.org/docs/format/Flight.html) for highly efficient data transfers.
+The Timeseer.AI Client uses the Timeseer REST API and uses Apache Arrow where possible to make data transfers efficient.
 
 Communications are protected by an API key.
 An API key can be generated within Timeseer under `Configure > API keys`.
 Each API key has a name and a secret value that is shown only once.
 
 The API key is used to create a connection to a Timeseer instance running at a specific host and port:
```

### Comparing `timeseer-0.5.1/timeseer.egg-info/SOURCES.txt` & `timeseer-0.5.2/timeseer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

