# Comparing `tmp/prefect_gitlab-0.2.4.tar.gz` & `tmp/prefect_gitlab-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect_gitlab-0.2.4.tar", last modified: Fri Apr 26 15:03:59 2024, max compression
+gzip compressed data, was "prefect_gitlab-0.2.5.tar", last modified: Thu May 16 20:58:39 2024, max compression
```

## Comparing `prefect_gitlab-0.2.4.tar` & `prefect_gitlab-0.2.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:59.843779 prefect_gitlab-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-26 15:03:46.000000 prefect_gitlab-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-26 15:03:46.000000 prefect_gitlab-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-04-26 15:03:59.843779 prefect_gitlab-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-26 15:03:46.000000 prefect_gitlab-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:59.839779 prefect_gitlab-0.2.4/prefect_gitlab/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-26 15:03:46.000000 prefect_gitlab-0.2.4/prefect_gitlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-26 15:03:59.000000 prefect_gitlab-0.2.4/prefect_gitlab/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-26 15:03:46.000000 prefect_gitlab-0.2.4/prefect_gitlab/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     7759 2024-04-26 15:03:46.000000 prefect_gitlab-0.2.4/prefect_gitlab/repositories.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:59.843779 prefect_gitlab-0.2.4/prefect_gitlab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-04-26 15:03:59.000000 prefect_gitlab-0.2.4/prefect_gitlab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-26 15:03:59.000000 prefect_gitlab-0.2.4/prefect_gitlab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:03:59.000000 prefect_gitlab-0.2.4/prefect_gitlab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-26 15:03:59.000000 prefect_gitlab-0.2.4/prefect_gitlab.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-26 15:03:59.000000 prefect_gitlab-0.2.4/prefect_gitlab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-26 15:03:59.000000 prefect_gitlab-0.2.4/prefect_gitlab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-26 15:03:46.000000 prefect_gitlab-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:03:59.843779 prefect_gitlab-0.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:59.843779 prefect_gitlab-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-26 15:03:46.000000 prefect_gitlab-0.2.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-26 15:03:46.000000 prefect_gitlab-0.2.4/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    10310 2024-04-26 15:03:46.000000 prefect_gitlab-0.2.4/tests/test_repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-26 15:03:46.000000 prefect_gitlab-0.2.4/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:39.688641 prefect_gitlab-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-16 20:58:28.000000 prefect_gitlab-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-16 20:58:28.000000 prefect_gitlab-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-05-16 20:58:39.688641 prefect_gitlab-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-16 20:58:28.000000 prefect_gitlab-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:39.684641 prefect_gitlab-0.2.5/prefect_gitlab/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-16 20:58:28.000000 prefect_gitlab-0.2.5/prefect_gitlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-16 20:58:39.000000 prefect_gitlab-0.2.5/prefect_gitlab/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-05-16 20:58:28.000000 prefect_gitlab-0.2.5/prefect_gitlab/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7759 2024-05-16 20:58:28.000000 prefect_gitlab-0.2.5/prefect_gitlab/repositories.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:39.684641 prefect_gitlab-0.2.5/prefect_gitlab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-05-16 20:58:39.000000 prefect_gitlab-0.2.5/prefect_gitlab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-16 20:58:39.000000 prefect_gitlab-0.2.5/prefect_gitlab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 20:58:39.000000 prefect_gitlab-0.2.5/prefect_gitlab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-16 20:58:39.000000 prefect_gitlab-0.2.5/prefect_gitlab.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-16 20:58:39.000000 prefect_gitlab-0.2.5/prefect_gitlab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-16 20:58:39.000000 prefect_gitlab-0.2.5/prefect_gitlab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-16 20:58:28.000000 prefect_gitlab-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 20:58:39.688641 prefect_gitlab-0.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:39.684641 prefect_gitlab-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-16 20:58:28.000000 prefect_gitlab-0.2.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-16 20:58:28.000000 prefect_gitlab-0.2.5/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10310 2024-05-16 20:58:28.000000 prefect_gitlab-0.2.5/tests/test_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-16 20:58:28.000000 prefect_gitlab-0.2.5/tests/test_version.py
```

### Comparing `prefect_gitlab-0.2.4/LICENSE` & `prefect_gitlab-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect_gitlab-0.2.4/PKG-INFO` & `prefect_gitlab-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-gitlab
-Version: 0.2.4
+Version: 0.2.5
 Summary: A Prefect collection for working with GitLab repositories.
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-gitlab
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
-Requires-Dist: prefect>=2.13.5
+Requires-Dist: prefect<3.0.0,>=2.13.5
 Requires-Dist: python-gitlab>=3.12.0
 Requires-Dist: tenacity>=8.2.3
 Provides-Extra: dev
 Requires-Dist: aiohttp; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: prefect-gitlab Version: 0.2.4 Summary: A Prefect
+Metadata-Version: 2.1 Name: prefect-gitlab Version: 0.2.5 Summary: A Prefect
 collection for working with GitLab repositories. Author-email: "Prefect
 Technologies, Inc."
 prefect.io> License: Apache License 2.0 Project-URL: Homepage, https://
 github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-gitlab
 Keywords: prefect Classifier: Natural Language :: English Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Requires-Python: >=3.8 Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-prefect>=2.13.5 Requires-Dist: python-gitlab>=3.12.0 Requires-Dist:
+prefect<3.0.0,>=2.13.5 Requires-Dist: python-gitlab>=3.12.0 Requires-Dist:
 tenacity>=8.2.3 Provides-Extra: dev Requires-Dist: aiohttp; extra == "dev"
 Requires-Dist: coverage; extra == "dev" Requires-Dist: interrogate; extra ==
 "dev" Requires-Dist: mkdocs-gen-files; extra == "dev" Requires-Dist: mkdocs-
 material; extra == "dev" Requires-Dist: mkdocs; extra == "dev" Requires-Dist:
 mkdocstrings[python]; extra == "dev" Requires-Dist: mock; python_version <
 "3.8" and extra == "dev" Requires-Dist: mypy; extra == "dev" Requires-Dist:
 pillow; extra == "dev" Requires-Dist: pre-commit; extra == "dev" Requires-Dist:
```

### Comparing `prefect_gitlab-0.2.4/README.md` & `prefect_gitlab-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `prefect_gitlab-0.2.4/prefect_gitlab/credentials.py` & `prefect_gitlab-0.2.5/prefect_gitlab/credentials.py`

 * *Files identical despite different names*

### Comparing `prefect_gitlab-0.2.4/prefect_gitlab/repositories.py` & `prefect_gitlab-0.2.5/prefect_gitlab/repositories.py`

 * *Files identical despite different names*

### Comparing `prefect_gitlab-0.2.4/prefect_gitlab.egg-info/PKG-INFO` & `prefect_gitlab-0.2.5/prefect_gitlab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-gitlab
-Version: 0.2.4
+Version: 0.2.5
 Summary: A Prefect collection for working with GitLab repositories.
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-gitlab
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
-Requires-Dist: prefect>=2.13.5
+Requires-Dist: prefect<3.0.0,>=2.13.5
 Requires-Dist: python-gitlab>=3.12.0
 Requires-Dist: tenacity>=8.2.3
 Provides-Extra: dev
 Requires-Dist: aiohttp; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: prefect-gitlab Version: 0.2.4 Summary: A Prefect
+Metadata-Version: 2.1 Name: prefect-gitlab Version: 0.2.5 Summary: A Prefect
 collection for working with GitLab repositories. Author-email: "Prefect
 Technologies, Inc."
 prefect.io> License: Apache License 2.0 Project-URL: Homepage, https://
 github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-gitlab
 Keywords: prefect Classifier: Natural Language :: English Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Requires-Python: >=3.8 Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-prefect>=2.13.5 Requires-Dist: python-gitlab>=3.12.0 Requires-Dist:
+prefect<3.0.0,>=2.13.5 Requires-Dist: python-gitlab>=3.12.0 Requires-Dist:
 tenacity>=8.2.3 Provides-Extra: dev Requires-Dist: aiohttp; extra == "dev"
 Requires-Dist: coverage; extra == "dev" Requires-Dist: interrogate; extra ==
 "dev" Requires-Dist: mkdocs-gen-files; extra == "dev" Requires-Dist: mkdocs-
 material; extra == "dev" Requires-Dist: mkdocs; extra == "dev" Requires-Dist:
 mkdocstrings[python]; extra == "dev" Requires-Dist: mock; python_version <
 "3.8" and extra == "dev" Requires-Dist: mypy; extra == "dev" Requires-Dist:
 pillow; extra == "dev" Requires-Dist: pre-commit; extra == "dev" Requires-Dist:
```

### Comparing `prefect_gitlab-0.2.4/pyproject.toml` & `prefect_gitlab-0.2.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,36 +3,34 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prefect-gitlab"
 description = "A Prefect collection for working with GitLab repositories."
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
 dependencies = [
-    "prefect>=2.13.5",
-    "python-gitlab>=3.12.0",
-    "tenacity>=8.2.3",
+  "prefect>=2.13.5, < 3.0.0",
+  "python-gitlab>=3.12.0",
+  "tenacity>=8.2.3",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = [
   "aiohttp",
   "coverage",
@@ -74,8 +72,8 @@
 omit = ["tests/*", "prefect_gitlab/_version.py"]
 
 [tool.coverage.report]
 fail_under = 80
 show_missing = true
 
 [tool.pytest.ini_options]
-asyncio_mode = "auto"
+asyncio_mode = "auto"
```

### Comparing `prefect_gitlab-0.2.4/tests/test_credentials.py` & `prefect_gitlab-0.2.5/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `prefect_gitlab-0.2.4/tests/test_repositories.py` & `prefect_gitlab-0.2.5/tests/test_repositories.py`

 * *Files identical despite different names*

