# Comparing `tmp/sipmessage-0.1.0.tar.gz` & `tmp/sipmessage-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sipmessage-0.1.0.tar", last modified: Thu May 16 10:22:02 2024, max compression
+gzip compressed data, was "sipmessage-0.1.1.tar", last modified: Thu May 16 13:40:00 2024, max compression
```

## Comparing `sipmessage-0.1.0.tar` & `sipmessage-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,29 @@
-drwxr-xr-x   0 sharky    (1000) sharky    (1000)        0 2024-05-16 10:22:02.871898 sipmessage-0.1.0/
--rw-r--r--   0 sharky    (1000) sharky    (1000)     1295 2024-04-25 06:45:36.000000 sipmessage-0.1.0/LICENSE
--rw-r--r--   0 sharky    (1000) sharky    (1000)      125 2024-05-16 10:19:32.000000 sipmessage-0.1.0/MANIFEST.in
--rw-r--r--   0 sharky    (1000) sharky    (1000)     1720 2024-05-16 10:19:32.000000 sipmessage-0.1.0/Makefile
--rw-r--r--   0 sharky    (1000) sharky    (1000)     1238 2024-05-16 10:22:02.871898 sipmessage-0.1.0/PKG-INFO
--rw-r--r--   0 sharky    (1000) sharky    (1000)      136 2024-04-19 06:42:47.000000 sipmessage-0.1.0/README.rst
--rw-r--r--   0 sharky    (1000) sharky    (1000)     1697 2024-05-16 10:21:38.000000 sipmessage-0.1.0/pyproject.toml
--rw-r--r--   0 sharky    (1000) sharky    (1000)       38 2024-05-16 10:22:02.871898 sipmessage-0.1.0/setup.cfg
--rw-r--r--   0 sharky    (1000) sharky    (1000)       38 2024-04-25 06:45:36.000000 sipmessage-0.1.0/setup.py
-drwxr-xr-x   0 sharky    (1000) sharky    (1000)        0 2024-05-16 10:22:02.867898 sipmessage-0.1.0/src/
-drwxr-xr-x   0 sharky    (1000) sharky    (1000)        0 2024-05-16 10:22:02.871898 sipmessage-0.1.0/src/sipmessage/
--rw-r--r--   0 sharky    (1000) sharky    (1000)      161 2024-05-16 10:19:32.000000 sipmessage-0.1.0/src/sipmessage/__init__.py
--rw-r--r--   0 sharky    (1000) sharky    (1000)      551 2024-05-16 10:19:32.000000 sipmessage-0.1.0/src/sipmessage/parameters.py
--rw-r--r--   0 sharky    (1000) sharky    (1000)     2275 2024-05-16 10:19:32.000000 sipmessage-0.1.0/src/sipmessage/uri.py
-drwxr-xr-x   0 sharky    (1000) sharky    (1000)        0 2024-05-16 10:22:02.871898 sipmessage-0.1.0/src/sipmessage.egg-info/
--rw-r--r--   0 sharky    (1000) sharky    (1000)     1238 2024-05-16 10:22:02.000000 sipmessage-0.1.0/src/sipmessage.egg-info/PKG-INFO
--rw-r--r--   0 sharky    (1000) sharky    (1000)      416 2024-05-16 10:22:02.000000 sipmessage-0.1.0/src/sipmessage.egg-info/SOURCES.txt
--rw-r--r--   0 sharky    (1000) sharky    (1000)        1 2024-05-16 10:22:02.000000 sipmessage-0.1.0/src/sipmessage.egg-info/dependency_links.txt
--rw-r--r--   0 sharky    (1000) sharky    (1000)       48 2024-05-16 10:22:02.000000 sipmessage-0.1.0/src/sipmessage.egg-info/requires.txt
--rw-r--r--   0 sharky    (1000) sharky    (1000)       11 2024-05-16 10:22:02.000000 sipmessage-0.1.0/src/sipmessage.egg-info/top_level.txt
-drwxr-xr-x   0 sharky    (1000) sharky    (1000)        0 2024-05-16 10:22:02.871898 sipmessage-0.1.0/tests/
--rw-r--r--   0 sharky    (1000) sharky    (1000)        0 2024-05-16 10:19:32.000000 sipmessage-0.1.0/tests/__init__.py
--rw-r--r--   0 sharky    (1000) sharky    (1000)      556 2024-05-16 10:19:32.000000 sipmessage-0.1.0/tests/test_parameters.py
--rw-r--r--   0 sharky    (1000) sharky    (1000)      190 2024-05-16 10:19:32.000000 sipmessage-0.1.0/tests/test_public_api.py
--rw-r--r--   0 sharky    (1000) sharky    (1000)     3205 2024-05-16 10:19:32.000000 sipmessage-0.1.0/tests/test_uri.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:40:00.894530 sipmessage-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-16 13:39:57.000000 sipmessage-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-16 13:39:57.000000 sipmessage-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-16 13:39:57.000000 sipmessage-0.1.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-16 13:40:00.894530 sipmessage-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-16 13:39:57.000000 sipmessage-0.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:40:00.890530 sipmessage-0.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-16 13:39:57.000000 sipmessage-0.1.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-16 13:39:57.000000 sipmessage-0.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-16 13:39:57.000000 sipmessage-0.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-16 13:39:57.000000 sipmessage-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 13:40:00.894530 sipmessage-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 13:39:57.000000 sipmessage-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:40:00.886530 sipmessage-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:40:00.890530 sipmessage-0.1.1/src/sipmessage/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-16 13:39:57.000000 sipmessage-0.1.1/src/sipmessage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-16 13:39:57.000000 sipmessage-0.1.1/src/sipmessage/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-16 13:39:57.000000 sipmessage-0.1.1/src/sipmessage/uri.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:40:00.890530 sipmessage-0.1.1/src/sipmessage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-16 13:40:00.000000 sipmessage-0.1.1/src/sipmessage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-16 13:40:00.000000 sipmessage-0.1.1/src/sipmessage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 13:40:00.000000 sipmessage-0.1.1/src/sipmessage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-16 13:40:00.000000 sipmessage-0.1.1/src/sipmessage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-16 13:40:00.000000 sipmessage-0.1.1/src/sipmessage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:40:00.890530 sipmessage-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 13:39:57.000000 sipmessage-0.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-16 13:39:57.000000 sipmessage-0.1.1/tests/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-16 13:39:57.000000 sipmessage-0.1.1/tests/test_public_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-16 13:39:57.000000 sipmessage-0.1.1/tests/test_uri.py
```

### Comparing `sipmessage-0.1.0/LICENSE` & `sipmessage-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sipmessage-0.1.0/Makefile` & `sipmessage-0.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `sipmessage-0.1.0/PKG-INFO` & `sipmessage-0.1.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sipmessage
-Version: 0.1.0
+Version: 0.1.1
 Summary: Pure python parsing of SIP messages and headers
 Author-email: Spacinov Engineering <opensource@spacinov.com>
 License: BSD License
 Project-URL: Homepage, https://sipmessage.readthedocs.io/
 Project-URL: Documentation, https://sipmessage.readthedocs.io/
 Project-URL: Repository, https://github.com/spacinov/sipmessage
 Project-URL: Issues, https://github.com/spacinov/sipmessage/issues
@@ -18,16 +18,21 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Communications :: Telephony
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
-Provides-Extra: dev
 License-File: LICENSE
+Provides-Extra: dev
+Requires-Dist: check-manifest; extra == "dev"
+Requires-Dist: coverage; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: pyroma; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
 
 ==========
 sipmessage
 ==========
 
 
 The ``sipmessage`` project provides a set of Python helpers and structures
```

### Comparing `sipmessage-0.1.0/pyproject.toml` & `sipmessage-0.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 # Version
 name = "sipmessage"
-version = "0.1.0"
+version = "0.1.1"
 
 # Dependencies
 dependencies = []
 requires-python = ">= 3.10"
 
 # Development
 authors = [
```

### Comparing `sipmessage-0.1.0/src/sipmessage/uri.py` & `sipmessage-0.1.1/src/sipmessage/uri.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,23 +7,41 @@
 import urllib.parse
 
 from .parameters import Parameters
 
 
 @dataclasses.dataclass
 class URI:
+    """
+    A SIP or SIPS URL as described by RFC3261.
+    """
+
     scheme: str
+    "The URL scheme specifier."
+
     host: str
+    "The host providing the SIP resource."
+
     user: str | None = None
+    "The identifier of a particular resource at the host being addressed."
+
     password: str | None = None
+    "A password associated with the user."
+
     port: int | None = None
+    "The port number where the request is to be sent."
+
     parameters: Parameters = dataclasses.field(default_factory=Parameters)
+    "Parameters affecting a request constructed from the URI."
 
     @classmethod
     def parse(cls, value: str) -> "URI":
+        """
+        Parse the given string into a :class:`URI` instance.
+        """
         parsed = urllib.parse.urlparse(value)
         if "@" in parsed.path:
             user_password, host_port = parsed.path.split("@")
             if ":" in user_password:
                 user, password = user_password.split(":")
             else:
                 user = user_password
```

### Comparing `sipmessage-0.1.0/src/sipmessage.egg-info/PKG-INFO` & `sipmessage-0.1.1/src/sipmessage.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sipmessage
-Version: 0.1.0
+Version: 0.1.1
 Summary: Pure python parsing of SIP messages and headers
 Author-email: Spacinov Engineering <opensource@spacinov.com>
 License: BSD License
 Project-URL: Homepage, https://sipmessage.readthedocs.io/
 Project-URL: Documentation, https://sipmessage.readthedocs.io/
 Project-URL: Repository, https://github.com/spacinov/sipmessage
 Project-URL: Issues, https://github.com/spacinov/sipmessage/issues
@@ -18,16 +18,21 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Communications :: Telephony
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
-Provides-Extra: dev
 License-File: LICENSE
+Provides-Extra: dev
+Requires-Dist: check-manifest; extra == "dev"
+Requires-Dist: coverage; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: pyroma; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
 
 ==========
 sipmessage
 ==========
 
 
 The ``sipmessage`` project provides a set of Python helpers and structures
```

### Comparing `sipmessage-0.1.0/tests/test_parameters.py` & `sipmessage-0.1.1/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `sipmessage-0.1.0/tests/test_uri.py` & `sipmessage-0.1.1/tests/test_uri.py`

 * *Files identical despite different names*

