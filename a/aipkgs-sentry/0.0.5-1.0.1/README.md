# Comparing `tmp/aipkgs_sentry-0.0.5.tar.gz` & `tmp/aipkgs_sentry-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aipkgs_sentry-0.0.5.tar", max compression
+gzip compressed data, was "aipkgs_sentry-1.0.1.tar", max compression
```

## Comparing `aipkgs_sentry-0.0.5.tar` & `aipkgs_sentry-1.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1058 2022-03-08 13:06:48.932779 aipkgs_sentry-0.0.5/LICENSE.md
--rw-r--r--   0        0        0       13 2022-03-08 13:06:48.933040 aipkgs_sentry-0.0.5/README.rst
--rw-r--r--   0        0        0       42 2022-09-03 17:57:35.167810 aipkgs_sentry-0.0.5/aipkgs_sentry/__init__.py
--rw-r--r--   0        0        0      870 2022-09-03 17:58:25.064464 aipkgs_sentry-0.0.5/aipkgs_sentry/helpers.py
--rw-r--r--   0        0        0      606 2024-05-09 12:12:17.511184 aipkgs_sentry-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      621 1970-01-01 00:00:00.000000 aipkgs_sentry-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1058 2022-03-08 13:06:48.932779 aipkgs_sentry-1.0.1/LICENSE.md
+-rw-r--r--   0        0        0       13 2022-03-08 13:06:48.933040 aipkgs_sentry-1.0.1/README.rst
+-rw-r--r--   0        0        0       42 2022-09-03 17:57:35.167810 aipkgs_sentry-1.0.1/aipkgs_sentry/__init__.py
+-rw-r--r--   0        0        0      870 2022-09-03 17:58:25.064464 aipkgs_sentry-1.0.1/aipkgs_sentry/helpers.py
+-rw-r--r--   0        0        0      606 2024-05-15 22:15:48.795059 aipkgs_sentry-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      621 1970-01-01 00:00:00.000000 aipkgs_sentry-1.0.1/PKG-INFO
```

### Comparing `aipkgs_sentry-0.0.5/LICENSE.md` & `aipkgs_sentry-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aipkgs_sentry-0.0.5/aipkgs_sentry/helpers.py` & `aipkgs_sentry-1.0.1/aipkgs_sentry/helpers.py`

 * *Files identical despite different names*

### Comparing `aipkgs_sentry-0.0.5/pyproject.toml` & `aipkgs_sentry-1.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core>=1.0.1"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "aipkgs-sentry"
-version = "0.0.5"
+version = "1.0.1"
 description = "Sentry integration for aipy packages"
 authors = ["Alexy <alexy.ib@outlook.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://gitlab.com/aipy/public/packages.git"
 repository = "https://gitlab.com/aipy/public/packages.git"
 keywords = ["ai"]
 include = [
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.11.3"
+python = "^3.11.4"
 sentry-sdk = "^2.1.1"
 
 [tool.poetry.extras]
 flask = ["sentry-sdk"]
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
```

### Comparing `aipkgs_sentry-0.0.5/PKG-INFO` & `aipkgs_sentry-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: aipkgs-sentry
-Version: 0.0.5
+Version: 1.0.1
 Summary: Sentry integration for aipy packages
 Home-page: https://gitlab.com/aipy/public/packages.git
 License: MIT
 Keywords: ai
 Author: Alexy
 Author-email: alexy.ib@outlook.com
-Requires-Python: >=3.11.3,<4.0.0
+Requires-Python: >=3.11.4,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: flask
 Requires-Dist: sentry-sdk (>=2.1.1,<3.0.0) ; extra == "flask"
 Project-URL: Repository, https://gitlab.com/aipy/public/packages.git
 Description-Content-Type: text/x-rst
```

