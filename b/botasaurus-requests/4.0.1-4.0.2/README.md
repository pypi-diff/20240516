# Comparing `tmp/botasaurus_requests-4.0.1.tar.gz` & `tmp/botasaurus_requests-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botasaurus_requests-4.0.1.tar", last modified: Thu May 16 07:05:45 2024, max compression
+gzip compressed data, was "botasaurus_requests-4.0.2.tar", last modified: Thu May 16 12:30:42 2024, max compression
```

## Comparing `botasaurus_requests-4.0.1.tar` & `botasaurus_requests-4.0.2.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 07:05:45.170810 botasaurus_requests-4.0.1/
--rw-rw-rw-   0        0        0    11558 2024-05-16 05:34:38.000000 botasaurus_requests-4.0.1/LICENSE
--rw-rw-rw-   0        0        0       14 2024-05-16 05:34:38.000000 botasaurus_requests-4.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0    14523 2024-05-16 07:05:45.169816 botasaurus_requests-4.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      597 2024-05-16 07:05:01.000000 botasaurus_requests-4.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 07:05:45.145617 botasaurus_requests-4.0.1/botasaurus_requests/
--rw-rw-rw-   0        0        0      659 2024-05-16 06:58:22.000000 botasaurus_requests-4.0.1/botasaurus_requests/__init__.py
--rw-rw-rw-   0        0        0     4939 2024-05-16 06:58:22.000000 botasaurus_requests-4.0.1/botasaurus_requests/__main__.py
--rw-rw-rw-   0        0        0       21 2024-05-16 06:58:22.000000 botasaurus_requests-4.0.1/botasaurus_requests/__version__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 07:05:45.166809 botasaurus_requests-4.0.1/botasaurus_requests/bin/
--rw-rw-rw-   0        0        0        0 2024-05-16 05:45:16.000000 botasaurus_requests-4.0.1/botasaurus_requests/bin/__init__.py
--rw-rw-rw-   0        0        0     6715 2024-05-16 06:58:22.000000 botasaurus_requests-4.0.1/botasaurus_requests/cffi.py
--rw-rw-rw-   0        0        0    15399 2024-05-16 06:48:02.000000 botasaurus_requests-4.0.1/botasaurus_requests/client.py
--rw-rw-rw-   0        0        0    16718 2024-05-16 06:48:02.000000 botasaurus_requests-4.0.1/botasaurus_requests/cookies.py
--rw-rw-rw-   0        0        0      767 2024-05-16 06:02:03.000000 botasaurus_requests-4.0.1/botasaurus_requests/exceptions.py
--rw-rw-rw-   0        0        0     6026 2024-05-16 06:58:22.000000 botasaurus_requests-4.0.1/botasaurus_requests/headers.py
--rw-rw-rw-   0        0        0    16753 2024-05-16 06:58:22.000000 botasaurus_requests-4.0.1/botasaurus_requests/parser.py
--rw-rw-rw-   0        0        0    16873 2024-05-16 06:58:22.000000 botasaurus_requests-4.0.1/botasaurus_requests/reqs.py
--rw-rw-rw-   0        0        0     8797 2024-05-16 06:58:22.000000 botasaurus_requests-4.0.1/botasaurus_requests/response.py
--rw-rw-rw-   0        0        0    12167 2024-05-16 06:58:22.000000 botasaurus_requests-4.0.1/botasaurus_requests/session.py
--rw-rw-rw-   0        0        0     4692 2024-05-16 05:45:16.000000 botasaurus_requests-4.0.1/botasaurus_requests/toolbelt.py
-drwxrwxrwx   0        0        0        0 2024-05-16 07:05:45.168309 botasaurus_requests-4.0.1/botasaurus_requests.egg-info/
--rw-rw-rw-   0        0        0    14523 2024-05-16 07:05:44.000000 botasaurus_requests-4.0.1/botasaurus_requests.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      719 2024-05-16 07:05:45.000000 botasaurus_requests-4.0.1/botasaurus_requests.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 07:05:44.000000 botasaurus_requests-4.0.1/botasaurus_requests.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-05-16 07:05:44.000000 botasaurus_requests-4.0.1/botasaurus_requests.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-16 07:05:44.000000 botasaurus_requests-4.0.1/botasaurus_requests.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1008 2024-05-16 07:05:44.000000 botasaurus_requests-4.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       81 2024-05-16 07:05:45.173829 botasaurus_requests-4.0.1/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-24 07:16:00.000000 botasaurus_requests-4.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:30:42.110888 botasaurus_requests-4.0.2/
+-rw-rw-rw-   0        0        0    11558 2024-05-16 05:34:38.000000 botasaurus_requests-4.0.2/LICENSE
+-rw-rw-rw-   0        0        0       14 2024-05-16 05:34:38.000000 botasaurus_requests-4.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    14535 2024-05-16 12:30:42.110554 botasaurus_requests-4.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      609 2024-05-16 07:09:14.000000 botasaurus_requests-4.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 12:30:42.062419 botasaurus_requests-4.0.2/botasaurus_requests/
+-rw-rw-rw-   0        0        0      700 2024-05-16 11:45:50.000000 botasaurus_requests-4.0.2/botasaurus_requests/__init__.py
+-rw-rw-rw-   0        0        0     4939 2024-05-16 06:58:22.000000 botasaurus_requests-4.0.2/botasaurus_requests/__main__.py
+-rw-rw-rw-   0        0        0       21 2024-05-16 06:58:22.000000 botasaurus_requests-4.0.2/botasaurus_requests/__version__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:30:42.106170 botasaurus_requests-4.0.2/botasaurus_requests/bin/
+-rw-rw-rw-   0        0        0        0 2024-05-16 05:45:16.000000 botasaurus_requests-4.0.2/botasaurus_requests/bin/__init__.py
+-rw-rw-rw-   0        0        0     6715 2024-05-16 06:58:22.000000 botasaurus_requests-4.0.2/botasaurus_requests/cffi.py
+-rw-rw-rw-   0        0        0    15963 2024-05-16 12:29:29.000000 botasaurus_requests-4.0.2/botasaurus_requests/client.py
+-rw-rw-rw-   0        0        0    16718 2024-05-16 06:48:02.000000 botasaurus_requests-4.0.2/botasaurus_requests/cookies.py
+-rw-rw-rw-   0        0        0      767 2024-05-16 06:02:03.000000 botasaurus_requests-4.0.2/botasaurus_requests/exceptions.py
+-rw-rw-rw-   0        0        0     6026 2024-05-16 06:58:22.000000 botasaurus_requests-4.0.2/botasaurus_requests/headers.py
+-rw-rw-rw-   0        0        0    16753 2024-05-16 06:58:22.000000 botasaurus_requests-4.0.2/botasaurus_requests/parser.py
+-rw-rw-rw-   0        0        0    19318 2024-05-16 11:31:13.000000 botasaurus_requests-4.0.2/botasaurus_requests/reqs.py
+-rw-rw-rw-   0        0        0     8486 2024-05-16 11:43:30.000000 botasaurus_requests-4.0.2/botasaurus_requests/request_class.py
+-rw-rw-rw-   0        0        0       19 2024-05-16 12:29:29.000000 botasaurus_requests-4.0.2/botasaurus_requests/request_functions.py
+-rw-rw-rw-   0        0        0     9875 2024-05-16 12:29:29.000000 botasaurus_requests-4.0.2/botasaurus_requests/response.py
+-rw-rw-rw-   0        0        0    12167 2024-05-16 06:58:22.000000 botasaurus_requests-4.0.2/botasaurus_requests/session.py
+-rw-rw-rw-   0        0        0     4692 2024-05-16 05:45:16.000000 botasaurus_requests-4.0.2/botasaurus_requests/toolbelt.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:30:42.108779 botasaurus_requests-4.0.2/botasaurus_requests.egg-info/
+-rw-rw-rw-   0        0        0    14535 2024-05-16 12:30:41.000000 botasaurus_requests-4.0.2/botasaurus_requests.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      797 2024-05-16 12:30:41.000000 botasaurus_requests-4.0.2/botasaurus_requests.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 12:30:41.000000 botasaurus_requests-4.0.2/botasaurus_requests.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-05-16 12:30:41.000000 botasaurus_requests-4.0.2/botasaurus_requests.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-16 12:30:41.000000 botasaurus_requests-4.0.2/botasaurus_requests.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1008 2024-05-16 12:30:40.000000 botasaurus_requests-4.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       81 2024-05-16 12:30:42.120408 botasaurus_requests-4.0.2/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-24 07:16:00.000000 botasaurus_requests-4.0.2/setup.py
```

### Comparing `botasaurus_requests-4.0.1/LICENSE` & `botasaurus_requests-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.1/PKG-INFO` & `botasaurus_requests-4.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botasaurus_requests
-Version: 4.0.1
+Version: 4.0.2
 Summary: botasaurus_requests is a fork of the requests library with the playwright dependencies removed.
 Author-email: Chetan <chetan@omkar.cloud>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -218,33 +218,32 @@
 Requires-Dist: urllib3
 Requires-Dist: rich
 Requires-Dist: click
 Requires-Dist: gevent
 
 # Botasaurus Requests
 
-botasaurus-requests is a fork of the requests library with the playwright dependencies removed.
+botasaurus-requests is a fork of the [hrequests](https://github.com/daijro/hrequests) library with the playwright dependencies removed.
 
 ## Installation
 
 ```bash
 pip install botasaurus-requests
 ```
 
 ## Usage
 
 ```python
 from botasaurus_requests import request
 
-driver = Driver()
 response = request.get(
     "https://www.g2.com/products/omkar-cloud/reviews",
     headers={
         "Referer": "https://www.google.com/",
     },
 )
 print(response.status_code)
 ```
 
 ## Credits
 
-Special thanks to [daijro](https://github.com/daijro) for creating [hrequests](https://github.com/daijro/hrequests).
+Kudos to [daijro](https://github.com/daijro) for creating [hrequests](https://github.com/daijro/hrequests).
```

### Comparing `botasaurus_requests-4.0.1/botasaurus_requests/__init__.py` & `botasaurus_requests-4.0.2/botasaurus_requests/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,12 +21,11 @@
 
 if detect_module():
     os.environ['BOTASAURUS_REQUESTS_MODULE'] = '1'
 
 
 from .response import Response, ProcessResponse
 from .session import Session, TLSSession, chrome, firefox
-from .reqs import *
+# from .reqs import *
+from  . import request_functions as request
 from .headers import Headers
-
-
-from .__version__ import __version__
+from .request_class import Request
```

### Comparing `botasaurus_requests-4.0.1/botasaurus_requests/__main__.py` & `botasaurus_requests-4.0.2/botasaurus_requests/__main__.py`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.1/botasaurus_requests/cffi.py` & `botasaurus_requests-4.0.2/botasaurus_requests/cffi.py`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.1/botasaurus_requests/client.py` & `botasaurus_requests-4.0.2/botasaurus_requests/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,31 @@
 
 
 def verify_proxy(proxy: str) -> None:
     # verify that the proxy is valid with regex
     if not PROXY_PATTERN.match(proxy):
         raise ProxyFormatException(f'Invalid proxy: {proxy}')
 
+def addcookies(headers, value):
+
+        if "cookie" in headers:
+            headers["Cookie"] = headers["cookie"]
+            del headers["cookie"]
+
+        cookie_header = "; ".join(
+                    [str(x) + "=" + str(y) for x, y in value.items()]
+                )
+
+        if cookie_header:
+            if headers.get("Cookie"):
+                headers["Cookie"] = (
+                            headers["Cookie"] + "; " + cookie_header
+                        )
+            else:
+                headers["Cookie"] = cookie_header
 
 @dataclass
 class TLSClient:
     client_identifier: Optional[str] = None
     random_tls_extension_order: bool = True
     force_http1: bool = False
     catch_panics: bool = False
@@ -337,22 +354,24 @@
             # Remove items, where the key or value is set to None.
             none_keys = [k for (k, v) in merged_headers.items() if v is None or k is None]
             for key in none_keys:
                 del merged_headers[key]
 
             headers = merged_headers
 
+        if isinstance(cookies, dict):
+            # addcookies(self.headers, cookies)
+            addcookies(headers, cookies)
+
         # Cookies
-        if isinstance(cookies, RequestsCookieJar):
+        elif isinstance(cookies, RequestsCookieJar):
             merge_cookies(self.cookies, cookies)
         elif isinstance(cookies, list):
             merge_cookies(self.cookies, list_to_cookiejar(cookies))
-        elif isinstance(cookies, dict):
-            self.cookies.set_cookie(cookiejar_from_dict(cookies))
-        print(headers)
+    
         # turn cookie jar into dict
 
         # Proxy
         proxy = proxy or self.proxy
         if proxy:
             verify_proxy(proxy)
```

### Comparing `botasaurus_requests-4.0.1/botasaurus_requests/cookies.py` & `botasaurus_requests-4.0.2/botasaurus_requests/cookies.py`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.1/botasaurus_requests/exceptions.py` & `botasaurus_requests-4.0.2/botasaurus_requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.1/botasaurus_requests/headers.py` & `botasaurus_requests-4.0.2/botasaurus_requests/headers.py`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.1/botasaurus_requests/parser.py` & `botasaurus_requests-4.0.2/botasaurus_requests/parser.py`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.1/botasaurus_requests/reqs.py` & `botasaurus_requests-4.0.2/botasaurus_requests/reqs.py`

 * *Files 24% similar despite different names*

```diff
@@ -272,21 +272,97 @@
 
 
 '''
 Requests shortcuts
 '''
 
 # Shortcuts for creating synchronous requests
-get: partial = partial(request, 'GET')
-options: partial = partial(request, 'OPTIONS')
-head: partial = partial(request, 'HEAD')
-post: partial = partial(request, 'POST')
-put: partial = partial(request, 'PUT')
-patch: partial = partial(request, 'PATCH')
-delete: partial = partial(request, 'DELETE')
+_get: partial = partial(request, 'GET')
+_options: partial = partial(request, 'OPTIONS')
+_head: partial = partial(request, 'HEAD')
+_post: partial = partial(request, 'POST')
+_put: partial = partial(request, 'PUT')
+_patch: partial = partial(request, 'PATCH')
+_delete: partial = partial(request, 'DELETE')
+
+
+def add_google_referer_if_given(kwargs):
+    headers = kwargs.get('headers', {})
+    referer = kwargs.pop('referer', None)
+    # Set the referrer only if it's not None and 'Referer' is not already set in headers
+    if referer is not None and ('Referer' not in headers or 'referer' not in headers):
+        headers['Referer'] = referer
+        kwargs['headers'] = headers
+
+def fix_proxies(kwargs):
+    proxies = kwargs.pop('proxies', None)
+    # Set the referrer only if it's not None and 'Referer' is not already set in headers
+    if proxies is not None:
+        if isinstance(proxies, dict):
+            proxies = proxies.get("http", proxies.get("https"))
+        if proxies and isinstance(proxies, str):
+            kwargs['proxy'] = proxies
+        else: 
+            raise Exception("Invalid proxy format. Please provide a string.")
+
+def add_redirects(kwargs, default_value):
+    return {
+        'allow_redirects': default_value,
+        **kwargs, 
+    }
+
+# proxies
+def get(url: str, *args, **kwargs) -> Response:
+    '''
+    Send a GET request with TLS client
+    '''
+
+    add_google_referer_if_given(kwargs)
+    fix_proxies(kwargs)
+    
+
+    return _get(url, *args, **add_redirects(kwargs, True))
+
+def options(url: str, *args, **kwargs) -> Response:
+    '''
+    Send an OPTIONS request with TLS client
+    '''
+    fix_proxies(kwargs)
+    return _options(url, *args, **add_redirects(kwargs, False))
+
+def head(url: str, *args, **kwargs) -> Response:
+    '''
+    Send a HEAD request with TLS client
+    '''
+    fix_proxies(kwargs)
+    return _head(url, *args, **add_redirects(kwargs, True))
+def post(url: str, *args, **kwargs) -> Response:
+    '''
+    Send a POST request with TLS client
+    '''
+    fix_proxies(kwargs)
+    return _post(url, *args, **add_redirects(kwargs, True))
+def put(url: str, *args, **kwargs) -> Response:
+    '''
+    Send a PUT request with TLS client
+    '''
+    fix_proxies(kwargs)
+    return _put(url, *args, **add_redirects(kwargs, True))
+def patch(url: str, *args, **kwargs) -> Response:
+    '''
+    Send a PATCH request with TLS client
+    '''
+    fix_proxies(kwargs)
+    return _patch(url, *args, **add_redirects(kwargs, True))
+def delete(url: str, *args, **kwargs) -> Response:
+    '''
+    Send a DELETE request with TLS client
+    '''
+    fix_proxies(kwargs)
+    return _delete(url, *args, **add_redirects(kwargs, False))
 
 '''
 Asynchronous requests shortcuts
 '''
 
 # Shortcuts for creating an unsent TLSRequest
 async_get: partial = partial(async_request, 'GET')
```

### Comparing `botasaurus_requests-4.0.1/botasaurus_requests/response.py` & `botasaurus_requests-4.0.2/botasaurus_requests/response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-import os
 import re
-import sys
 from dataclasses import dataclass
 from datetime import datetime, timedelta
 from http.client import responses as status_codes
-from typing import Callable, Iterable, List, Literal, Optional, Union
+from typing import List, Literal, Optional, Union
 
 import cchardet as chardet
 from orjson import dumps, loads
+from requests.exceptions import HTTPError
 
 import botasaurus_requests
 from botasaurus_requests.cffi import library
 from botasaurus_requests.exceptions import ClientException
 
 from .cookies import RequestsCookieJar
 from .toolbelt import CaseInsensitiveDict, FileUtils
@@ -198,14 +197,43 @@
         return resolved_links
 
     def __bool__(self) -> bool:
         '''Returns True if :attr:`status_code` is less than 400'''
         return self.ok
 
 
+    def raise_for_status(self):
+        """Raises :class:`HTTPError`, if one occurred."""
+
+        http_error_msg = ""
+        if isinstance(self.reason, bytes):
+            # We attempt to decode utf-8 first because some servers
+            # choose to localize their reason strings. If the string
+            # isn't utf-8, we fall back to iso-8859-1 for all other
+            # encodings. (See PR #3538)
+            try:
+                reason = self.reason.decode("utf-8")
+            except UnicodeDecodeError:
+                reason = self.reason.decode("iso-8859-1")
+        else:
+            reason = self.reason
+
+        if 400 <= self.status_code < 500:
+            http_error_msg = (
+                f"{self.status_code} Client Error: {reason} for url: {self.url}"
+            )
+
+        elif 500 <= self.status_code < 600:
+            http_error_msg = (
+                f"{self.status_code} Server Error: {reason} for url: {self.url}"
+            )
+
+        if http_error_msg:
+            raise HTTPError(http_error_msg, response=self)
+
     def __enter__(self):
         return self
 
     def __repr__(self):
         return f"<Response [{self.status_code}]>"
```

### Comparing `botasaurus_requests-4.0.1/botasaurus_requests/session.py` & `botasaurus_requests-4.0.2/botasaurus_requests/session.py`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.1/botasaurus_requests/toolbelt.py` & `botasaurus_requests-4.0.2/botasaurus_requests/toolbelt.py`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.1/botasaurus_requests.egg-info/PKG-INFO` & `botasaurus_requests-4.0.2/botasaurus_requests.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botasaurus_requests
-Version: 4.0.1
+Version: 4.0.2
 Summary: botasaurus_requests is a fork of the requests library with the playwright dependencies removed.
 Author-email: Chetan <chetan@omkar.cloud>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -218,33 +218,32 @@
 Requires-Dist: urllib3
 Requires-Dist: rich
 Requires-Dist: click
 Requires-Dist: gevent
 
 # Botasaurus Requests
 
-botasaurus-requests is a fork of the requests library with the playwright dependencies removed.
+botasaurus-requests is a fork of the [hrequests](https://github.com/daijro/hrequests) library with the playwright dependencies removed.
 
 ## Installation
 
 ```bash
 pip install botasaurus-requests
 ```
 
 ## Usage
 
 ```python
 from botasaurus_requests import request
 
-driver = Driver()
 response = request.get(
     "https://www.g2.com/products/omkar-cloud/reviews",
     headers={
         "Referer": "https://www.google.com/",
     },
 )
 print(response.status_code)
 ```
 
 ## Credits
 
-Special thanks to [daijro](https://github.com/daijro) for creating [hrequests](https://github.com/daijro/hrequests).
+Kudos to [daijro](https://github.com/daijro) for creating [hrequests](https://github.com/daijro/hrequests).
```

### Comparing `botasaurus_requests-4.0.1/botasaurus_requests.egg-info/SOURCES.txt` & `botasaurus_requests-4.0.2/botasaurus_requests.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 botasaurus_requests/cffi.py
 botasaurus_requests/client.py
 botasaurus_requests/cookies.py
 botasaurus_requests/exceptions.py
 botasaurus_requests/headers.py
 botasaurus_requests/parser.py
 botasaurus_requests/reqs.py
+botasaurus_requests/request_class.py
+botasaurus_requests/request_functions.py
 botasaurus_requests/response.py
 botasaurus_requests/session.py
 botasaurus_requests/toolbelt.py
 botasaurus_requests.egg-info/PKG-INFO
 botasaurus_requests.egg-info/SOURCES.txt
 botasaurus_requests.egg-info/dependency_links.txt
 botasaurus_requests.egg-info/requires.txt
```

### Comparing `botasaurus_requests-4.0.1/pyproject.toml` & `botasaurus_requests-4.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "botasaurus_requests"
-version="4.0.1"
+version="4.0.2"
 description = "botasaurus_requests is a fork of the requests library with the playwright dependencies removed."
 authors = [
   {name = "Chetan", email = "chetan@omkar.cloud" } # Optional
 ]
 license = {file = "LICENSE"}
 readme = "README.md"
 keywords = [
```

