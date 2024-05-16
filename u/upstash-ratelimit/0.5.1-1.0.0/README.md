# Comparing `tmp/upstash_ratelimit-0.5.1.tar.gz` & `tmp/upstash_ratelimit-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upstash_ratelimit-0.5.1.tar", max compression
+gzip compressed data, was "upstash_ratelimit-1.0.0.tar", max compression
```

## Comparing `upstash_ratelimit-0.5.1.tar` & `upstash_ratelimit-1.0.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1072 2023-07-17 10:57:03.774984 upstash_ratelimit-0.5.1/LICENSE
--rw-r--r--   0        0        0     8062 2023-07-17 10:57:03.778984 upstash_ratelimit-0.5.1/README.md
--rw-r--r--   0        0        0     1331 2023-07-17 10:57:03.778984 upstash_ratelimit-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      268 2023-07-17 10:57:03.778984 upstash_ratelimit-0.5.1/upstash_ratelimit/__init__.py
--rw-r--r--   0        0        0      253 2023-07-17 10:57:03.778984 upstash_ratelimit-0.5.1/upstash_ratelimit/asyncio/__init__.py
--rw-r--r--   0        0        0     4482 2023-07-17 10:57:03.778984 upstash_ratelimit-0.5.1/upstash_ratelimit/asyncio/ratelimit.py
--rw-r--r--   0        0        0    14777 2023-07-17 10:57:03.778984 upstash_ratelimit-0.5.1/upstash_ratelimit/limiter.py
--rw-r--r--   0        0        0        0 2023-07-17 10:57:03.778984 upstash_ratelimit-0.5.1/upstash_ratelimit/py.typed
--rw-r--r--   0        0        0     4245 2023-07-17 10:57:03.778984 upstash_ratelimit-0.5.1/upstash_ratelimit/ratelimit.py
--rw-r--r--   0        0        0      138 2023-07-17 10:57:03.778984 upstash_ratelimit-0.5.1/upstash_ratelimit/typing.py
--rw-r--r--   0        0        0     1123 2023-07-17 10:57:03.778984 upstash_ratelimit-0.5.1/upstash_ratelimit/utils.py
--rw-r--r--   0        0        0     9255 1970-01-01 00:00:00.000000 upstash_ratelimit-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-12-04 11:03:24.325189 upstash_ratelimit-1.0.0/LICENSE
+-rw-r--r--   0        0        0     8062 2023-12-04 11:03:24.325189 upstash_ratelimit-1.0.0/README.md
+-rw-r--r--   0        0        0     1389 2023-12-04 11:03:24.325189 upstash_ratelimit-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      268 2023-12-04 11:03:24.325189 upstash_ratelimit-1.0.0/upstash_ratelimit/__init__.py
+-rw-r--r--   0        0        0      253 2023-12-04 11:03:24.325189 upstash_ratelimit-1.0.0/upstash_ratelimit/asyncio/__init__.py
+-rw-r--r--   0        0        0     4482 2023-12-04 11:03:24.325189 upstash_ratelimit-1.0.0/upstash_ratelimit/asyncio/ratelimit.py
+-rw-r--r--   0        0        0    14777 2023-12-04 11:03:24.329189 upstash_ratelimit-1.0.0/upstash_ratelimit/limiter.py
+-rw-r--r--   0        0        0        0 2023-12-04 11:03:24.329189 upstash_ratelimit-1.0.0/upstash_ratelimit/py.typed
+-rw-r--r--   0        0        0     4245 2023-12-04 11:03:24.329189 upstash_ratelimit-1.0.0/upstash_ratelimit/ratelimit.py
+-rw-r--r--   0        0        0      138 2023-12-04 11:03:24.329189 upstash_ratelimit-1.0.0/upstash_ratelimit/typing.py
+-rw-r--r--   0        0        0     1123 2023-12-04 11:03:24.329189 upstash_ratelimit-1.0.0/upstash_ratelimit/utils.py
+-rw-r--r--   0        0        0     9317 1970-01-01 00:00:00.000000 upstash_ratelimit-1.0.0/PKG-INFO
```

### Comparing `upstash_ratelimit-0.5.1/LICENSE` & `upstash_ratelimit-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.5.1/README.md` & `upstash_ratelimit-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.5.1/pyproject.toml` & `upstash_ratelimit-1.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 [tool.poetry]
 name = "upstash-ratelimit"
-version = "0.5.1"
+version = "1.0.0"
 description = "Serverless ratelimiting package from Upstash"
 authors = ["Upstash <support@upstash.com>", "Zgîmbău Tudor <tudor.zgimbau@gmail.com>"]
 maintainers = ["Upstash <support@upstash.com>"]
 readme = "README.md"
 repository = "https://github.com/upstash/ratelimit-python"
 keywords = ["ratelimit", "rate limit", "Upstash rate limit", "Redis rate limit"]
 classifiers = [
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Software Development :: Libraries",
 ]
 packages = [{include = "upstash_ratelimit"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-upstash-redis = "^0.15.0"
+upstash-redis = "^1.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.0"
 pytest-asyncio = "^0.21.0"
 mypy = "^1.4.1"
 
 [build-system]
```

### Comparing `upstash_ratelimit-0.5.1/upstash_ratelimit/asyncio/ratelimit.py` & `upstash_ratelimit-1.0.0/upstash_ratelimit/asyncio/ratelimit.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.5.1/upstash_ratelimit/limiter.py` & `upstash_ratelimit-1.0.0/upstash_ratelimit/limiter.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.5.1/upstash_ratelimit/ratelimit.py` & `upstash_ratelimit-1.0.0/upstash_ratelimit/ratelimit.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.5.1/upstash_ratelimit/utils.py` & `upstash_ratelimit-1.0.0/upstash_ratelimit/utils.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.5.1/PKG-INFO` & `upstash_ratelimit-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: upstash-ratelimit
-Version: 0.5.1
+Version: 1.0.0
 Summary: Serverless ratelimiting package from Upstash
 Home-page: https://github.com/upstash/ratelimit-python
 Keywords: ratelimit,rate limit,Upstash rate limit,Redis rate limit
 Author: Upstash
 Author-email: support@upstash.com
 Maintainer: Upstash
 Maintainer-email: support@upstash.com
 Requires-Python: >=3.8,<4.0
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries
-Requires-Dist: upstash-redis (>=0.15.0,<0.16.0)
+Requires-Dist: upstash-redis (>=1.0.0,<2.0.0)
 Project-URL: Repository, https://github.com/upstash/ratelimit-python
 Description-Content-Type: text/markdown
 
 # Upstash Ratelimit Python SDK
 
 upstash-ratelimit is a connectionless rate limiting library for Python, designed to be used in serverless environments such as:
 - AWS Lambda
```

