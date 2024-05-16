# Comparing `tmp/openai_priority_loadbalancer-1.0.1.tar.gz` & `tmp/openai_priority_loadbalancer-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_priority_loadbalancer-1.0.1.tar", last modified: Wed May 15 10:41:08 2024, max compression
+gzip compressed data, was "openai_priority_loadbalancer-1.0.2.tar", last modified: Wed May 15 16:31:32 2024, max compression
```

## Comparing `openai_priority_loadbalancer-1.0.1.tar` & `openai_priority_loadbalancer-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 10:41:08.557744 openai_priority_loadbalancer-1.0.1/
--rw-rw-rw-   0        0        0     1068 2024-05-11 18:48:22.000000 openai_priority_loadbalancer-1.0.1/LICENSE
--rw-rw-rw-   0        0        0    12101 2024-05-15 10:38:20.000000 openai_priority_loadbalancer-1.0.1/PACKAGE_README.md
--rw-rw-rw-   0        0        0    12740 2024-05-15 10:41:08.552352 openai_priority_loadbalancer-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    12216 2024-05-15 09:57:38.000000 openai_priority_loadbalancer-1.0.1/README.md
--rw-rw-rw-   0        0        0      711 2024-05-15 10:39:10.000000 openai_priority_loadbalancer-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-15 10:41:08.557744 openai_priority_loadbalancer-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-15 10:41:08.449846 openai_priority_loadbalancer-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-15 10:41:08.494955 openai_priority_loadbalancer-1.0.1/src/openai_priority_loadbalancer/
--rw-rw-rw-   0        0        0       45 2024-05-14 20:10:13.000000 openai_priority_loadbalancer-1.0.1/src/openai_priority_loadbalancer/__init__.py
--rw-rw-rw-   0        0        0     9649 2024-05-15 10:38:20.000000 openai_priority_loadbalancer-1.0.1/src/openai_priority_loadbalancer/openai_priority_loadbalancer.py
-drwxrwxrwx   0        0        0        0 2024-05-15 10:41:08.548589 openai_priority_loadbalancer-1.0.1/src/openai_priority_loadbalancer.egg-info/
--rw-rw-rw-   0        0        0    12740 2024-05-15 10:41:08.000000 openai_priority_loadbalancer-1.0.1/src/openai_priority_loadbalancer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      439 2024-05-15 10:41:08.000000 openai_priority_loadbalancer-1.0.1/src/openai_priority_loadbalancer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 10:41:08.000000 openai_priority_loadbalancer-1.0.1/src/openai_priority_loadbalancer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-15 10:41:08.000000 openai_priority_loadbalancer-1.0.1/src/openai_priority_loadbalancer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2024-05-15 10:41:08.000000 openai_priority_loadbalancer-1.0.1/src/openai_priority_loadbalancer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 16:31:32.846495 openai_priority_loadbalancer-1.0.2/
+-rw-rw-rw-   0        0        0     1068 2024-05-11 18:48:22.000000 openai_priority_loadbalancer-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0    12172 2024-05-15 16:29:57.000000 openai_priority_loadbalancer-1.0.2/PACKAGE_README.md
+-rw-rw-rw-   0        0        0    12811 2024-05-15 16:31:32.826688 openai_priority_loadbalancer-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    12216 2024-05-15 09:57:38.000000 openai_priority_loadbalancer-1.0.2/README.md
+-rw-rw-rw-   0        0        0      711 2024-05-15 16:30:50.000000 openai_priority_loadbalancer-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-15 16:31:32.847207 openai_priority_loadbalancer-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-15 16:31:32.624682 openai_priority_loadbalancer-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-15 16:31:32.696539 openai_priority_loadbalancer-1.0.2/src/openai_priority_loadbalancer/
+-rw-rw-rw-   0        0        0       45 2024-05-14 20:10:13.000000 openai_priority_loadbalancer-1.0.2/src/openai_priority_loadbalancer/__init__.py
+-rw-rw-rw-   0        0        0    10355 2024-05-15 16:29:57.000000 openai_priority_loadbalancer-1.0.2/src/openai_priority_loadbalancer/openai_priority_loadbalancer.py
+drwxrwxrwx   0        0        0        0 2024-05-15 16:31:32.820889 openai_priority_loadbalancer-1.0.2/src/openai_priority_loadbalancer.egg-info/
+-rw-rw-rw-   0        0        0    12811 2024-05-15 16:31:32.000000 openai_priority_loadbalancer-1.0.2/src/openai_priority_loadbalancer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2024-05-15 16:31:32.000000 openai_priority_loadbalancer-1.0.2/src/openai_priority_loadbalancer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 16:31:32.000000 openai_priority_loadbalancer-1.0.2/src/openai_priority_loadbalancer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-15 16:31:32.000000 openai_priority_loadbalancer-1.0.2/src/openai_priority_loadbalancer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2024-05-15 16:31:32.000000 openai_priority_loadbalancer-1.0.2/src/openai_priority_loadbalancer.egg-info/top_level.txt
```

### Comparing `openai_priority_loadbalancer-1.0.1/LICENSE` & `openai_priority_loadbalancer-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_priority_loadbalancer-1.0.1/PACKAGE_README.md` & `openai_priority_loadbalancer-1.0.2/PACKAGE_README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 - Prioritize exhaustion of all tokens in a PTU instance with a fallback onto multiple consumption instances.
 - Tiered prioritization of multiple consumption instances (e.g. use instances first that are geographically closer).
 
 While the [OpenAI Python API library](https://github.com/openai/openai-python) respects HTTP 429 and automatically retries after the requested wait period, the library is not set up to support the aforementioned customer desires. The library does, however, allow for the injection of custom httpx clients. This gave rise to this project.
 
 And while there are other Python OpenAI load balancers freely available, I have not seen one yet that addresses the aforementioned scenarios.
 
-Python OpenAI LoadBalancer is injected cleanly into the OpenAI Python API library. The changes between a conventional and a load-balanced Azure OpenAI implementation are few and almost entirely configuration of the backends to be used. You can see a side-by-side example in the [aoai.py](./aoai.py) file in this repo.
+Python OpenAI Load Balancer is injected cleanly into the OpenAI Python API library. The changes between a conventional and a load-balanced Azure OpenAI implementation are few and almost entirely configuration of the backends to be used. You can see a side-by-side example in the [aoai.py](https://github.com/simonkurtz-MSFT/python-openai-loadbalancer/blob/main/aoai.py) file in this repo.
 
 **Please refer to the GitHub repo for detailed test harnesses for the use cases described below.**
 
 ## Disclaimer
 
 **This is a pseudo load-balancer.**
```

### Comparing `openai_priority_loadbalancer-1.0.1/PKG-INFO` & `openai_priority_loadbalancer-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_priority_loadbalancer
-Version: 1.0.1
+Version: 1.0.2
 Summary: A multi-backend, prioritization load balancer for OpenAI
 Author-email: Simon Kurtz <simonkurtz@gmail.com>
 Project-URL: Homepage, https://github.com/simonkurtz-MSFT/python-openai-loadbalancer
 Project-URL: Issues, https://github.com/simonkurtz-MSFT/python-openai-loadbalancer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,15 +21,15 @@
 - Prioritize exhaustion of all tokens in a PTU instance with a fallback onto multiple consumption instances.
 - Tiered prioritization of multiple consumption instances (e.g. use instances first that are geographically closer).
 
 While the [OpenAI Python API library](https://github.com/openai/openai-python) respects HTTP 429 and automatically retries after the requested wait period, the library is not set up to support the aforementioned customer desires. The library does, however, allow for the injection of custom httpx clients. This gave rise to this project.
 
 And while there are other Python OpenAI load balancers freely available, I have not seen one yet that addresses the aforementioned scenarios.
 
-Python OpenAI LoadBalancer is injected cleanly into the OpenAI Python API library. The changes between a conventional and a load-balanced Azure OpenAI implementation are few and almost entirely configuration of the backends to be used. You can see a side-by-side example in the [aoai.py](./aoai.py) file in this repo.
+Python OpenAI Load Balancer is injected cleanly into the OpenAI Python API library. The changes between a conventional and a load-balanced Azure OpenAI implementation are few and almost entirely configuration of the backends to be used. You can see a side-by-side example in the [aoai.py](https://github.com/simonkurtz-MSFT/python-openai-loadbalancer/blob/main/aoai.py) file in this repo.
 
 **Please refer to the GitHub repo for detailed test harnesses for the use cases described below.**
 
 ## Disclaimer
 
 **This is a pseudo load-balancer.**
```

### Comparing `openai_priority_loadbalancer-1.0.1/README.md` & `openai_priority_loadbalancer-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `openai_priority_loadbalancer-1.0.1/pyproject.toml` & `openai_priority_loadbalancer-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "openai_priority_loadbalancer"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Simon Kurtz", email="simonkurtz@gmail.com" },
 ]
 description = "A multi-backend, prioritization load balancer for OpenAI"
 readme = "PACKAGE_README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `openai_priority_loadbalancer-1.0.1/src/openai_priority_loadbalancer/openai_priority_loadbalancer.py` & `openai_priority_loadbalancer-1.0.2/src/openai_priority_loadbalancer/openai_priority_loadbalancer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,33 @@
-from datetime import datetime, MINYEAR, MAXYEAR, timedelta, timezone
-from dateutil.tz import tzutc
-from httpx import Client, Response, BaseTransport, AsyncBaseTransport, AsyncClient
-from typing import List
+"""Module providing a prioritized load-balancing for Azure OpenAI."""
+
 import logging
 import random
 import traceback
+from typing import List
+from datetime import datetime, MAXYEAR, MINYEAR, timedelta, timezone
+from dateutil.tz import tzutc
+from httpx import AsyncClient, Client, Response
 
 class Backend:
+    """Class representing a backend object used with Azure OpenAI, etc."""
+
     # Constructor
     def __init__(self, host: str, priority: int):
         self.host = host
         self.priority = priority
         self.is_throttling = False
         self.retry_after = datetime.min
         self.successful_call_count = 0
 
 # Reference design at https://github.com/encode/httpx/blob/master/httpx/_transports/base.py
 # BaseLoadBalancer providing functionality to both synchronous and asynchronous load balancers
 class BaseLoadBalancer():
+    """Logically abstract Base Load Balancer class that should be inherited"""
+
     # Constructor
     def __init__(self, transport, backends: List[Backend]):
         self._transport = transport
         self.backends = backends
         self._backend_index = -1
         self._remaining_backends = 1
         self._log = logging.getLogger("openai-priority-loadbalancer")     # https://www.loggly.com/ultimate-guide/python-logging-basics/
@@ -30,44 +36,43 @@
     def _check_throttling(self):
         min_datetime = datetime(MINYEAR, 1, 1, tzinfo = tzutc())
 
         for backend in self.backends:
             if backend.is_throttling and datetime.now(tzutc()) >= backend.retry_after:
                 backend.is_throttling = False
                 backend.retry_after = min_datetime
-                self._log.info(f"Backend {backend.host} is no longer throttling.")
+                self._log.info("Backend %s is no longer throttling.", backend.host)
 
     def _get_backend_index(self):
         # This is the main logic to pick the backend to be used
         selected_priority = float('inf')
         available_backends = []
 
-        for i in range(len(self.backends)):
-            backend = self.backends[i]
-
+        # Evaluate all defined backends for availability and priority, leaving only the most-desirable available backends from which to select.
+        for i, backend in enumerate(self.backends):
             if not backend.is_throttling:
-                backendPriority = backend.priority
+                backend_priority = backend.priority
 
-                if backendPriority < selected_priority:
-                    selected_priority = backendPriority
+                if backend_priority < selected_priority:
+                    selected_priority = backend_priority
                     available_backends.clear()
                     available_backends.append(i)
-                elif backendPriority == selected_priority:
+                elif backend_priority == selected_priority:
                     available_backends.append(i)
 
         if len(available_backends) == 1:
             return available_backends[0]
 
         if len(available_backends) > 0:
             # Since this code is very likely being called from multiple python instances with multiple workers in parallel executions, there's no way to distribute requests uniformly across all Azure OpenAI instances.
             # Doing so would require a centralized service, cache, etc. to keep track of a common backends list, but that would also imply a locking mechanism for updates, which would
             # immediately inhibit the performance benefits of the load balancer. This is why this is more of a pseudo load-balancer. Therefore, we'll just randomize across the available backends.
             return random.choice(available_backends)
         else:
-            # If there are no available Backend, -1 will be returned to indicate that nothing is available (and that we should bail).
+            # If there are no available backends, -1 will be returned to indicate that nothing is available (and that we consequently need to bail by returning an HTTP 429).
             return -1
 
     def _get_remaining_backends(self):
         self._remaining_backends = 0
 
         for backend in self.backends:
             if not backend.is_throttling:
@@ -80,83 +85,87 @@
 
         for backend in self.backends:
             if backend.is_throttling and backend.retry_after < soonest_retry_after:
                 soonest_retry_after = backend.retry_after
                 soonest_backend = backend.host
 
         delay = int((soonest_retry_after - datetime.now(timezone.utc)).total_seconds()) + 1     # Add a 1 second buffer to ensure we don't retry too early
-        self._log.info(f"Soonest Retry After: {soonest_backend} - {str(delay)} second(s)")
+        self._log.info("Soonest Retry After: %s - %s second(s)", soonest_backend, str(delay))
         return delay
 
     def _handle_200_399_response(self, request, response, backend_index):
         # Successful requests
-        self._log.info(f"Request sent to server: {request.url}, Status code: {response.status_code}")
+        self._log.info("Request sent to server: %s, Status code: %s", request.url, response.status_code)
         self.backends[backend_index].successful_call_count += 1
 
     def _handle_429_5xx_response(self, request, response, backend_index):
         # If the server is throttling or there's a server error, retry with a different server
-        self._log.info(f"Request sent to server: {request.url}, Status Code: {response.status_code} - FAIL")
+        self._log.info("Request sent to server: %s, Status code: %s - FAIL", request.url, response.status_code)
 
         retry_after = int(response.headers.get('Retry-After', '-1'))
 
         if retry_after == -1:
             retry_after = int(response.headers.get('x-ratelimit-reset-requests', '-1'))
 
         if retry_after == -1:
             retry_after = int(response.headers.get('x-ratelimit-reset-requests', '10'))
 
-        self._log.info(f"Backend {self.backends[backend_index].host} is throttling. Retry after {retry_after} second(s).")
+        self._log.info("Backend %s is throttling. Retry after %s second(s).", self.backends[backend_index].host, retry_after)
 
         backend = self.backends[backend_index]
         backend.is_throttling = True
         backend.retry_after = datetime.now(tzutc()) + timedelta(seconds = retry_after)
         self._get_remaining_backends()
 
     def _handle_4xx_response(self, request, response):
         # Would likely be a 4xx error other than 429
-        self._log.warning(f"Request sent to server: {request.url}, Status code: {response.status_code} - FAIL")
+        self._log.warning("Request sent to server: %s, Status code: %s - FAIL", request.url, response.status_code)
 
-    def modify_request(self, request, backend_index):
+    def _modify_request(self, request, backend_index):
         # Modify the request. Note that only the URL and Host header are being modified on the original request object. We make the smallest incision possible to avoid side effects.
         # Update URL and host header as both must match the backend server.
         request.url = request.url.copy_with(host = self.backends[backend_index].host)
         request.headers = request.headers.copy()    # Create a mutable copy of the headers
         request.headers['host'] = self.backends[backend_index].host
 
     def _return_429(self):
         self._log.warning("No backend available!")
         retry_after = str(self._get_soonest_retry_after())
-        self._log.info(f"Returning HTTP 429 with Retry-After header value of {retry_after} second(s).")
+        self._log.info("Returning HTTP 429 with Retry-After header value of %s second(s).", retry_after)
         return Response(429, content = '', headers={'Retry-After': retry_after})
 
 class AsyncLoadBalancer(BaseLoadBalancer):
+    """Asynchronous Load Balancer class based on BaseLoadBalancer"""
+
     # Constructor
     def __init__(self, backends: List[Backend]):
         super().__init__(AsyncClient(), backends)
 
     # Public Methods
     async def handle_async_request(self, request):
+        """Handles an asynchronous request by issuing an asynchronous request to an available backed."""
+
         self._check_throttling()
         self._get_remaining_backends()
         response = None
 
         while True and self._remaining_backends > 0:
             # 1) Determine the appropriate backend to use
             backend_index = self._get_backend_index()
 
             if backend_index == -1:
                 return self._return_429()
 
             # 2) Modify the intercepted request
-            self.modify_request(request, backend_index)
+            self._modify_request(request, backend_index)
 
             # 3) Send the request to the selected backend (via async)
             try:
                 response = await self._transport.send(request)
-            except Exception as e:
+            except Exception:
                 self._log.error(traceback.print_exc())
 
             # 4) Evaluate the response from the backend
             if response is not None and (response.status_code == 429 or response.status_code >= 500):
                 self._handle_429_5xx_response(request, response, backend_index)
                 continue
 
@@ -170,38 +179,42 @@
 
         if self._remaining_backends == 0:
             return self._return_429()
 
         return response
 
 class LoadBalancer(BaseLoadBalancer):
+    """Synchronous Load Balancer class based on BaseLoadBalancer"""
+
     # Constructor
     def __init__(self, backends: List[Backend]):
         super().__init__(Client(), backends)
 
     # Public Methods
     def handle_request(self, request):
+        """Handles a synchronous request by issuing a request to an available backed."""
+
         self._check_throttling()
         self._get_remaining_backends()
         response = None
 
         while True and self._remaining_backends > 0:
             # 1) Determine the appropriate backend to use
             backend_index = self._get_backend_index()
 
             if backend_index == -1:
                 return self._return_429()
 
             # 2) Modify the intercepted request
-            self.modify_request(request, backend_index)
+            self._modify_request(request, backend_index)
 
             # 3) Send the request to the selected backend
             try:
                 response = self._transport.send(request)
-            except Exception as e:
+            except Exception:
                 self._log.error(traceback.print_exc())
 
             # 4) Evaluate the response from the backend
             if response is not None and (response.status_code == 429 or response.status_code >= 500):
                 self._handle_429_5xx_response(request, response, backend_index)
                 continue
```

### Comparing `openai_priority_loadbalancer-1.0.1/src/openai_priority_loadbalancer.egg-info/PKG-INFO` & `openai_priority_loadbalancer-1.0.2/src/openai_priority_loadbalancer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_priority_loadbalancer
-Version: 1.0.1
+Version: 1.0.2
 Summary: A multi-backend, prioritization load balancer for OpenAI
 Author-email: Simon Kurtz <simonkurtz@gmail.com>
 Project-URL: Homepage, https://github.com/simonkurtz-MSFT/python-openai-loadbalancer
 Project-URL: Issues, https://github.com/simonkurtz-MSFT/python-openai-loadbalancer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,15 +21,15 @@
 - Prioritize exhaustion of all tokens in a PTU instance with a fallback onto multiple consumption instances.
 - Tiered prioritization of multiple consumption instances (e.g. use instances first that are geographically closer).
 
 While the [OpenAI Python API library](https://github.com/openai/openai-python) respects HTTP 429 and automatically retries after the requested wait period, the library is not set up to support the aforementioned customer desires. The library does, however, allow for the injection of custom httpx clients. This gave rise to this project.
 
 And while there are other Python OpenAI load balancers freely available, I have not seen one yet that addresses the aforementioned scenarios.
 
-Python OpenAI LoadBalancer is injected cleanly into the OpenAI Python API library. The changes between a conventional and a load-balanced Azure OpenAI implementation are few and almost entirely configuration of the backends to be used. You can see a side-by-side example in the [aoai.py](./aoai.py) file in this repo.
+Python OpenAI Load Balancer is injected cleanly into the OpenAI Python API library. The changes between a conventional and a load-balanced Azure OpenAI implementation are few and almost entirely configuration of the backends to be used. You can see a side-by-side example in the [aoai.py](https://github.com/simonkurtz-MSFT/python-openai-loadbalancer/blob/main/aoai.py) file in this repo.
 
 **Please refer to the GitHub repo for detailed test harnesses for the use cases described below.**
 
 ## Disclaimer
 
 **This is a pseudo load-balancer.**
```

