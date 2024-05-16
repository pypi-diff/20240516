# Comparing `tmp/octoxlabs-0.2.3.tar.gz` & `tmp/octoxlabs-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octoxlabs-0.2.3.tar", last modified: Mon Feb 20 10:48:27 2023, max compression
+gzip compressed data, was "octoxlabs-0.4.3.tar", last modified: Thu May 16 19:21:07 2024, max compression
```

## Comparing `octoxlabs-0.2.3.tar` & `octoxlabs-0.4.3.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 ogulcankahraman   (501) staff       (20)        0 2023-02-20 10:48:27.094493 octoxlabs-0.2.3/
--rw-r--r--   0 ogulcankahraman   (501) staff       (20)     1071 2023-02-20 10:31:34.000000 octoxlabs-0.2.3/LICENSE
--rw-r--r--   0 ogulcankahraman   (501) staff       (20)     2401 2023-02-20 10:48:27.094304 octoxlabs-0.2.3/PKG-INFO
--rw-r--r--   0 ogulcankahraman   (501) staff       (20)      663 2023-02-20 10:31:34.000000 octoxlabs-0.2.3/README.md
--rw-r--r--   0 ogulcankahraman   (501) staff       (20)      838 2023-02-20 10:48:21.000000 octoxlabs-0.2.3/pyproject.toml
--rw-r--r--   0 ogulcankahraman   (501) staff       (20)       38 2023-02-20 10:48:27.094542 octoxlabs-0.2.3/setup.cfg
-drwxr-xr-x   0 ogulcankahraman   (501) staff       (20)        0 2023-02-20 10:48:27.091358 octoxlabs-0.2.3/src/
--rw-r--r--   0 ogulcankahraman   (501) staff       (20)      668 2023-02-20 10:39:05.000000 octoxlabs-0.2.3/src/example.py
-drwxr-xr-x   0 ogulcankahraman   (501) staff       (20)        0 2023-02-20 10:48:27.092466 octoxlabs-0.2.3/src/octoxlabs/
--rw-r--r--   0 ogulcankahraman   (501) staff       (20)       79 2023-02-20 10:31:34.000000 octoxlabs-0.2.3/src/octoxlabs/__init__.py
-drwxr-xr-x   0 ogulcankahraman   (501) staff       (20)        0 2023-02-20 10:48:27.093384 octoxlabs-0.2.3/src/octoxlabs/constants/
--rw-r--r--   0 ogulcankahraman   (501) staff       (20)        0 2023-02-20 10:31:34.000000 octoxlabs-0.2.3/src/octoxlabs/constants/__init__.py
--rw-r--r--   0 ogulcankahraman   (501) staff       (20)      814 2023-02-20 10:38:17.000000 octoxlabs-0.2.3/src/octoxlabs/constants/paths.py
--rw-r--r--   0 ogulcankahraman   (501) staff       (20)      124 2023-02-20 10:31:34.000000 octoxlabs-0.2.3/src/octoxlabs/exceptions.py
-drwxr-xr-x   0 ogulcankahraman   (501) staff       (20)        0 2023-02-20 10:48:27.094070 octoxlabs-0.2.3/src/octoxlabs/models/
--rw-r--r--   0 ogulcankahraman   (501) staff       (20)        0 2023-02-20 10:31:34.000000 octoxlabs-0.2.3/src/octoxlabs/models/__init__.py
--rw-r--r--   0 ogulcankahraman   (501) staff       (20)     2346 2023-02-20 10:31:34.000000 octoxlabs-0.2.3/src/octoxlabs/models/adapter.py
--rw-r--r--   0 ogulcankahraman   (501) staff       (20)      651 2023-02-20 10:31:34.000000 octoxlabs-0.2.3/src/octoxlabs/models/discovery.py
--rw-r--r--   0 ogulcankahraman   (501) staff       (20)     1308 2023-02-20 10:31:34.000000 octoxlabs-0.2.3/src/octoxlabs/models/query.py
--rw-r--r--   0 ogulcankahraman   (501) staff       (20)     6723 2023-02-20 10:31:34.000000 octoxlabs-0.2.3/src/octoxlabs/octoxlabs.py
--rw-r--r--   0 ogulcankahraman   (501) staff       (20)     1273 2023-02-20 10:31:34.000000 octoxlabs-0.2.3/src/octoxlabs/service.py
--rw-r--r--   0 ogulcankahraman   (501) staff       (20)      165 2023-02-20 10:31:34.000000 octoxlabs-0.2.3/src/octoxlabs/utils.py
-drwxr-xr-x   0 ogulcankahraman   (501) staff       (20)        0 2023-02-20 10:48:27.093161 octoxlabs-0.2.3/src/octoxlabs.egg-info/
--rw-r--r--   0 ogulcankahraman   (501) staff       (20)     2401 2023-02-20 10:48:27.000000 octoxlabs-0.2.3/src/octoxlabs.egg-info/PKG-INFO
--rw-r--r--   0 ogulcankahraman   (501) staff       (20)      558 2023-02-20 10:48:27.000000 octoxlabs-0.2.3/src/octoxlabs.egg-info/SOURCES.txt
--rw-r--r--   0 ogulcankahraman   (501) staff       (20)        1 2023-02-20 10:48:27.000000 octoxlabs-0.2.3/src/octoxlabs.egg-info/dependency_links.txt
--rw-r--r--   0 ogulcankahraman   (501) staff       (20)       17 2023-02-20 10:48:27.000000 octoxlabs-0.2.3/src/octoxlabs.egg-info/requires.txt
--rw-r--r--   0 ogulcankahraman   (501) staff       (20)       18 2023-02-20 10:48:27.000000 octoxlabs-0.2.3/src/octoxlabs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:07.724658 octoxlabs-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-16 19:21:01.000000 octoxlabs-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-05-16 19:21:07.720658 octoxlabs-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-16 19:21:01.000000 octoxlabs-0.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-16 19:21:01.000000 octoxlabs-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 19:21:07.724658 octoxlabs-0.4.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:07.716658 octoxlabs-0.4.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:07.720658 octoxlabs-0.4.3/src/octoxlabs/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-16 19:21:01.000000 octoxlabs-0.4.3/src/octoxlabs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:07.720658 octoxlabs-0.4.3/src/octoxlabs/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:01.000000 octoxlabs-0.4.3/src/octoxlabs/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-16 19:21:01.000000 octoxlabs-0.4.3/src/octoxlabs/constants/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-16 19:21:01.000000 octoxlabs-0.4.3/src/octoxlabs/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:07.720658 octoxlabs-0.4.3/src/octoxlabs/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:01.000000 octoxlabs-0.4.3/src/octoxlabs/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-16 19:21:01.000000 octoxlabs-0.4.3/src/octoxlabs/models/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-16 19:21:01.000000 octoxlabs-0.4.3/src/octoxlabs/models/companies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-16 19:21:01.000000 octoxlabs-0.4.3/src/octoxlabs/models/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-16 19:21:01.000000 octoxlabs-0.4.3/src/octoxlabs/models/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-16 19:21:01.000000 octoxlabs-0.4.3/src/octoxlabs/models/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20926 2024-05-16 19:21:01.000000 octoxlabs-0.4.3/src/octoxlabs/octoxlabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-16 19:21:01.000000 octoxlabs-0.4.3/src/octoxlabs/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-16 19:21:01.000000 octoxlabs-0.4.3/src/octoxlabs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:07.720658 octoxlabs-0.4.3/src/octoxlabs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-05-16 19:21:07.000000 octoxlabs-0.4.3/src/octoxlabs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-16 19:21:07.000000 octoxlabs-0.4.3/src/octoxlabs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 19:21:07.000000 octoxlabs-0.4.3/src/octoxlabs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-16 19:21:07.000000 octoxlabs-0.4.3/src/octoxlabs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-16 19:21:07.000000 octoxlabs-0.4.3/src/octoxlabs.egg-info/top_level.txt
```

### Comparing `octoxlabs-0.2.3/LICENSE` & `octoxlabs-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `octoxlabs-0.2.3/PKG-INFO` & `octoxlabs-0.4.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octoxlabs
-Version: 0.2.3
+Version: 0.4.3
 Summary: py-octoxlabs is an API client for Octox Labs Cyber Security Asset Management platform on python programming language.
 Author-email: Octox Labs Development Team <development@octoxlabs.com>
 License: MIT License
         
         Copyright (c) 2022 Octox Labs Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,14 +26,16 @@
         SOFTWARE.
 Project-URL: Homepage, https://github.com/octoxlabs/py-octoxlabs
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: urllib3
 
 # Octox Labs Python SDK
 py-octoxlabs is an API client for Octox Labs Cyber Security Asset Management platform on python programming language.
 
 ## Installation
 ```shell
 pip install octoxlabs
```

### Comparing `octoxlabs-0.2.3/README.md` & `octoxlabs-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `octoxlabs-0.2.3/pyproject.toml` & `octoxlabs-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "octoxlabs"
-version = "0.2.3"
+version = "0.4.3"
 authors = [
   { name="Octox Labs Development Team", email="development@octoxlabs.com" },
 ]
 description = "py-octoxlabs is an API client for Octox Labs Cyber Security Asset Management platform on python programming language."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `octoxlabs-0.2.3/src/octoxlabs/models/adapter.py` & `octoxlabs-0.4.3/src/octoxlabs/models/adapter.py`

 * *Files identical despite different names*

### Comparing `octoxlabs-0.2.3/src/octoxlabs/models/discovery.py` & `octoxlabs-0.4.3/src/octoxlabs/models/discovery.py`

 * *Files identical despite different names*

### Comparing `octoxlabs-0.2.3/src/octoxlabs/models/query.py` & `octoxlabs-0.4.3/src/octoxlabs/models/query.py`

 * *Files identical despite different names*

### Comparing `octoxlabs-0.2.3/src/octoxlabs/service.py` & `octoxlabs-0.4.3/src/octoxlabs/service.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,38 +4,43 @@
 
 # Third Party
 import urllib3
 import requests
 
 # Local Folder
 from .exceptions import ApiException
+from .constants.paths import access_token_path
 
 urllib3.disable_warnings()
 
 
 class OctoxLabsService:
     ip: str
     base_url: str
 
     token: str
-    token_prefix: str = "Octoxlabs"
+    access_token: str
+    token_prefix: str = "Bearer"
 
-    headers: Dict[str, str]
+    headers: Dict[str, str] = None
 
     def __init__(self, ip: str, token: str):
         self.set_ip(ip=ip)
         self.set_token(token=token)
 
     def set_ip(self, ip: str):
         self.ip = ip
         self.base_url = os.getenv("OCTOXLABS_URL", None) or f"https://{self.ip}:8043"
 
     def set_token(self, token: str):
         self.token = token
-        self.headers = {"Authorization": f"{self.token_prefix} {self.token}"}
+        self.access_token = self.request_builder(
+            method="POST", path=access_token_path(), json={"token": self.token}
+        ).json()["access"]
+        self.headers = {"Authorization": f"{self.token_prefix} {self.access_token}"}
 
     def request_builder(
         self,
         path: str,
         method: str = "GET",
         params: Dict[str, Union[str, int]] = None,
         **kwargs,
```

### Comparing `octoxlabs-0.2.3/src/octoxlabs.egg-info/PKG-INFO` & `octoxlabs-0.4.3/src/octoxlabs.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octoxlabs
-Version: 0.2.3
+Version: 0.4.3
 Summary: py-octoxlabs is an API client for Octox Labs Cyber Security Asset Management platform on python programming language.
 Author-email: Octox Labs Development Team <development@octoxlabs.com>
 License: MIT License
         
         Copyright (c) 2022 Octox Labs Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,14 +26,16 @@
         SOFTWARE.
 Project-URL: Homepage, https://github.com/octoxlabs/py-octoxlabs
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: urllib3
 
 # Octox Labs Python SDK
 py-octoxlabs is an API client for Octox Labs Cyber Security Asset Management platform on python programming language.
 
 ## Installation
 ```shell
 pip install octoxlabs
```

### Comparing `octoxlabs-0.2.3/src/octoxlabs.egg-info/SOURCES.txt` & `octoxlabs-0.4.3/src/octoxlabs.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 LICENSE
 README.md
 pyproject.toml
-src/example.py
 src/octoxlabs/__init__.py
 src/octoxlabs/exceptions.py
 src/octoxlabs/octoxlabs.py
 src/octoxlabs/service.py
 src/octoxlabs/utils.py
 src/octoxlabs.egg-info/PKG-INFO
 src/octoxlabs.egg-info/SOURCES.txt
 src/octoxlabs.egg-info/dependency_links.txt
 src/octoxlabs.egg-info/requires.txt
 src/octoxlabs.egg-info/top_level.txt
 src/octoxlabs/constants/__init__.py
 src/octoxlabs/constants/paths.py
 src/octoxlabs/models/__init__.py
 src/octoxlabs/models/adapter.py
+src/octoxlabs/models/companies.py
 src/octoxlabs/models/discovery.py
-src/octoxlabs/models/query.py
+src/octoxlabs/models/query.py
+src/octoxlabs/models/users.py
```

