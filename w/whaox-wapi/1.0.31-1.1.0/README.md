# Comparing `tmp/whaox-wapi-1.0.31.tar.gz` & `tmp/whaox-wapi-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whaox-wapi-1.0.31.tar", last modified: Thu May  9 16:01:19 2024, max compression
+gzip compressed data, was "whaox-wapi-1.1.0.tar", last modified: Thu May 16 18:03:17 2024, max compression
```

## Comparing `whaox-wapi-1.0.31.tar` & `whaox-wapi-1.1.0.tar`

### file list

```diff
@@ -1,32 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 16:01:19.207046 whaox-wapi-1.0.31/
--rw-rw-rw-   0        0        0     1083 2024-04-11 20:02:10.000000 whaox-wapi-1.0.31/LICENSE
--rw-rw-rw-   0        0        0     3020 2024-05-09 16:01:19.204104 whaox-wapi-1.0.31/PKG-INFO
--rw-rw-rw-   0        0        0     2632 2024-04-15 10:27:15.000000 whaox-wapi-1.0.31/README.md
--rw-rw-rw-   0        0        0       42 2024-05-09 16:01:19.207124 whaox-wapi-1.0.31/setup.cfg
--rw-rw-rw-   0        0        0      800 2024-05-09 16:01:16.000000 whaox-wapi-1.0.31/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-09 16:01:19.164600 whaox-wapi-1.0.31/tests/
--rw-rw-rw-   0        0        0      952 2024-05-09 16:00:05.000000 whaox-wapi-1.0.31/tests/test.py
-drwxrwxrwx   0        0        0        0 2024-05-09 16:01:19.165130 whaox-wapi-1.0.31/wapi/
--rw-rw-rw-   0        0        0       27 2024-04-15 09:31:56.000000 whaox-wapi-1.0.31/wapi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 16:01:19.168773 whaox-wapi-1.0.31/wapi/features/
--rw-rw-rw-   0        0        0      973 2024-05-09 15:55:00.000000 whaox-wapi-1.0.31/wapi/features/GET.py
--rw-rw-rw-   0        0        0      797 2024-05-08 20:23:21.000000 whaox-wapi-1.0.31/wapi/features/POST.py
--rw-rw-rw-   0        0        0      837 2024-05-09 11:47:35.000000 whaox-wapi-1.0.31/wapi/features/Route.py
--rw-rw-rw-   0        0        0       72 2024-04-12 10:19:11.000000 whaox-wapi-1.0.31/wapi/features/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 16:01:19.170884 whaox-wapi-1.0.31/wapi/static/
--rw-rw-rw-   0        0        0       48 2024-04-11 20:01:35.000000 whaox-wapi-1.0.31/wapi/static/T.py
--rw-rw-rw-   0        0        0        0 2024-04-15 09:20:58.000000 whaox-wapi-1.0.31/wapi/static/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 16:01:19.176808 whaox-wapi-1.0.31/wapi/utils/
--rw-rw-rw-   0        0        0        0 2024-04-15 09:21:14.000000 whaox-wapi-1.0.31/wapi/utils/__init__.py
--rw-rw-rw-   0        0        0      307 2024-05-08 19:32:55.000000 whaox-wapi-1.0.31/wapi/utils/get_path.py
--rw-rw-rw-   0        0        0       54 2024-05-09 11:47:35.000000 whaox-wapi-1.0.31/wapi/utils/is_class.py
--rw-rw-rw-   0        0        0      124 2024-04-11 20:01:35.000000 whaox-wapi-1.0.31/wapi/utils/is_dataclass.py
--rw-rw-rw-   0        0        0       59 2024-05-09 09:32:44.000000 whaox-wapi-1.0.31/wapi/utils/is_object.py
--rw-rw-rw-   0        0        0      390 2024-05-09 10:55:41.000000 whaox-wapi-1.0.31/wapi/utils/merge_paths.py
--rw-rw-rw-   0        0        0      250 2024-05-09 10:56:52.000000 whaox-wapi-1.0.31/wapi/utils/set_path.py
-drwxrwxrwx   0        0        0        0 2024-05-09 16:01:19.202928 whaox-wapi-1.0.31/whaox_wapi.egg-info/
--rw-rw-rw-   0        0        0     3020 2024-05-09 16:01:19.000000 whaox-wapi-1.0.31/whaox_wapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      528 2024-05-09 16:01:19.000000 whaox-wapi-1.0.31/whaox_wapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 16:01:19.000000 whaox-wapi-1.0.31/whaox_wapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-09 16:01:19.000000 whaox-wapi-1.0.31/whaox_wapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-09 16:01:19.000000 whaox-wapi-1.0.31/whaox_wapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 18:03:17.013820 whaox-wapi-1.1.0/
+-rw-rw-rw-   0        0        0     1083 2024-04-11 20:02:10.000000 whaox-wapi-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     3041 2024-05-16 18:03:17.012023 whaox-wapi-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2632 2024-04-15 10:27:15.000000 whaox-wapi-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-16 18:03:17.014328 whaox-wapi-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      932 2024-05-16 18:03:08.000000 whaox-wapi-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 18:03:16.942027 whaox-wapi-1.1.0/wapi/
+-rw-rw-rw-   0        0        0       27 2024-04-15 09:31:56.000000 whaox-wapi-1.1.0/wapi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 18:03:16.949501 whaox-wapi-1.1.0/wapi/features/
+-rw-rw-rw-   0        0        0      669 2024-05-16 17:54:49.000000 whaox-wapi-1.1.0/wapi/features/DELETE.py
+-rw-rw-rw-   0        0        0      663 2024-05-16 18:00:57.000000 whaox-wapi-1.1.0/wapi/features/GET.py
+-rw-rw-rw-   0        0        0      667 2024-05-16 17:54:49.000000 whaox-wapi-1.1.0/wapi/features/PATCH.py
+-rw-rw-rw-   0        0        0      659 2024-05-16 18:00:57.000000 whaox-wapi-1.1.0/wapi/features/POST.py
+-rw-rw-rw-   0        0        0      663 2024-05-16 17:54:49.000000 whaox-wapi-1.1.0/wapi/features/PUT.py
+-rw-rw-rw-   0        0        0      837 2024-05-09 11:47:35.000000 whaox-wapi-1.1.0/wapi/features/Route.py
+-rw-rw-rw-   0        0        0      148 2024-05-16 18:00:57.000000 whaox-wapi-1.1.0/wapi/features/__init__.py
+-rw-rw-rw-   0        0        0     1263 2024-05-16 17:49:50.000000 whaox-wapi-1.1.0/wapi/features/request.py
+drwxrwxrwx   0        0        0        0 2024-05-16 18:03:16.954884 whaox-wapi-1.1.0/wapi/static/
+-rw-rw-rw-   0        0        0       48 2024-04-11 20:01:35.000000 whaox-wapi-1.1.0/wapi/static/T.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 09:20:58.000000 whaox-wapi-1.1.0/wapi/static/__init__.py
+-rw-rw-rw-   0        0        0      118 2024-05-16 16:57:54.000000 whaox-wapi-1.1.0/wapi/static/methods.py
+-rw-rw-rw-   0        0        0      440 2024-05-16 17:01:19.000000 whaox-wapi-1.1.0/wapi/static/params.py
+drwxrwxrwx   0        0        0        0 2024-05-16 18:03:16.963902 whaox-wapi-1.1.0/wapi/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-15 09:21:14.000000 whaox-wapi-1.1.0/wapi/utils/__init__.py
+-rw-rw-rw-   0        0        0      299 2024-05-14 15:31:03.000000 whaox-wapi-1.1.0/wapi/utils/get_path.py
+-rw-rw-rw-   0        0        0      252 2024-05-16 17:25:56.000000 whaox-wapi-1.1.0/wapi/utils/get_used_vars.py
+-rw-rw-rw-   0        0        0       54 2024-05-09 11:47:35.000000 whaox-wapi-1.1.0/wapi/utils/is_class.py
+-rw-rw-rw-   0        0        0      124 2024-04-11 20:01:35.000000 whaox-wapi-1.1.0/wapi/utils/is_dataclass.py
+-rw-rw-rw-   0        0        0       59 2024-05-09 09:32:44.000000 whaox-wapi-1.1.0/wapi/utils/is_object.py
+-rw-rw-rw-   0        0        0      311 2024-05-14 15:31:03.000000 whaox-wapi-1.1.0/wapi/utils/merge_paths.py
+-rw-rw-rw-   0        0        0      242 2024-05-14 15:31:57.000000 whaox-wapi-1.1.0/wapi/utils/set_path.py
+drwxrwxrwx   0        0        0        0 2024-05-16 18:03:17.009353 whaox-wapi-1.1.0/whaox_wapi.egg-info/
+-rw-rw-rw-   0        0        0     3041 2024-05-16 18:03:16.000000 whaox-wapi-1.1.0/whaox_wapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      680 2024-05-16 18:03:16.000000 whaox-wapi-1.1.0/whaox_wapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 18:03:16.000000 whaox-wapi-1.1.0/whaox_wapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-16 18:03:16.000000 whaox-wapi-1.1.0/whaox_wapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-16 18:03:16.000000 whaox-wapi-1.1.0/whaox_wapi.egg-info/top_level.txt
```

### Comparing `whaox-wapi-1.0.31/LICENSE` & `whaox-wapi-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `whaox-wapi-1.0.31/PKG-INFO` & `whaox-wapi-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: whaox-wapi
-Version: 1.0.31
+Version: 1.1.0
 Summary: Web-Library for Python
 Home-page: https://github.com/topanim/WApi
 Author: WHAOX
 Author-email: gorogannisan641@gmail.com
 License: MIT LICENSE, see LICENSE file
-Keywords: python,web,api,requests,post,get
+Keywords: python,web,api,requests,post,get,put,patch,delete,rest
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: jsons
 Requires-Dist: requests
 
 
 # WApi: Web-Library for Python
```

### Comparing `whaox-wapi-1.0.31/README.md` & `whaox-wapi-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `whaox-wapi-1.0.31/setup.py` & `whaox-wapi-1.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 #!/usr/bin/env python
 
 from io import open
+
 from setuptools import setup, find_packages
 
 """
 :authors: WHAOX
 :license: MIT License, see LICENSE file
 :copyright: (c) 2024 WHAOX
 """
 
-version = '1.0.31'
+version = '1.1.0'
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='whaox-wapi',
     version=version,
@@ -28,9 +29,20 @@
     url='https://github.com/topanim/WApi',
 
     license='MIT LICENSE, see LICENSE file',
 
     packages=find_packages(),
     install_requires=['jsons', 'requests'],
 
-    keywords=['python', 'web', 'api', 'requests', 'post', 'get']
+    keywords=[
+        'python',
+        'web',
+        'api',
+        'requests',
+        'post',
+        'get',
+        'put',
+        'patch',
+        'delete',
+        'rest'
+    ]
 )
```

### Comparing `whaox-wapi-1.0.31/wapi/features/GET.py` & `whaox-wapi-1.1.0/wapi/features/GET.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,29 @@
 from functools import wraps
 
-from jsons import load
-from requests import Response, get
+from requests import Response
 
+from wapi.features.request import make_request
 from wapi.static.T import T
+from wapi.static.methods import HTTPMethod
 from wapi.utils.get_path import get_path
 
 
 def GET(
         path: str = "",
-        _T: T = None,
-        *,
-        auto: bool = False,
-        unpack: bool = False
+        _T: T = None
 ) -> T | Response:
     def decorator(func):
         @wraps(func)
         def wrapper(self, *args, **kwargs):
-            headers = kwargs.pop("headers", None)
             p = get_path(self, func, path)
-            url = p.format(*args, **kwargs)
-            if auto:
-                if unpack and (body := kwargs.pop('body', None)):
-                    kwargs.update(body)
-
-                url += "?" + "&".join([f'{k}={v}' for k, v in kwargs.items()])
-
-            response = get(url, headers=headers)
-
-            if _T is None:
-                return response
-            return load(response.json(), _T)
 
+            return make_request(
+                url=p,
+                method=HTTPMethod.GET,
+                _T=_T,
+                data=kwargs
+            )
         return wrapper
 
     return decorator
+
```

### Comparing `whaox-wapi-1.0.31/wapi/features/POST.py` & `whaox-wapi-1.1.0/wapi/features/PATCH.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 from functools import wraps
 
-from jsons import load, dump
-from requests import Response, post
+from requests import Response
 
+from wapi.features.request import make_request
 from wapi.static.T import T
+from wapi.static.methods import HTTPMethod
 from wapi.utils.get_path import get_path
 
 
-def POST(
+def PATCH(
         path: str = "",
-        _T: T = None,
+        _T: T = None
 ) -> T | Response:
     def decorator(func):
         @wraps(func)
-        def wrapper(self, **kwargs):
-            headers = kwargs.pop('headers', None)
-            data = dict()
-
-            if body := dump(kwargs.pop('body', None)):
-                data.update(body)
-
-            url = get_path(self, func, path).format(**kwargs)
-            response = post(url, json=data, headers=headers)
-
-            if _T is None:
-                return response
-            return load(response.json(), _T)
+        def wrapper(self, *args, **kwargs):
+            p = get_path(self, func, path)
+
+            return make_request(
+                url=p,
+                method=HTTPMethod.PATCH,
+                _T=_T,
+                data=kwargs
+            )
 
         return wrapper
 
     return decorator
```

### Comparing `whaox-wapi-1.0.31/wapi/features/Route.py` & `whaox-wapi-1.1.0/wapi/features/Route.py`

 * *Files identical despite different names*

### Comparing `whaox-wapi-1.0.31/whaox_wapi.egg-info/PKG-INFO` & `whaox-wapi-1.1.0/whaox_wapi.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: whaox-wapi
-Version: 1.0.31
+Version: 1.1.0
 Summary: Web-Library for Python
 Home-page: https://github.com/topanim/WApi
 Author: WHAOX
 Author-email: gorogannisan641@gmail.com
 License: MIT LICENSE, see LICENSE file
-Keywords: python,web,api,requests,post,get
+Keywords: python,web,api,requests,post,get,put,patch,delete,rest
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: jsons
 Requires-Dist: requests
 
 
 # WApi: Web-Library for Python
```

