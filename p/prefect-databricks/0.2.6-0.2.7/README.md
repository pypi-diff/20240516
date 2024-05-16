# Comparing `tmp/prefect_databricks-0.2.6.tar.gz` & `tmp/prefect_databricks-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect_databricks-0.2.6.tar", last modified: Fri May  3 16:56:44 2024, max compression
+gzip compressed data, was "prefect_databricks-0.2.7.tar", last modified: Thu May 16 20:58:31 2024, max compression
```

## Comparing `prefect_databricks-0.2.6.tar` & `prefect_databricks-0.2.7.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:56:44.963230 prefect_databricks-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-03 16:56:32.000000 prefect_databricks-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-03 16:56:32.000000 prefect_databricks-0.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7591 2024-05-03 16:56:44.963230 prefect_databricks-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-05-03 16:56:32.000000 prefect_databricks-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:56:44.959230 prefect_databricks-0.2.6/prefect_databricks/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-03 16:56:32.000000 prefect_databricks-0.2.6/prefect_databricks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-03 16:56:44.000000 prefect_databricks-0.2.6/prefect_databricks/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-03 16:56:32.000000 prefect_databricks-0.2.6/prefect_databricks/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    19110 2024-05-03 16:56:32.000000 prefect_databricks-0.2.6/prefect_databricks/flows.py
--rw-r--r--   0 runner    (1001) docker     (127)    81198 2024-05-03 16:56:32.000000 prefect_databricks-0.2.6/prefect_databricks/jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:56:44.959230 prefect_databricks-0.2.6/prefect_databricks/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:56:32.000000 prefect_databricks-0.2.6/prefect_databricks/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   168341 2024-05-03 16:56:32.000000 prefect_databricks-0.2.6/prefect_databricks/models/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-05-03 16:56:32.000000 prefect_databricks-0.2.6/prefect_databricks/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:56:44.959230 prefect_databricks-0.2.6/prefect_databricks/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)   178999 2024-05-03 16:56:32.000000 prefect_databricks-0.2.6/prefect_databricks/schemas/jobs-2.1-aws.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:56:44.959230 prefect_databricks-0.2.6/prefect_databricks/schemas/original/
--rw-r--r--   0 runner    (1001) docker     (127)   178843 2024-05-03 16:56:32.000000 prefect_databricks-0.2.6/prefect_databricks/schemas/original/jobs-2.1-aws.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:56:44.963230 prefect_databricks-0.2.6/prefect_databricks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7591 2024-05-03 16:56:44.000000 prefect_databricks-0.2.6/prefect_databricks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-03 16:56:44.000000 prefect_databricks-0.2.6/prefect_databricks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 16:56:44.000000 prefect_databricks-0.2.6/prefect_databricks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-03 16:56:44.000000 prefect_databricks-0.2.6/prefect_databricks.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-03 16:56:44.000000 prefect_databricks-0.2.6/prefect_databricks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-03 16:56:44.000000 prefect_databricks-0.2.6/prefect_databricks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-03 16:56:32.000000 prefect_databricks-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 16:56:44.963230 prefect_databricks-0.2.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:56:44.963230 prefect_databricks-0.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-03 16:56:32.000000 prefect_databricks-0.2.6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-03 16:56:32.000000 prefect_databricks-0.2.6/tests/mock_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-03 16:56:32.000000 prefect_databricks-0.2.6/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-03 16:56:32.000000 prefect_databricks-0.2.6/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    13610 2024-05-03 16:56:32.000000 prefect_databricks-0.2.6/tests/test_flows.py
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-03 16:56:32.000000 prefect_databricks-0.2.6/tests/test_generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-03 16:56:32.000000 prefect_databricks-0.2.6/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-03 16:56:32.000000 prefect_databricks-0.2.6/tests/test_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-03 16:56:32.000000 prefect_databricks-0.2.6/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:31.271456 prefect_databricks-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-16 20:58:19.000000 prefect_databricks-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-16 20:58:19.000000 prefect_databricks-0.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7598 2024-05-16 20:58:31.271456 prefect_databricks-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-05-16 20:58:19.000000 prefect_databricks-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:31.267456 prefect_databricks-0.2.7/prefect_databricks/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-16 20:58:19.000000 prefect_databricks-0.2.7/prefect_databricks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-16 20:58:30.000000 prefect_databricks-0.2.7/prefect_databricks/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-16 20:58:19.000000 prefect_databricks-0.2.7/prefect_databricks/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19110 2024-05-16 20:58:19.000000 prefect_databricks-0.2.7/prefect_databricks/flows.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81198 2024-05-16 20:58:19.000000 prefect_databricks-0.2.7/prefect_databricks/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:31.267456 prefect_databricks-0.2.7/prefect_databricks/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:19.000000 prefect_databricks-0.2.7/prefect_databricks/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   168341 2024-05-16 20:58:19.000000 prefect_databricks-0.2.7/prefect_databricks/models/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-05-16 20:58:19.000000 prefect_databricks-0.2.7/prefect_databricks/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:31.267456 prefect_databricks-0.2.7/prefect_databricks/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)   178999 2024-05-16 20:58:19.000000 prefect_databricks-0.2.7/prefect_databricks/schemas/jobs-2.1-aws.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:31.267456 prefect_databricks-0.2.7/prefect_databricks/schemas/original/
+-rw-r--r--   0 runner    (1001) docker     (127)   178843 2024-05-16 20:58:19.000000 prefect_databricks-0.2.7/prefect_databricks/schemas/original/jobs-2.1-aws.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:31.271456 prefect_databricks-0.2.7/prefect_databricks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7598 2024-05-16 20:58:30.000000 prefect_databricks-0.2.7/prefect_databricks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-16 20:58:31.000000 prefect_databricks-0.2.7/prefect_databricks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 20:58:30.000000 prefect_databricks-0.2.7/prefect_databricks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-16 20:58:30.000000 prefect_databricks-0.2.7/prefect_databricks.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-16 20:58:30.000000 prefect_databricks-0.2.7/prefect_databricks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-16 20:58:30.000000 prefect_databricks-0.2.7/prefect_databricks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-16 20:58:19.000000 prefect_databricks-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 20:58:31.271456 prefect_databricks-0.2.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:31.271456 prefect_databricks-0.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-16 20:58:19.000000 prefect_databricks-0.2.7/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-16 20:58:19.000000 prefect_databricks-0.2.7/tests/mock_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-16 20:58:19.000000 prefect_databricks-0.2.7/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-16 20:58:19.000000 prefect_databricks-0.2.7/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13610 2024-05-16 20:58:19.000000 prefect_databricks-0.2.7/tests/test_flows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-16 20:58:19.000000 prefect_databricks-0.2.7/tests/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-16 20:58:19.000000 prefect_databricks-0.2.7/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-16 20:58:19.000000 prefect_databricks-0.2.7/tests/test_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-16 20:58:19.000000 prefect_databricks-0.2.7/tests/test_version.py
```

### Comparing `prefect_databricks-0.2.6/LICENSE` & `prefect_databricks-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.6/PKG-INFO` & `prefect_databricks-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-databricks
-Version: 0.2.6
+Version: 0.2.7
 Summary: Prefect integrations with Databricks
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-databricks
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: prefect>=2.14.10
+Requires-Dist: prefect<3.0.0,>=2.14.10
 Provides-Extra: dev
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
```

### Comparing `prefect_databricks-0.2.6/README.md` & `prefect_databricks-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.6/prefect_databricks/credentials.py` & `prefect_databricks-0.2.7/prefect_databricks/credentials.py`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.6/prefect_databricks/flows.py` & `prefect_databricks-0.2.7/prefect_databricks/flows.py`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.6/prefect_databricks/jobs.py` & `prefect_databricks-0.2.7/prefect_databricks/jobs.py`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.6/prefect_databricks/models/jobs.py` & `prefect_databricks-0.2.7/prefect_databricks/models/jobs.py`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.6/prefect_databricks/rest.py` & `prefect_databricks-0.2.7/prefect_databricks/rest.py`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.6/prefect_databricks/schemas/jobs-2.1-aws.yaml` & `prefect_databricks-0.2.7/prefect_databricks/schemas/jobs-2.1-aws.yaml`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.6/prefect_databricks/schemas/original/jobs-2.1-aws.yaml` & `prefect_databricks-0.2.7/prefect_databricks/schemas/original/jobs-2.1-aws.yaml`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.6/prefect_databricks.egg-info/PKG-INFO` & `prefect_databricks-0.2.7/prefect_databricks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-databricks
-Version: 0.2.6
+Version: 0.2.7
 Summary: Prefect integrations with Databricks
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-databricks
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: prefect>=2.14.10
+Requires-Dist: prefect<3.0.0,>=2.14.10
 Provides-Extra: dev
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
```

### Comparing `prefect_databricks-0.2.6/prefect_databricks.egg-info/SOURCES.txt` & `prefect_databricks-0.2.7/prefect_databricks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.6/pyproject.toml` & `prefect_databricks-0.2.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,35 +3,31 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prefect-databricks"
 description = "Prefect integrations with Databricks"
 readme = "README.md"
 requires-python = ">=3.8"
-license = {text = "Apache License 2.0"}
+license = { text = "Apache License 2.0" }
 keywords = ["prefect"]
-authors = [
-  {name = "Prefect Technologies, Inc.", email = "help@prefect.io"}
-]
+authors = [{ name = "Prefect Technologies, Inc.", email = "help@prefect.io" }]
 classifiers = [
   "Natural Language :: English",
   "Intended Audience :: Developers",
   "Intended Audience :: System Administrators",
   "License :: OSI Approved :: Apache Software License",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Topic :: Software Development :: Libraries",
 ]
-dependencies = [
-  "prefect>=2.14.10",
-]
+dependencies = ["prefect>=2.14.10, < 3.0.0"]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = [
   "coverage",
   "interrogate",
   "mkdocs-gen-files",
@@ -72,8 +68,8 @@
 omit = ["tests/*", "prefect_databricks/_version.py"]
 
 [tool.coverage.report]
 fail_under = 80
 show_missing = true
 
 [tool.pytest.ini_options]
-asyncio_mode = "auto"
+asyncio_mode = "auto"
```

### Comparing `prefect_databricks-0.2.6/tests/mock_schema.yaml` & `prefect_databricks-0.2.7/tests/mock_schema.yaml`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.6/tests/test_block_standards.py` & `prefect_databricks-0.2.7/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.6/tests/test_flows.py` & `prefect_databricks-0.2.7/tests/test_flows.py`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.6/tests/test_generate.py` & `prefect_databricks-0.2.7/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.6/tests/test_jobs.py` & `prefect_databricks-0.2.7/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.6/tests/test_rest.py` & `prefect_databricks-0.2.7/tests/test_rest.py`

 * *Files identical despite different names*

