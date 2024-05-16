# Comparing `tmp/bkstorages-1.1.0.tar.gz` & `tmp/bkstorages-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bkstorages-1.1.0.tar", max compression
+gzip compressed data, was "bkstorages-1.1.1.tar", max compression
```

## Comparing `bkstorages-1.1.0.tar` & `bkstorages-1.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      782 2023-08-08 10:34:10.480000 bkstorages-1.1.0/bkstorages/__init__.py
--rw-r--r--   0        0        0      760 2023-08-08 10:34:10.480000 bkstorages-1.1.0/bkstorages/backends/__init__.py
--rw-r--r--   0        0        0    18027 2023-08-08 10:34:10.480000 bkstorages-1.1.0/bkstorages/backends/bkrepo.py
--rw-r--r--   0        0        0    25222 2023-08-08 10:34:10.480000 bkstorages-1.1.0/bkstorages/backends/rgw.py
--rw-r--r--   0        0        0     1859 2023-08-08 10:34:10.480000 bkstorages-1.1.0/bkstorages/exceptions.py
--rw-r--r--   0        0        0     5413 2023-08-08 10:34:10.480000 bkstorages-1.1.0/bkstorages/utils.py
--rw-r--r--   0        0        0     1521 2023-08-08 10:34:10.480000 bkstorages-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      696 2023-08-08 11:04:10.890000 bkstorages-1.1.0/setup.py
--rw-r--r--   0        0        0      633 2023-08-08 11:04:10.890000 bkstorages-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     6075 2023-12-28 08:29:17.324152 bkstorages-1.1.1/README.md
+-rw-r--r--   0        0        0      782 2024-05-16 02:50:27.535389 bkstorages-1.1.1/bkstorages/__init__.py
+-rw-r--r--   0        0        0      760 2023-12-28 08:29:17.324851 bkstorages-1.1.1/bkstorages/backends/__init__.py
+-rw-r--r--   0        0        0    18027 2023-12-28 08:29:17.325154 bkstorages-1.1.1/bkstorages/backends/bkrepo.py
+-rw-r--r--   0        0        0    25222 2023-12-28 08:29:17.325462 bkstorages-1.1.1/bkstorages/backends/rgw.py
+-rw-r--r--   0        0        0     1859 2023-12-28 08:29:17.325821 bkstorages-1.1.1/bkstorages/exceptions.py
+-rw-r--r--   0        0        0     5413 2023-12-28 08:29:17.326288 bkstorages-1.1.1/bkstorages/utils.py
+-rw-r--r--   0        0        0     1811 2024-05-16 02:50:27.536097 bkstorages-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6822 1970-01-01 00:00:00.000000 bkstorages-1.1.1/PKG-INFO
```

### Comparing `bkstorages-1.1.0/bkstorages/__init__.py` & `bkstorages-1.1.1/bkstorages/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,8 +4,8 @@
  * Copyright (C) 2017-2021 THL A29 Limited, a Tencent company. All rights reserved.
  * Licensed under the MIT License (the "License"); you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at http://opensource.org/licenses/MIT
  * Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
  * an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
  * specific language governing permissions and limitations under the License.
 """
-__version__ = "1.1.0"
+__version__ = "1.1.1"
```

### Comparing `bkstorages-1.1.0/bkstorages/backends/__init__.py` & `bkstorages-1.1.1/bkstorages/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `bkstorages-1.1.0/bkstorages/backends/bkrepo.py` & `bkstorages-1.1.1/bkstorages/backends/bkrepo.py`

 * *Files identical despite different names*

### Comparing `bkstorages-1.1.0/bkstorages/backends/rgw.py` & `bkstorages-1.1.1/bkstorages/backends/rgw.py`

 * *Files identical despite different names*

### Comparing `bkstorages-1.1.0/bkstorages/exceptions.py` & `bkstorages-1.1.1/bkstorages/exceptions.py`

 * *Files identical despite different names*

### Comparing `bkstorages-1.1.0/bkstorages/utils.py` & `bkstorages-1.1.1/bkstorages/utils.py`

 * *Files identical despite different names*

### Comparing `bkstorages-1.1.0/pyproject.toml` & `bkstorages-1.1.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,30 @@
 [tool.poetry]
 name = "bkstorages"
-version = "1.1.0"
+version = "1.1.1"
 description = "File storage backends for blueking PaaS platform"
-classifiers = ["Programming Language :: Python", "Programming Language :: Python :: 3", "Framework :: Django"]
+readme = "README.md"
 authors = ["blueking <blueking@tencent.com>"]
+license = "MIT"
+classifiers = [
+  "Programming Language :: Python :: 3",
+  "License :: OSI Approved :: MIT License",
+  "Framework :: Django",
+]
+
+[project.urls]
+Homepage = "https://github.com/TencentBlueKing/bkpaas-python-sdk/"
+Repository = "https://github.com/TencentBlueKing/bkpaas-python-sdk/"
+
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dependencies]
-python = ">=3.6.2,<3.11"
+python = ">=3.6.2,<3.12"
 boto3 = ">=1.4.1"
 six = "*"
 requests = "*"
 curlify = "^2.2.1"
 
 [tool.poetry.dev-dependencies]
 django = ">=1.7,<3.0.0"
@@ -20,25 +34,25 @@
 pyproject-flake8 = "^0.0.1-alpha.2"
 flake8-comprehensions = "^3.5.0"
 # pytest
 pytest = "6.2.5"
 pytest-django = "4.1.0"
 requests-mock = "^1.8.0"
 # black
-black = "21.7b0"
+black = "*"
 # mypy
-mypy = "0.910"
+mypy = "*"
 # install extension stubs if missing
 types-requests = "2.25.0"
 types-setuptools = "57.0.0"
 types-six = "0.1.7"
 types-toml = "0.1.3"
 # isort
 isort = "^5.9.2"
-moto = {extras = ["s3"], version = "^3.1.3"}
+moto = { extras = ["s3"], version = "^3.1.3" }
 
 [tool.black]
 line-length = 119
 skip-string-normalization = 'true'
 exclude = '''
 /(
   | .+/dist/.*
@@ -56,15 +70,15 @@
 
 [tool.flake8]
 ignore = "C901,E203,W503"
 max-line-length = 119
 max-complexity = 12
 format = "pylint"
 # ignore example
- exclude = "*.pyc,.git,__pycache__,*/dist/*"
+exclude = "*.pyc,.git,__pycache__,*/dist/*"
 
 [tool.mypy]
 ignore_missing_imports = true
 show_error_codes = true
 strict_optional = false
 pretty = true
```

