# Comparing `tmp/prefect_bitbucket-0.2.3.tar.gz` & `tmp/prefect_bitbucket-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect_bitbucket-0.2.3.tar", last modified: Thu Apr 25 19:20:30 2024, max compression
+gzip compressed data, was "prefect_bitbucket-0.2.4.tar", last modified: Fri Apr 26 15:04:00 2024, max compression
```

## Comparing `prefect_bitbucket-0.2.3.tar` & `prefect_bitbucket-0.2.4.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:30.371102 prefect_bitbucket-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     6643 2024-04-25 19:20:30.371102 prefect_bitbucket-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-04-25 19:20:16.000000 prefect_bitbucket-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:30.367102 prefect_bitbucket-0.2.3/prefect_bitbucket/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-25 19:20:16.000000 prefect_bitbucket-0.2.3/prefect_bitbucket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 19:20:29.000000 prefect_bitbucket-0.2.3/prefect_bitbucket/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-25 19:20:16.000000 prefect_bitbucket-0.2.3/prefect_bitbucket/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     7332 2024-04-25 19:20:16.000000 prefect_bitbucket-0.2.3/prefect_bitbucket/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:30.367102 prefect_bitbucket-0.2.3/prefect_bitbucket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6643 2024-04-25 19:20:30.000000 prefect_bitbucket-0.2.3/prefect_bitbucket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-25 19:20:30.000000 prefect_bitbucket-0.2.3/prefect_bitbucket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:20:30.000000 prefect_bitbucket-0.2.3/prefect_bitbucket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-25 19:20:30.000000 prefect_bitbucket-0.2.3/prefect_bitbucket.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-25 19:20:30.000000 prefect_bitbucket-0.2.3/prefect_bitbucket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-25 19:20:30.000000 prefect_bitbucket-0.2.3/prefect_bitbucket.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-25 19:20:16.000000 prefect_bitbucket-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 19:20:30.371102 prefect_bitbucket-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:30.367102 prefect_bitbucket-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-25 19:20:16.000000 prefect_bitbucket-0.2.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-25 19:20:16.000000 prefect_bitbucket-0.2.3/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     9989 2024-04-25 19:20:16.000000 prefect_bitbucket-0.2.3/tests/test_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-25 19:20:16.000000 prefect_bitbucket-0.2.3/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:00.011325 prefect_bitbucket-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-26 15:03:47.000000 prefect_bitbucket-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-26 15:03:47.000000 prefect_bitbucket-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-04-26 15:04:00.011325 prefect_bitbucket-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-04-26 15:03:47.000000 prefect_bitbucket-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:00.007325 prefect_bitbucket-0.2.4/prefect_bitbucket/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-26 15:03:47.000000 prefect_bitbucket-0.2.4/prefect_bitbucket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-26 15:03:59.000000 prefect_bitbucket-0.2.4/prefect_bitbucket/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-26 15:03:47.000000 prefect_bitbucket-0.2.4/prefect_bitbucket/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7332 2024-04-26 15:03:47.000000 prefect_bitbucket-0.2.4/prefect_bitbucket/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:00.011325 prefect_bitbucket-0.2.4/prefect_bitbucket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-04-26 15:03:59.000000 prefect_bitbucket-0.2.4/prefect_bitbucket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-26 15:04:00.000000 prefect_bitbucket-0.2.4/prefect_bitbucket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:03:59.000000 prefect_bitbucket-0.2.4/prefect_bitbucket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-26 15:03:59.000000 prefect_bitbucket-0.2.4/prefect_bitbucket.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-26 15:03:59.000000 prefect_bitbucket-0.2.4/prefect_bitbucket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-26 15:03:59.000000 prefect_bitbucket-0.2.4/prefect_bitbucket.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-26 15:03:47.000000 prefect_bitbucket-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:04:00.011325 prefect_bitbucket-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:00.007325 prefect_bitbucket-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-26 15:03:47.000000 prefect_bitbucket-0.2.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-26 15:03:47.000000 prefect_bitbucket-0.2.4/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9989 2024-04-26 15:03:47.000000 prefect_bitbucket-0.2.4/tests/test_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-26 15:03:47.000000 prefect_bitbucket-0.2.4/tests/test_version.py
```

### Comparing `prefect_bitbucket-0.2.3/PKG-INFO` & `prefect_bitbucket-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-bitbucket
-Version: 0.2.3
+Version: 0.2.4
 Summary: Prefect integrations for working with Bitbucket repositories.
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-bitbucket
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: prefect>=2.14.10
 Requires-Dist: atlassian-python-api!=3.41.5,!=3.41.6,!=3.41.7,!=3.41.8,>=3.32.1
 Provides-Extra: dev
 Requires-Dist: aiohttp; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
```

### Comparing `prefect_bitbucket-0.2.3/README.md` & `prefect_bitbucket-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `prefect_bitbucket-0.2.3/prefect_bitbucket/credentials.py` & `prefect_bitbucket-0.2.4/prefect_bitbucket/credentials.py`

 * *Files identical despite different names*

### Comparing `prefect_bitbucket-0.2.3/prefect_bitbucket/repository.py` & `prefect_bitbucket-0.2.4/prefect_bitbucket/repository.py`

 * *Files identical despite different names*

### Comparing `prefect_bitbucket-0.2.3/prefect_bitbucket.egg-info/PKG-INFO` & `prefect_bitbucket-0.2.4/prefect_bitbucket.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-bitbucket
-Version: 0.2.3
+Version: 0.2.4
 Summary: Prefect integrations for working with Bitbucket repositories.
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-bitbucket
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: prefect>=2.14.10
 Requires-Dist: atlassian-python-api!=3.41.5,!=3.41.6,!=3.41.7,!=3.41.8,>=3.32.1
 Provides-Extra: dev
 Requires-Dist: aiohttp; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
```

### Comparing `prefect_bitbucket-0.2.3/pyproject.toml` & `prefect_bitbucket-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `prefect_bitbucket-0.2.3/tests/test_credentials.py` & `prefect_bitbucket-0.2.4/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `prefect_bitbucket-0.2.3/tests/test_repository.py` & `prefect_bitbucket-0.2.4/tests/test_repository.py`

 * *Files identical despite different names*

