# Comparing `tmp/prefect_github-0.2.4.tar.gz` & `tmp/prefect_github-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect_github-0.2.4.tar", last modified: Fri Apr 26 15:04:08 2024, max compression
+gzip compressed data, was "prefect_github-0.2.5.tar", last modified: Thu May 16 20:58:38 2024, max compression
```

## Comparing `prefect_github-0.2.4.tar` & `prefect_github-0.2.5.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:08.389030 prefect_github-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-26 15:03:47.000000 prefect_github-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-26 15:03:47.000000 prefect_github-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-04-26 15:04:08.389030 prefect_github-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-04-26 15:03:47.000000 prefect_github-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:08.373031 prefect_github-0.2.4/prefect_github/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-26 15:03:47.000000 prefect_github-0.2.4/prefect_github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-26 15:04:07.000000 prefect_github-0.2.4/prefect_github/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:08.369030 prefect_github-0.2.4/prefect_github/configs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:08.377030 prefect_github-0.2.4/prefect_github/configs/mutation/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-26 15:03:47.000000 prefect_github-0.2.4/prefect_github/configs/mutation/add_comment.json
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-26 15:03:47.000000 prefect_github-0.2.4/prefect_github/configs/mutation/add_pull_request_review.json
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-26 15:03:47.000000 prefect_github-0.2.4/prefect_github/configs/mutation/add_reaction.json
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-26 15:03:47.000000 prefect_github-0.2.4/prefect_github/configs/mutation/add_star.json
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-26 15:03:47.000000 prefect_github-0.2.4/prefect_github/configs/mutation/close_issue.json
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-26 15:03:47.000000 prefect_github-0.2.4/prefect_github/configs/mutation/close_pull_request.json
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-26 15:03:47.000000 prefect_github-0.2.4/prefect_github/configs/mutation/create_issue.json
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-26 15:03:47.000000 prefect_github-0.2.4/prefect_github/configs/mutation/create_pull_request.json
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-26 15:03:47.000000 prefect_github-0.2.4/prefect_github/configs/mutation/remove_reaction.json
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-26 15:03:47.000000 prefect_github-0.2.4/prefect_github/configs/mutation/remove_star.json
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-26 15:03:47.000000 prefect_github-0.2.4/prefect_github/configs/mutation/request_reviews.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:08.377030 prefect_github-0.2.4/prefect_github/configs/query/
--rw-r--r--   0 runner    (1001) docker     (127)     7626 2024-04-26 15:03:47.000000 prefect_github-0.2.4/prefect_github/configs/query/organization.json
--rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-04-26 15:03:47.000000 prefect_github-0.2.4/prefect_github/configs/query/repository.json
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-26 15:03:47.000000 prefect_github-0.2.4/prefect_github/configs/query/repository_owner.json
--rw-r--r--   0 runner    (1001) docker     (127)     9764 2024-04-26 15:03:47.000000 prefect_github-0.2.4/prefect_github/configs/query/user.json
--rw-r--r--   0 runner    (1001) docker     (127)     9766 2024-04-26 15:03:47.000000 prefect_github-0.2.4/prefect_github/configs/query/viewer.json
--rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-04-26 15:03:47.000000 prefect_github-0.2.4/prefect_github/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-26 15:03:47.000000 prefect_github-0.2.4/prefect_github/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-04-26 15:03:47.000000 prefect_github-0.2.4/prefect_github/graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)    20646 2024-04-26 15:03:47.000000 prefect_github-0.2.4/prefect_github/mutations.py
--rw-r--r--   0 runner    (1001) docker     (127)    64980 2024-04-26 15:03:47.000000 prefect_github-0.2.4/prefect_github/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)   108596 2024-04-26 15:03:47.000000 prefect_github-0.2.4/prefect_github/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-04-26 15:03:47.000000 prefect_github-0.2.4/prefect_github/repository_owner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:08.385030 prefect_github-0.2.4/prefect_github/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:47.000000 prefect_github-0.2.4/prefect_github/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  4561834 2024-04-26 15:03:47.000000 prefect_github-0.2.4/prefect_github/schemas/graphql_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)  1066892 2024-04-26 15:03:47.000000 prefect_github-0.2.4/prefect_github/schemas/graphql_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    77111 2024-04-26 15:03:47.000000 prefect_github-0.2.4/prefect_github/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-26 15:03:47.000000 prefect_github-0.2.4/prefect_github/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    73099 2024-04-26 15:03:47.000000 prefect_github-0.2.4/prefect_github/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:08.389030 prefect_github-0.2.4/prefect_github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-04-26 15:04:08.000000 prefect_github-0.2.4/prefect_github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-26 15:04:08.000000 prefect_github-0.2.4/prefect_github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:04:08.000000 prefect_github-0.2.4/prefect_github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-26 15:04:08.000000 prefect_github-0.2.4/prefect_github.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-26 15:04:08.000000 prefect_github-0.2.4/prefect_github.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-26 15:04:08.000000 prefect_github-0.2.4/prefect_github.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-26 15:03:47.000000 prefect_github-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:04:08.389030 prefect_github-0.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:08.389030 prefect_github-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-26 15:03:47.000000 prefect_github-0.2.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-26 15:03:47.000000 prefect_github-0.2.4/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-26 15:03:47.000000 prefect_github-0.2.4/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-26 15:03:47.000000 prefect_github-0.2.4/tests/test_graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-26 15:03:47.000000 prefect_github-0.2.4/tests/test_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-26 15:03:47.000000 prefect_github-0.2.4/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-26 15:03:47.000000 prefect_github-0.2.4/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:38.732838 prefect_github-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-16 20:58:26.000000 prefect_github-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-16 20:58:26.000000 prefect_github-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-05-16 20:58:38.732838 prefect_github-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-05-16 20:58:26.000000 prefect_github-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:38.720838 prefect_github-0.2.5/prefect_github/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-16 20:58:38.000000 prefect_github-0.2.5/prefect_github/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:38.716838 prefect_github-0.2.5/prefect_github/configs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:38.720838 prefect_github-0.2.5/prefect_github/configs/mutation/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/configs/mutation/add_comment.json
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/configs/mutation/add_pull_request_review.json
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/configs/mutation/add_reaction.json
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/configs/mutation/add_star.json
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/configs/mutation/close_issue.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/configs/mutation/close_pull_request.json
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/configs/mutation/create_issue.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/configs/mutation/create_pull_request.json
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/configs/mutation/remove_reaction.json
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/configs/mutation/remove_star.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/configs/mutation/request_reviews.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:38.724838 prefect_github-0.2.5/prefect_github/configs/query/
+-rw-r--r--   0 runner    (1001) docker     (127)     7626 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/configs/query/organization.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/configs/query/repository.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/configs/query/repository_owner.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9764 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/configs/query/user.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9766 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/configs/query/viewer.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20646 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/mutations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64980 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)   108596 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/repository_owner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:38.728838 prefect_github-0.2.5/prefect_github/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  4561834 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/schemas/graphql_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)  1066892 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/schemas/graphql_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77111 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73099 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:38.732838 prefect_github-0.2.5/prefect_github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-05-16 20:58:38.000000 prefect_github-0.2.5/prefect_github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-16 20:58:38.000000 prefect_github-0.2.5/prefect_github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 20:58:38.000000 prefect_github-0.2.5/prefect_github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-16 20:58:38.000000 prefect_github-0.2.5/prefect_github.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-16 20:58:38.000000 prefect_github-0.2.5/prefect_github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-16 20:58:38.000000 prefect_github-0.2.5/prefect_github.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-16 20:58:26.000000 prefect_github-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 20:58:38.732838 prefect_github-0.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:38.732838 prefect_github-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-16 20:58:26.000000 prefect_github-0.2.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-16 20:58:26.000000 prefect_github-0.2.5/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-16 20:58:26.000000 prefect_github-0.2.5/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-16 20:58:26.000000 prefect_github-0.2.5/tests/test_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-16 20:58:26.000000 prefect_github-0.2.5/tests/test_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-16 20:58:26.000000 prefect_github-0.2.5/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-16 20:58:26.000000 prefect_github-0.2.5/tests/test_version.py
```

### Comparing `prefect_github-0.2.4/LICENSE` & `prefect_github-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.4/PKG-INFO` & `prefect_github-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-github
-Version: 0.2.4
+Version: 0.2.5
 Summary: Prefect integrations interacting with GitHub
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-github
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: sgqlc>=15.0
-Requires-Dist: prefect>=2.13.5
+Requires-Dist: prefect<3.0.0,>=2.13.5
 Provides-Extra: dev
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
```

### Comparing `prefect_github-0.2.4/README.md` & `prefect_github-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.4/prefect_github/configs/mutation/add_pull_request_review.json` & `prefect_github-0.2.5/prefect_github/configs/mutation/add_pull_request_review.json`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.4/prefect_github/configs/mutation/close_issue.json` & `prefect_github-0.2.5/prefect_github/configs/mutation/close_issue.json`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.4/prefect_github/configs/mutation/close_pull_request.json` & `prefect_github-0.2.5/prefect_github/configs/mutation/close_pull_request.json`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.4/prefect_github/configs/mutation/create_issue.json` & `prefect_github-0.2.5/prefect_github/configs/mutation/create_issue.json`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.4/prefect_github/configs/mutation/create_pull_request.json` & `prefect_github-0.2.5/prefect_github/configs/mutation/create_pull_request.json`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.4/prefect_github/configs/mutation/request_reviews.json` & `prefect_github-0.2.5/prefect_github/configs/mutation/request_reviews.json`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.4/prefect_github/configs/query/organization.json` & `prefect_github-0.2.5/prefect_github/configs/query/organization.json`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.4/prefect_github/configs/query/repository.json` & `prefect_github-0.2.5/prefect_github/configs/query/repository.json`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.4/prefect_github/configs/query/repository_owner.json` & `prefect_github-0.2.5/prefect_github/configs/query/repository_owner.json`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.4/prefect_github/configs/query/user.json` & `prefect_github-0.2.5/prefect_github/configs/query/user.json`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.4/prefect_github/configs/query/viewer.json` & `prefect_github-0.2.5/prefect_github/configs/query/viewer.json`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.4/prefect_github/credentials.py` & `prefect_github-0.2.5/prefect_github/credentials.py`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.4/prefect_github/graphql.py` & `prefect_github-0.2.5/prefect_github/graphql.py`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.4/prefect_github/mutations.py` & `prefect_github-0.2.5/prefect_github/mutations.py`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.4/prefect_github/organization.py` & `prefect_github-0.2.5/prefect_github/organization.py`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.4/prefect_github/repository.py` & `prefect_github-0.2.5/prefect_github/repository.py`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.4/prefect_github/repository_owner.py` & `prefect_github-0.2.5/prefect_github/repository_owner.py`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.4/prefect_github/schemas/graphql_schema.json` & `prefect_github-0.2.5/prefect_github/schemas/graphql_schema.json`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.4/prefect_github/schemas/graphql_schema.py` & `prefect_github-0.2.5/prefect_github/schemas/graphql_schema.py`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.4/prefect_github/user.py` & `prefect_github-0.2.5/prefect_github/user.py`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.4/prefect_github/utils.py` & `prefect_github-0.2.5/prefect_github/utils.py`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.4/prefect_github/viewer.py` & `prefect_github-0.2.5/prefect_github/viewer.py`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.4/prefect_github.egg-info/PKG-INFO` & `prefect_github-0.2.5/prefect_github.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-github
-Version: 0.2.4
+Version: 0.2.5
 Summary: Prefect integrations interacting with GitHub
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-github
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: sgqlc>=15.0
-Requires-Dist: prefect>=2.13.5
+Requires-Dist: prefect<3.0.0,>=2.13.5
 Provides-Extra: dev
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
```

### Comparing `prefect_github-0.2.4/prefect_github.egg-info/SOURCES.txt` & `prefect_github-0.2.5/prefect_github.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.4/pyproject.toml` & `prefect_github-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=45", "wheel", "setuptools_scm>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prefect-github"
-dependencies = ["sgqlc>=15.0", "prefect>=2.13.5"]
+dependencies = ["sgqlc>=15.0", "prefect>=2.13.5, < 3.0.0"]
 dynamic = ["version"]
 description = "Prefect integrations interacting with GitHub"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { text = "Apache License 2.0" }
 keywords = ["prefect"]
 authors = [{ name = "Prefect Technologies, Inc.", email = "help@prefect.io" }]
```

### Comparing `prefect_github-0.2.4/tests/test_credentials.py` & `prefect_github-0.2.5/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.4/tests/test_graphql.py` & `prefect_github-0.2.5/tests/test_graphql.py`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.4/tests/test_repository.py` & `prefect_github-0.2.5/tests/test_repository.py`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.4/tests/test_utils.py` & `prefect_github-0.2.5/tests/test_utils.py`

 * *Files identical despite different names*

