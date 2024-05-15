# Comparing `tmp/aipkgs_requests-0.1.4.tar.gz` & `tmp/aipkgs_requests-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aipkgs_requests-0.1.4.tar", max compression
+gzip compressed data, was "aipkgs_requests-1.0.1.tar", max compression
```

## Comparing `aipkgs_requests-0.1.4.tar` & `aipkgs_requests-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1058 2022-01-01 19:20:43.000000 aipkgs_requests-0.1.4/LICENSE.md
--rw-r--r--   0        0        0       13 2022-03-08 09:21:31.816882 aipkgs_requests-0.1.4/README.rst
--rw-r--r--   0        0        0      109 2022-03-08 12:59:23.046426 aipkgs_requests-0.1.4/aipkgs_requests/__init__.py
--rw-r--r--   0        0        0     1492 2022-09-03 17:57:35.173266 aipkgs_requests-0.1.4/aipkgs_requests/helpers.py
--rw-r--r--   0        0        0     1992 2022-09-03 17:57:35.176462 aipkgs_requests-0.1.4/aipkgs_requests/helpers_session.py
--rw-r--r--   0        0        0     2156 2023-10-28 13:29:46.880191 aipkgs_requests-0.1.4/aipkgs_requests/status.py
--rw-r--r--   0        0        0      512 2024-05-08 14:34:17.680032 aipkgs_requests-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 aipkgs_requests-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1058 2022-01-01 19:20:43.000000 aipkgs_requests-1.0.1/LICENSE.md
+-rw-r--r--   0        0        0       13 2022-03-08 09:21:31.816882 aipkgs_requests-1.0.1/README.rst
+-rw-r--r--   0        0        0      109 2022-03-08 12:59:23.046426 aipkgs_requests-1.0.1/aipkgs_requests/__init__.py
+-rw-r--r--   0        0        0     1492 2022-09-03 17:57:35.173266 aipkgs_requests-1.0.1/aipkgs_requests/helpers.py
+-rw-r--r--   0        0        0     1992 2022-09-03 17:57:35.176462 aipkgs_requests-1.0.1/aipkgs_requests/helpers_session.py
+-rw-r--r--   0        0        0     2156 2023-10-28 13:29:46.880191 aipkgs_requests-1.0.1/aipkgs_requests/status.py
+-rw-r--r--   0        0        0      534 2024-05-15 22:12:33.986624 aipkgs_requests-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      553 1970-01-01 00:00:00.000000 aipkgs_requests-1.0.1/PKG-INFO
```

### Comparing `aipkgs_requests-0.1.4/LICENSE.md` & `aipkgs_requests-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aipkgs_requests-0.1.4/aipkgs_requests/helpers.py` & `aipkgs_requests-1.0.1/aipkgs_requests/helpers.py`

 * *Files identical despite different names*

### Comparing `aipkgs_requests-0.1.4/aipkgs_requests/helpers_session.py` & `aipkgs_requests-1.0.1/aipkgs_requests/helpers_session.py`

 * *Files identical despite different names*

### Comparing `aipkgs_requests-0.1.4/aipkgs_requests/status.py` & `aipkgs_requests-1.0.1/aipkgs_requests/status.py`

 * *Files identical despite different names*

### Comparing `aipkgs_requests-0.1.4/PKG-INFO` & `aipkgs_requests-1.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: aipkgs-requests
-Version: 0.1.4
-Summary: 
+Version: 1.0.1
+Summary: A package for requests
 Home-page: https://gitlab.com/aipy/packages.git
 License: MIT
 Keywords: ai
 Author: Alexy
 Author-email: alexy.ib@outlook.com
-Requires-Python: >=3.11.3,<4.0.0
+Requires-Python: >=3.11.4,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Repository, https://gitlab.com/aipy/packages.git
 Description-Content-Type: text/x-rst
```

