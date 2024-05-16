# Comparing `tmp/nadeo_api-0.0.2.tar.gz` & `tmp/nadeo_api-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nadeo_api-0.0.2.tar", last modified: Sun May 12 19:27:10 2024, max compression
+gzip compressed data, was "nadeo_api-0.1.0.tar", last modified: Thu May 16 00:26:47 2024, max compression
```

## Comparing `nadeo_api-0.0.2.tar` & `nadeo_api-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 19:27:10.394418 nadeo_api-0.0.2/
--rw-rw-rw-   0        0        0     1064 2024-05-07 17:58:02.000000 nadeo_api-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     2537 2024-05-12 19:27:10.393416 nadeo_api-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      705 2024-05-12 19:26:22.000000 nadeo_api-0.0.2/README.md
--rw-rw-rw-   0        0        0      641 2024-05-12 17:57:41.000000 nadeo_api-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-12 19:27:10.394418 nadeo_api-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-12 19:27:10.352990 nadeo_api-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-12 19:27:10.372821 nadeo_api-0.0.2/src/nadeo_api/
--rw-rw-rw-   0        0        0      227 2024-05-12 17:55:07.000000 nadeo_api-0.0.2/src/nadeo_api/__init__.py
--rw-rw-rw-   0        0        0     6059 2024-05-12 19:19:42.000000 nadeo_api-0.0.2/src/nadeo_api/auth.py
--rw-rw-rw-   0        0        0     4752 2024-05-12 19:12:41.000000 nadeo_api-0.0.2/src/nadeo_api/decode_token_payload.py
--rw-rw-rw-   0        0        0      195 2024-05-08 07:25:08.000000 nadeo_api-0.0.2/src/nadeo_api/iso_to_unix.py
-drwxrwxrwx   0        0        0        0 2024-05-12 19:27:10.392416 nadeo_api-0.0.2/src/nadeo_api.egg-info/
--rw-rw-rw-   0        0        0     2537 2024-05-12 19:27:10.000000 nadeo_api-0.0.2/src/nadeo_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      354 2024-05-12 19:27:10.000000 nadeo_api-0.0.2/src/nadeo_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 19:27:10.000000 nadeo_api-0.0.2/src/nadeo_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-12 19:27:10.000000 nadeo_api-0.0.2/src/nadeo_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-12 19:27:10.000000 nadeo_api-0.0.2/src/nadeo_api.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-12 19:27:10.391417 nadeo_api-0.0.2/tests/
--rw-rw-rw-   0        0        0      257 2024-05-12 19:21:20.000000 nadeo_api-0.0.2/tests/test_auth.py
+drwxrwxrwx   0        0        0        0 2024-05-16 00:26:47.178122 nadeo_api-0.1.0/
+-rw-rw-rw-   0        0        0     1064 2024-05-07 17:58:02.000000 nadeo_api-0.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     3365 2024-05-16 00:26:47.177122 nadeo_api-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1493 2024-05-15 20:11:16.000000 nadeo_api-0.1.0/README.md
+-rw-rw-rw-   0        0        0      671 2024-05-16 00:12:55.000000 nadeo_api-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-16 00:26:47.178122 nadeo_api-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-16 00:26:47.138748 nadeo_api-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-16 00:26:47.150898 nadeo_api-0.1.0/src/nadeo_api/
+-rw-rw-rw-   0        0        0      240 2024-05-16 00:13:14.000000 nadeo_api-0.1.0/src/nadeo_api/__init__.py
+-rw-rw-rw-   0        0        0     9931 2024-05-15 23:21:32.000000 nadeo_api-0.1.0/src/nadeo_api/auth.py
+-rw-rw-rw-   0        0        0     2139 2024-05-16 00:07:27.000000 nadeo_api-0.1.0/src/nadeo_api/core.py
+-rw-rw-rw-   0        0        0     2941 2024-05-16 00:07:12.000000 nadeo_api-0.1.0/src/nadeo_api/live.py
+-rw-rw-rw-   0        0        0        0 2024-05-15 05:36:16.000000 nadeo_api-0.1.0/src/nadeo_api/meet.py
+-rw-rw-rw-   0        0        0        0 2024-05-15 05:36:21.000000 nadeo_api-0.1.0/src/nadeo_api/oauth.py
+drwxrwxrwx   0        0        0        0 2024-05-16 00:26:47.176123 nadeo_api-0.1.0/src/nadeo_api.egg-info/
+-rw-rw-rw-   0        0        0     3365 2024-05-16 00:26:47.000000 nadeo_api-0.1.0/src/nadeo_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2024-05-16 00:26:47.000000 nadeo_api-0.1.0/src/nadeo_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 00:26:47.000000 nadeo_api-0.1.0/src/nadeo_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-16 00:26:47.000000 nadeo_api-0.1.0/src/nadeo_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-16 00:26:47.000000 nadeo_api-0.1.0/src/nadeo_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 00:26:47.175123 nadeo_api-0.1.0/tests/
+-rw-rw-rw-   0        0        0      257 2024-05-12 19:21:20.000000 nadeo_api-0.1.0/tests/test_auth.py
```

### Comparing `nadeo_api-0.0.2/LICENSE.txt` & `nadeo_api-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nadeo_api-0.0.2/PKG-INFO` & `nadeo_api-0.1.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nadeo-api
-Version: 0.0.2
-Summary: Access Nadeo's web services API
+Version: 0.1.0
+Summary: Access Nadeo's web services API and the public Trackmania API
 Author-email: Ezio416 <e@e416.dev>
 License: MIT License
         
         Copyright (c) 2024 Ezio416
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -38,19 +38,29 @@
 # nadeo-api
 
 <!-- [![tests](https://github.com/ezio416/py416/actions/workflows/tests.yml/badge.svg)](https://github.com/ezio416/py-nadeo-api/actions) -->
 <!-- [![docs](https://readthedocs.org/projects/py416/badge/?version=latest)](https://nadeo-api.readthedocs.io/en/latest/) -->
 [![PyPI](https://badge.fury.io/py/nadeo-api.svg)](https://pypi.org/project/nadeo-api/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
-A library to assist with accessing Nadeo's undocumented (officially) web services API.
+A library to assist with accessing Nadeo's web services API and the public Trackmania API (OAuth2).
+
+The web services API has community-driven documentation [here](https://webservices.openplanet.dev/).\
+The main section of this API (named "Core") has an up-to-date list of valid endpoints being kept [here](https://github.com/openplanet-nl/core-api-tracking).\
+Most of these endpoints are not documented at all, but you may help supplement the documentation [here](https://github.com/openplanet-nl/nadeoapi-docs).
+
+The public Trackmania API has official documentation [here](https://api.trackmania.com/doc).
 
 Installing the package from PyPI:
 ```
 python -m pip install nadeo-api
 ```
 
 Using the package:
-```
+```py
 import nadeo_api
-import nadeo_api.auth
+import nadeo_api.auth   # authentication - required for any endpoint
+import nadeo_api.core   # web services Core endpoints
+import nadeo_api.live   # web services Live endpoints
+import nadeo_api.meet   # web services Meet endpoints
+import nadeo_api.oauth  # OAuth2 endpoints (public API)
 ```
```

### Comparing `nadeo_api-0.0.2/pyproject.toml` & `nadeo_api-0.1.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nadeo-api"
-version = "0.0.2"
+version = "0.1.0"
 authors = [
   { name="Ezio416", email="e@e416.dev" },
 ]
-description = "Access Nadeo's web services API"
+description = "Access Nadeo's web services API and the public Trackmania API"
 readme = "README.md"
 license = { file="LICENSE.txt" }
 requires-python = ">=3.12"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
```

### Comparing `nadeo_api-0.0.2/src/nadeo_api.egg-info/PKG-INFO` & `nadeo_api-0.1.0/src/nadeo_api.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nadeo-api
-Version: 0.0.2
-Summary: Access Nadeo's web services API
+Version: 0.1.0
+Summary: Access Nadeo's web services API and the public Trackmania API
 Author-email: Ezio416 <e@e416.dev>
 License: MIT License
         
         Copyright (c) 2024 Ezio416
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -38,19 +38,29 @@
 # nadeo-api
 
 <!-- [![tests](https://github.com/ezio416/py416/actions/workflows/tests.yml/badge.svg)](https://github.com/ezio416/py-nadeo-api/actions) -->
 <!-- [![docs](https://readthedocs.org/projects/py416/badge/?version=latest)](https://nadeo-api.readthedocs.io/en/latest/) -->
 [![PyPI](https://badge.fury.io/py/nadeo-api.svg)](https://pypi.org/project/nadeo-api/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
-A library to assist with accessing Nadeo's undocumented (officially) web services API.
+A library to assist with accessing Nadeo's web services API and the public Trackmania API (OAuth2).
+
+The web services API has community-driven documentation [here](https://webservices.openplanet.dev/).\
+The main section of this API (named "Core") has an up-to-date list of valid endpoints being kept [here](https://github.com/openplanet-nl/core-api-tracking).\
+Most of these endpoints are not documented at all, but you may help supplement the documentation [here](https://github.com/openplanet-nl/nadeoapi-docs).
+
+The public Trackmania API has official documentation [here](https://api.trackmania.com/doc).
 
 Installing the package from PyPI:
 ```
 python -m pip install nadeo-api
 ```
 
 Using the package:
-```
+```py
 import nadeo_api
-import nadeo_api.auth
+import nadeo_api.auth   # authentication - required for any endpoint
+import nadeo_api.core   # web services Core endpoints
+import nadeo_api.live   # web services Live endpoints
+import nadeo_api.meet   # web services Meet endpoints
+import nadeo_api.oauth  # OAuth2 endpoints (public API)
 ```
```

