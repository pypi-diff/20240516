# Comparing `tmp/dj-test-queries-0.2.2.tar.gz` & `tmp/dj-test-queries-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj-test-queries-0.2.2.tar", last modified: Sat Aug 26 16:03:36 2023, max compression
+gzip compressed data, was "dj-test-queries-0.3.0.tar", last modified: Thu May 16 11:59:28 2024, max compression
```

## Comparing `dj-test-queries-0.2.2.tar` & `dj-test-queries-0.3.0.tar`

### file list

```diff
@@ -1,57 +1,55 @@
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-08-26 16:03:36.070683 dj-test-queries-0.2.2/
--rw-rw-r--   0 petr      (1000) petr      (1000)      146 2023-08-26 16:03:35.000000 dj-test-queries-0.2.2/.coveragerc
--rw-rw-r--   0 petr      (1000) petr      (1000)      331 2023-08-26 16:03:35.000000 dj-test-queries-0.2.2/.editorconfig
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-08-26 16:03:36.066683 dj-test-queries-0.2.2/.github/
--rw-rw-r--   0 petr      (1000) petr      (1000)      348 2023-08-26 16:03:35.000000 dj-test-queries-0.2.2/.github/ISSUE_TEMPLATE.md
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-08-26 16:03:36.066683 dj-test-queries-0.2.2/.github/workflows/
--rw-rw-r--   0 petr      (1000) petr      (1000)     2021 2023-08-26 16:03:35.000000 dj-test-queries-0.2.2/.github/workflows/ci.yml
--rw-rw-r--   0 petr      (1000) petr      (1000)      419 2023-08-26 16:03:35.000000 dj-test-queries-0.2.2/.gitignore
--rw-rw-r--   0 petr      (1000) petr      (1000)      553 2023-08-26 16:03:35.000000 dj-test-queries-0.2.2/.travis.yml
--rw-rw-r--   0 petr      (1000) petr      (1000)      158 2023-08-26 16:03:35.000000 dj-test-queries-0.2.2/AUTHORS.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     3274 2023-08-26 16:03:35.000000 dj-test-queries-0.2.2/CONTRIBUTING.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      354 2023-08-26 16:03:35.000000 dj-test-queries-0.2.2/HISTORY.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     1075 2023-08-26 16:03:35.000000 dj-test-queries-0.2.2/LICENSE
--rw-rw-r--   0 petr      (1000) petr      (1000)      205 2023-08-26 16:03:35.000000 dj-test-queries-0.2.2/MANIFEST.in
--rw-rw-r--   0 petr      (1000) petr      (1000)     3553 2023-08-26 16:03:36.070683 dj-test-queries-0.2.2/PKG-INFO
--rw-rw-r--   0 petr      (1000) petr      (1000)     2324 2023-08-26 16:03:35.000000 dj-test-queries-0.2.2/README.rst
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-08-26 16:03:36.066683 dj-test-queries-0.2.2/dj_test_queries.egg-info/
--rw-rw-r--   0 petr      (1000) petr      (1000)     3553 2023-08-26 16:03:35.000000 dj-test-queries-0.2.2/dj_test_queries.egg-info/PKG-INFO
--rw-rw-r--   0 petr      (1000) petr      (1000)      998 2023-08-26 16:03:36.000000 dj-test-queries-0.2.2/dj_test_queries.egg-info/SOURCES.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)        1 2023-08-26 16:03:35.000000 dj-test-queries-0.2.2/dj_test_queries.egg-info/dependency_links.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)        1 2023-08-26 16:03:35.000000 dj-test-queries-0.2.2/dj_test_queries.egg-info/not-zip-safe
--rw-rw-r--   0 petr      (1000) petr      (1000)       36 2023-08-26 16:03:35.000000 dj-test-queries-0.2.2/dj_test_queries.egg-info/requires.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)       13 2023-08-26 16:03:35.000000 dj-test-queries-0.2.2/dj_test_queries.egg-info/top_level.txt
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-08-26 16:03:36.070683 dj-test-queries-0.2.2/docs/
--rw-rw-r--   0 petr      (1000) petr      (1000)     6778 2023-08-26 16:03:35.000000 dj-test-queries-0.2.2/docs/Makefile
--rw-rw-r--   0 petr      (1000) petr      (1000)       28 2023-08-26 16:03:35.000000 dj-test-queries-0.2.2/docs/authors.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     8399 2023-08-26 16:03:35.000000 dj-test-queries-0.2.2/docs/conf.py
--rw-rw-r--   0 petr      (1000) petr      (1000)       33 2023-08-26 16:03:35.000000 dj-test-queries-0.2.2/docs/contributing.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)       28 2023-08-26 16:03:35.000000 dj-test-queries-0.2.2/docs/history.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      450 2023-08-26 16:03:35.000000 dj-test-queries-0.2.2/docs/index.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      215 2023-08-26 16:03:35.000000 dj-test-queries-0.2.2/docs/installation.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     6709 2023-08-26 16:03:35.000000 dj-test-queries-0.2.2/docs/make.bat
--rw-rw-r--   0 petr      (1000) petr      (1000)       27 2023-08-26 16:03:35.000000 dj-test-queries-0.2.2/docs/readme.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      438 2023-08-26 16:03:35.000000 dj-test-queries-0.2.2/docs/usage.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      329 2023-08-26 16:03:35.000000 dj-test-queries-0.2.2/manage.py
--rw-rw-r--   0 petr      (1000) petr      (1000)       31 2023-08-26 16:03:35.000000 dj-test-queries-0.2.2/pyproject.toml
--rw-rw-r--   0 petr      (1000) petr      (1000)       71 2023-08-26 16:03:35.000000 dj-test-queries-0.2.2/requirements.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)       34 2023-08-26 16:03:35.000000 dj-test-queries-0.2.2/requirements_dev.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      102 2023-08-26 16:03:35.000000 dj-test-queries-0.2.2/requirements_test.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      575 2023-08-26 16:03:35.000000 dj-test-queries-0.2.2/runtests.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      256 2023-08-26 16:03:36.070683 dj-test-queries-0.2.2/setup.cfg
--rwxrwxr-x   0 petr      (1000) petr      (1000)     2489 2023-08-26 16:03:35.000000 dj-test-queries-0.2.2/setup.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     2232 2023-08-26 16:03:35.000000 dj-test-queries-0.2.2/tasks.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-08-26 16:03:36.070683 dj-test-queries-0.2.2/test_queries/
--rw-rw-r--   0 petr      (1000) petr      (1000)       82 2023-08-26 16:03:35.000000 dj-test-queries-0.2.2/test_queries/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     4434 2023-08-26 16:03:35.000000 dj-test-queries-0.2.2/test_queries/test_num_queries.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-08-26 16:03:36.070683 dj-test-queries-0.2.2/tests/
--rw-rw-r--   0 petr      (1000) petr      (1000)      650 2023-08-26 16:03:35.000000 dj-test-queries-0.2.2/tests/README.md
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-08-26 16:03:35.000000 dj-test-queries-0.2.2/tests/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)       90 2023-08-26 16:03:35.000000 dj-test-queries-0.2.2/tests/requirements.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)     3046 2023-08-26 16:03:35.000000 dj-test-queries-0.2.2/tests/settings.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-08-26 16:03:36.070683 dj-test-queries-0.2.2/tests/sqllog/
--rw-rw-r--   0 petr      (1000) petr      (1000)        9 2023-08-26 16:03:35.000000 dj-test-queries-0.2.2/tests/sqllog/test_num_queries.TestNumQueriesMixin.test_file_comparison_with_existing_lines_not_equal.0.sqllog
--rw-rw-r--   0 petr      (1000) petr      (1000)     8102 2023-08-26 16:03:35.000000 dj-test-queries-0.2.2/tests/test_num_queries.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      200 2023-08-26 16:03:35.000000 dj-test-queries-0.2.2/tests/urls.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      389 2023-08-26 16:03:35.000000 dj-test-queries-0.2.2/tests/wsgi.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1488 2023-08-26 16:03:35.000000 dj-test-queries-0.2.2/tox.ini
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 11:59:28.890319 dj-test-queries-0.3.0/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      146 2024-05-16 11:59:27.000000 dj-test-queries-0.3.0/.coveragerc
+-rw-rw-r--   0 petr      (1000) petr      (1000)      331 2024-05-16 11:59:27.000000 dj-test-queries-0.3.0/.editorconfig
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 11:59:28.882319 dj-test-queries-0.3.0/.github/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      348 2024-05-16 11:59:27.000000 dj-test-queries-0.3.0/.github/ISSUE_TEMPLATE.md
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 11:59:28.882319 dj-test-queries-0.3.0/.github/workflows/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2509 2024-05-16 11:59:27.000000 dj-test-queries-0.3.0/.github/workflows/ci.yml
+-rw-rw-r--   0 petr      (1000) petr      (1000)      419 2024-05-16 11:59:27.000000 dj-test-queries-0.3.0/.gitignore
+-rw-rw-r--   0 petr      (1000) petr      (1000)      553 2024-05-16 11:59:27.000000 dj-test-queries-0.3.0/.travis.yml
+-rw-rw-r--   0 petr      (1000) petr      (1000)      158 2024-05-16 11:59:27.000000 dj-test-queries-0.3.0/AUTHORS.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3274 2024-05-16 11:59:27.000000 dj-test-queries-0.3.0/CONTRIBUTING.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      561 2024-05-16 11:59:27.000000 dj-test-queries-0.3.0/HISTORY.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1075 2024-05-16 11:59:27.000000 dj-test-queries-0.3.0/LICENSE
+-rw-rw-r--   0 petr      (1000) petr      (1000)      205 2024-05-16 11:59:27.000000 dj-test-queries-0.3.0/MANIFEST.in
+-rw-r--r--   0 petr      (1000) petr      (1000)     3873 2024-05-16 11:59:28.890319 dj-test-queries-0.3.0/PKG-INFO
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2386 2024-05-16 11:59:27.000000 dj-test-queries-0.3.0/README.rst
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 11:59:28.890319 dj-test-queries-0.3.0/dj_test_queries.egg-info/
+-rw-r--r--   0 petr      (1000) petr      (1000)     3873 2024-05-16 11:59:28.000000 dj-test-queries-0.3.0/dj_test_queries.egg-info/PKG-INFO
+-rw-rw-r--   0 petr      (1000) petr      (1000)      888 2024-05-16 11:59:28.000000 dj-test-queries-0.3.0/dj_test_queries.egg-info/SOURCES.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)        1 2024-05-16 11:59:28.000000 dj-test-queries-0.3.0/dj_test_queries.egg-info/dependency_links.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)        1 2024-05-16 11:59:28.000000 dj-test-queries-0.3.0/dj_test_queries.egg-info/not-zip-safe
+-rw-rw-r--   0 petr      (1000) petr      (1000)       36 2024-05-16 11:59:28.000000 dj-test-queries-0.3.0/dj_test_queries.egg-info/requires.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)       13 2024-05-16 11:59:28.000000 dj-test-queries-0.3.0/dj_test_queries.egg-info/top_level.txt
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 11:59:28.886319 dj-test-queries-0.3.0/docs/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     6778 2024-05-16 11:59:27.000000 dj-test-queries-0.3.0/docs/Makefile
+-rw-rw-r--   0 petr      (1000) petr      (1000)       28 2024-05-16 11:59:27.000000 dj-test-queries-0.3.0/docs/authors.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     8399 2024-05-16 11:59:27.000000 dj-test-queries-0.3.0/docs/conf.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)       33 2024-05-16 11:59:27.000000 dj-test-queries-0.3.0/docs/contributing.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)       28 2024-05-16 11:59:27.000000 dj-test-queries-0.3.0/docs/history.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      450 2024-05-16 11:59:27.000000 dj-test-queries-0.3.0/docs/index.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      215 2024-05-16 11:59:27.000000 dj-test-queries-0.3.0/docs/installation.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     6709 2024-05-16 11:59:27.000000 dj-test-queries-0.3.0/docs/make.bat
+-rw-rw-r--   0 petr      (1000) petr      (1000)       27 2024-05-16 11:59:27.000000 dj-test-queries-0.3.0/docs/readme.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      438 2024-05-16 11:59:27.000000 dj-test-queries-0.3.0/docs/usage.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      329 2024-05-16 11:59:27.000000 dj-test-queries-0.3.0/manage.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)       31 2024-05-16 11:59:27.000000 dj-test-queries-0.3.0/pyproject.toml
+-rw-rw-r--   0 petr      (1000) petr      (1000)       71 2024-05-16 11:59:27.000000 dj-test-queries-0.3.0/requirements.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)       34 2024-05-16 11:59:27.000000 dj-test-queries-0.3.0/requirements_dev.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      102 2024-05-16 11:59:27.000000 dj-test-queries-0.3.0/requirements_test.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      575 2024-05-16 11:59:27.000000 dj-test-queries-0.3.0/runtests.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      256 2024-05-16 11:59:28.890319 dj-test-queries-0.3.0/setup.cfg
+-rwxrwxr-x   0 petr      (1000) petr      (1000)     2489 2024-05-16 11:59:27.000000 dj-test-queries-0.3.0/setup.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2232 2024-05-16 11:59:27.000000 dj-test-queries-0.3.0/tasks.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 11:59:28.886319 dj-test-queries-0.3.0/test_queries/
+-rw-rw-r--   0 petr      (1000) petr      (1000)       82 2024-05-16 11:59:27.000000 dj-test-queries-0.3.0/test_queries/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     6205 2024-05-16 11:59:27.000000 dj-test-queries-0.3.0/test_queries/test_num_queries.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 11:59:28.886319 dj-test-queries-0.3.0/tests/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      650 2024-05-16 11:59:27.000000 dj-test-queries-0.3.0/tests/README.md
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-05-16 11:59:27.000000 dj-test-queries-0.3.0/tests/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)       90 2024-05-16 11:59:27.000000 dj-test-queries-0.3.0/tests/requirements.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3046 2024-05-16 11:59:27.000000 dj-test-queries-0.3.0/tests/settings.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     6783 2024-05-16 11:59:27.000000 dj-test-queries-0.3.0/tests/test_num_queries.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      200 2024-05-16 11:59:27.000000 dj-test-queries-0.3.0/tests/urls.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      389 2024-05-16 11:59:27.000000 dj-test-queries-0.3.0/tests/wsgi.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1544 2024-05-16 11:59:27.000000 dj-test-queries-0.3.0/tox.ini
```

### Comparing `dj-test-queries-0.2.2/.travis.yml` & `dj-test-queries-0.3.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `dj-test-queries-0.2.2/CONTRIBUTING.rst` & `dj-test-queries-0.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dj-test-queries-0.2.2/LICENSE` & `dj-test-queries-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dj-test-queries-0.2.2/PKG-INFO` & `dj-test-queries-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-test-queries
-Version: 0.2.2
+Version: 0.3.0
 Summary: Extension of assertNumQueries that can record queries that were executed and show the differences in future runs.
 Home-page: https://github.com/PetrDlouhy/dj-test-queries
 Author: Petr Dlouhý
 Author-email: petr.dlouhy@email.cz
 License: MIT
 Keywords: dj-test-queries
 Classifier: Development Status :: 3 - Alpha
@@ -16,26 +16,28 @@
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 License-File: LICENSE
 License-File: AUTHORS.rst
+Requires-Dist: django-debug-toolbar!=4.1.0,>=3.8.1
 
 =============================
 Django test queries
 =============================
 
 .. image:: https://badge.fury.io/py/dj-test-queries.svg
     :target: https://badge.fury.io/py/dj-test-queries
 
-.. image:: https://codecov.io/gh/PetrDlouhy/dj-test-queries/branch/master/graph/badge.svg
-    :target: https://codecov.io/gh/PetrDlouhy/dj-test-queries
+.. image:: https://codecov.io/gh/PetrDlouhy/django-test-queries/branch/master/graph/badge.svg
+    :target: https://codecov.io/gh/PetrDlouhy/django-test-queries
 
 Extension of assertNumQueries that can record queries that were executed and show the differences in future runs.
+It also shows tracebac of where the query was called.
 
 Documentation
 -------------
 
 The full documentation is at https://dj-test-queries.readthedocs.io.
 
 Quickstart
@@ -108,14 +110,21 @@
 
 
 
 
 History
 -------
 
+0.3.0 (2024-05-16)
+++++++++++++++++++
+
+* output messages to the error report and replace Django SQL output
+* sort queries before diffing
+* store stacktrace and other information in .sqllog.full_record file
+
 0.2.2 (2023-08-26)
 ++++++++++++++++++
 
 * Real fix for DDT 3.8.1
 
 0.2.1 (2023-08-24)
 ++++++++++++++++++
```

### Comparing `dj-test-queries-0.2.2/README.rst` & `dj-test-queries-0.3.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 =============================
 Django test queries
 =============================
 
 .. image:: https://badge.fury.io/py/dj-test-queries.svg
     :target: https://badge.fury.io/py/dj-test-queries
 
-.. image:: https://codecov.io/gh/PetrDlouhy/dj-test-queries/branch/master/graph/badge.svg
-    :target: https://codecov.io/gh/PetrDlouhy/dj-test-queries
+.. image:: https://codecov.io/gh/PetrDlouhy/django-test-queries/branch/master/graph/badge.svg
+    :target: https://codecov.io/gh/PetrDlouhy/django-test-queries
 
 Extension of assertNumQueries that can record queries that were executed and show the differences in future runs.
+It also shows tracebac of where the query was called.
 
 Documentation
 -------------
 
 The full documentation is at https://dj-test-queries.readthedocs.io.
 
 Quickstart
```

### Comparing `dj-test-queries-0.2.2/dj_test_queries.egg-info/PKG-INFO` & `dj-test-queries-0.3.0/dj_test_queries.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-test-queries
-Version: 0.2.2
+Version: 0.3.0
 Summary: Extension of assertNumQueries that can record queries that were executed and show the differences in future runs.
 Home-page: https://github.com/PetrDlouhy/dj-test-queries
 Author: Petr Dlouhý
 Author-email: petr.dlouhy@email.cz
 License: MIT
 Keywords: dj-test-queries
 Classifier: Development Status :: 3 - Alpha
@@ -16,26 +16,28 @@
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 License-File: LICENSE
 License-File: AUTHORS.rst
+Requires-Dist: django-debug-toolbar!=4.1.0,>=3.8.1
 
 =============================
 Django test queries
 =============================
 
 .. image:: https://badge.fury.io/py/dj-test-queries.svg
     :target: https://badge.fury.io/py/dj-test-queries
 
-.. image:: https://codecov.io/gh/PetrDlouhy/dj-test-queries/branch/master/graph/badge.svg
-    :target: https://codecov.io/gh/PetrDlouhy/dj-test-queries
+.. image:: https://codecov.io/gh/PetrDlouhy/django-test-queries/branch/master/graph/badge.svg
+    :target: https://codecov.io/gh/PetrDlouhy/django-test-queries
 
 Extension of assertNumQueries that can record queries that were executed and show the differences in future runs.
+It also shows tracebac of where the query was called.
 
 Documentation
 -------------
 
 The full documentation is at https://dj-test-queries.readthedocs.io.
 
 Quickstart
@@ -108,14 +110,21 @@
 
 
 
 
 History
 -------
 
+0.3.0 (2024-05-16)
+++++++++++++++++++
+
+* output messages to the error report and replace Django SQL output
+* sort queries before diffing
+* store stacktrace and other information in .sqllog.full_record file
+
 0.2.2 (2023-08-26)
 ++++++++++++++++++
 
 * Real fix for DDT 3.8.1
 
 0.2.1 (2023-08-24)
 ++++++++++++++++++
```

### Comparing `dj-test-queries-0.2.2/dj_test_queries.egg-info/SOURCES.txt` & `dj-test-queries-0.3.0/dj_test_queries.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -40,9 +40,8 @@
 test_queries/test_num_queries.py
 tests/README.md
 tests/__init__.py
 tests/requirements.txt
 tests/settings.py
 tests/test_num_queries.py
 tests/urls.py
-tests/wsgi.py
-tests/sqllog/test_num_queries.TestNumQueriesMixin.test_file_comparison_with_existing_lines_not_equal.0.sqllog
+tests/wsgi.py
```

### Comparing `dj-test-queries-0.2.2/docs/Makefile` & `dj-test-queries-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dj-test-queries-0.2.2/docs/conf.py` & `dj-test-queries-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dj-test-queries-0.2.2/docs/make.bat` & `dj-test-queries-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dj-test-queries-0.2.2/runtests.py` & `dj-test-queries-0.3.0/runtests.py`

 * *Files identical despite different names*

### Comparing `dj-test-queries-0.2.2/setup.py` & `dj-test-queries-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `dj-test-queries-0.2.2/tasks.py` & `dj-test-queries-0.3.0/tasks.py`

 * *Files identical despite different names*

### Comparing `dj-test-queries-0.2.2/tests/README.md` & `dj-test-queries-0.3.0/tests/README.md`

 * *Files identical despite different names*

### Comparing `dj-test-queries-0.2.2/tests/settings.py` & `dj-test-queries-0.3.0/tests/settings.py`

 * *Files identical despite different names*

### Comparing `dj-test-queries-0.2.2/tests/test_num_queries.py` & `dj-test-queries-0.3.0/tests/test_num_queries.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import os
-from unittest.mock import call, patch
 
 from django.db import connections
 from django.test import TestCase
 
 from test_queries import NumQueriesMixin
 
 current_directory = os.getcwd()
 
 
 class TestNumQueriesMixin(NumQueriesMixin, TestCase):
+    def setUp(self):
+        os.environ["TEST_QUERIES_REWRITE_SQLLOGS"] = "False"
+
     def test_basic_functionality(self):
         with self.assertNumQueries(1):
             connections["default"].cursor().execute("SELECT 1")
 
     def test_file_creation(self):
         # This test checks if the SQL log file is created
-        # You might need to adjust the expected filename based on your implementation
         expected_filename = "path_to_expected_file.sqllog"  # Adjust this
         with self.assertNumQueries(1):
             connections["default"].cursor().execute("SELECT 1")
         self.assertTrue(os.path.exists(expected_filename))
 
     def test_file_comparison(self):
         # This test checks if the SQL log files are compared correctly
-        # You might need to adjust the expected filename and contents based on your implementation
         expected_filename = "path_to_expected_file.sqllog"  # Adjust this
         with open(expected_filename, "w") as f:
             f.write("SELECT 1")
         with self.assertNumQueries(1):
             connections["default"].cursor().execute("SELECT 1")
 
     def test_file_comparison_function(self):
@@ -38,119 +38,101 @@
 
         def call_sql():
             connections["default"].cursor().execute("SELECT 1")
 
         self.assertNumQueries(1, call_sql)
 
     def test_environment_variables(self):
+        """If TEST_QUERIES_DISABLE=True, all values should pass."""
         os.environ["TEST_QUERIES_DISABLE"] = "1"
-        with self.assertNumQueries(1):
+        with self.assertNumQueries(100):
             connections["default"].cursor().execute("SELECT 1")
-        # Test content of the SQL log files
-        with open(
-            "tests/sqllog/test_num_queries.TestNumQueriesMixin.test_environment_variables.0.sqllog.new",
-            "r",
-        ) as f:
-            self.assertEqual(f.read(), "SELECT 1\n")
+        os.environ["TEST_QUERIES_DISABLE"] = "0"
+        # But if TEST_QUERIES_DISABLE=False, it should fail
+        with self.assertRaisesRegex(AssertionError, "1 != 100 : 1 queries executed, 100 expected"):
+            with self.assertNumQueries(100):
+                connections["default"].cursor().execute("SELECT 1")
 
     def test_file_comparison_with_existing_lines(self):
         # This test checks if the SQL log files are compared correctly when the file already has lines
-        # You might need to adjust the expected filename and contents based on your implementation
         expected_filename = (
             "tests/sqllog/test_num_queries.TestNumQueriesMixin.test_file_comparison_with_existing_lines.0.sqllog"
         )
         with open(expected_filename, "w") as f:
             f.write("SELECT 1\nSELECT 2")  # Writing multiple lines to the file
         with self.assertNumQueries(2):
             connections["default"].cursor().execute("SELECT 1")
             connections["default"].cursor().execute("SELECT 2")
-        # Test content of the SQL log files
-        with open(
-            "tests/sqllog/test_num_queries.TestNumQueriesMixin.test_file_comparison_with_existing_lines.0.sqllog.new",
-            "r",
-        ) as f:
-            self.assertEqual(f.read(), "SELECT 1\nSELECT 2\n")
 
     def test_file_comparison_with_existing_lines_not_equal(self):
         expected_filename = (
-            "tests/sqllog/test_num_queries.TestNumQueriesMixin.test_file_comparison_with_existing_lines.0.sqllog"
+            "tests/sqllog/"
+            "test_num_queries.TestNumQueriesMixin.test_file_comparison_with_existing_lines_not_equal.0.sqllog"
         )
         with open(expected_filename, "w") as f:
-            f.write("SELECT 1")  # Writing multiple lines to the file
-        with patch("builtins.print") as mock_print:
-            with self.assertRaisesRegex(AssertionError, "Captured queries were:\n1. SELECT 1\n2. SELECT 2"):
-                with self.assertNumQueries(1):
-                    connections["default"].cursor().execute("SELECT 1")
-                    connections["default"].cursor().execute("SELECT 2")
-            self.assertEquals(mock_print.call_args_list[0], call("New query was recorded:"))
-            self.assertIn("sql: SELECT 1", mock_print.mock_calls[1].args[0]),
-            self.assertEquals(mock_print.call_args_list[2], call("See difference:"))
-            self.assertEquals(
-                mock_print.call_args_list[3],
-                call(
-                    f"  diff {current_directory}/tests/sqllog/test_num_queries."
-                    "TestNumQueriesMixin.test_file_comparison_with_existing_lines_not_equal.0.sqllog "
-                    f"{current_directory}/tests/sqllog/test_num_queries."
-                    "TestNumQueriesMixin.test_file_comparison_with_existing_lines_not_equal.0.sqllog.new"
-                ),
-            )
-            self.assertEquals(len(mock_print.call_args_list), 4)
+            f.write("SELECT 2")  # Writing multiple lines to the file
+        with self.assertRaises(AssertionError) as cm:
+            with self.assertNumQueries(1):
+                connections["default"].cursor().execute("SELECT 1")
+                connections["default"].cursor().execute("SELECT 2")
+        error_message = str(cm.exception)
+        self.assertIn("2 != 1 : 2 queries executed, 1 expected", error_message)
+        self.assertIn("New query was recorded:\n\tSELECT 1", error_message)
+        self.assertIn("See difference:", error_message)
+        self.assertIn(
+            f"diff {current_directory}/tests/sqllog/test_num_queries."
+            "TestNumQueriesMixin.test_file_comparison_with_existing_lines_not_equal.0.sqllog "
+            f"{current_directory}/tests/sqllog/test_num_queries."
+            "TestNumQueriesMixin.test_file_comparison_with_existing_lines_not_equal.0.sqllog.new",
+            error_message,
+        )
 
     def test_file_comparison_with_existing_lines_delete(self):
         expected_filename = (
             "tests/sqllog/test_num_queries."
             "TestNumQueriesMixin.test_file_comparison_with_existing_lines_delete.0.sqllog"
         )
         with open(expected_filename, "w") as f:
             f.write("SELECT 1\nSELECT 3\nSELECT 3")  # Writing multiple lines to the file
-        with patch("builtins.print") as mock_print:
-            with self.assertRaisesRegex(AssertionError, "Captured queries were:\n1. SELECT 1\n2. SELECT 2"):
-                with self.assertNumQueries(1):
-                    connections["default"].cursor().execute("SELECT 1")
-                    connections["default"].cursor().execute("SELECT 2")
-                    connections["default"].cursor().execute("SELECT 3")
-            self.assertEquals(mock_print.call_args_list[0], call("New query was recorded:"))
-            self.assertIn("sql: SELECT 2", mock_print.mock_calls[1].args[0]),
-            self.assertEquals(mock_print.call_args_list[2], call("See difference:"))
-            self.assertEquals(
-                mock_print.call_args_list[3],
-                call(
-                    f"  diff {current_directory}/tests/sqllog/test_num_queries."
-                    "TestNumQueriesMixin.test_file_comparison_with_existing_lines_delete.0.sqllog "
-                    f"{current_directory}/tests/sqllog/test_num_queries."
-                    "TestNumQueriesMixin.test_file_comparison_with_existing_lines_delete.0.sqllog.new"
-                ),
-            )
-            self.assertEquals(
-                mock_print.call_args_list[4],
-                call("delete    a[2:3] --> b[3:3] ['SELECT 3...'] --> []"),
-            )
-            self.assertEquals(len(mock_print.call_args_list), 5)
+        with self.assertRaises(AssertionError) as cm:
+            with self.assertNumQueries(1):
+                connections["default"].cursor().execute("SELECT 1")
+                connections["default"].cursor().execute("SELECT 2")
+                connections["default"].cursor().execute("SELECT 3")
+        error_message = str(cm.exception)
+        self.assertIn("3 != 1 : 3 queries executed, 1 expected", error_message)
+        self.assertIn("New query was recorded:\n\tSELECT 2", error_message)
+        self.assertIn("See difference:", error_message)
+        self.assertIn(
+            f"diff {current_directory}/tests/sqllog/test_num_queries."
+            "TestNumQueriesMixin.test_file_comparison_with_existing_lines_delete.0.sqllog "
+            f"{current_directory}/tests/sqllog/test_num_queries."
+            "TestNumQueriesMixin.test_file_comparison_with_existing_lines_delete.0.sqllog.new",
+            error_message,
+        )
+        self.assertIn("delete    a[2:3] --> b[3:3] ['SELECT 3...'] --> []", error_message)
 
     def test_file_comparison_with_existing_lines_replace(self):
         expected_filename = (
             "tests/sqllog/test_num_queries."
             "TestNumQueriesMixin.test_file_comparison_with_existing_lines_replace.0.sqllog"
         )
         with open(expected_filename, "w") as f:
-            f.write("SELECT 1\nSELECT 2\nSELECT 3\nSELECT 4\nSELECT 5")  # Writing multiple lines to the file
-        with patch("builtins.print") as mock_print:
-            with self.assertRaisesRegex(AssertionError, "Captured queries were:\n1. SELECT 1\n2. SELECT 2"):
-                with self.assertNumQueries(1):
-                    connections["default"].cursor().execute("SELECT 1")
-                    connections["default"].cursor().execute("SELECT 2")
-                    connections["default"].cursor().execute("SELECT 0")
-                    connections["default"].cursor().execute("SELECT 4")
-                    connections["default"].cursor().execute("SELECT 5")
-            self.assertEquals(mock_print.call_args_list[0], call("Query was replaced:"))
-            self.assertIn("sql: SELECT 0", mock_print.mock_calls[1].args[0]),
-            self.assertEquals(mock_print.call_args_list[2], call("See difference:"))
-            self.assertEquals(
-                mock_print.call_args_list[3],
-                call(
-                    f"  diff {current_directory}/tests/sqllog/test_num_queries."
-                    "TestNumQueriesMixin.test_file_comparison_with_existing_lines_replace.0.sqllog "
-                    f"{current_directory}/tests/sqllog/test_num_queries."
-                    "TestNumQueriesMixin.test_file_comparison_with_existing_lines_replace.0.sqllog.new"
-                ),
-            )
-            self.assertEquals(len(mock_print.call_args_list), 4)
+            f.write("SELECT 1\nSELECT 2\nSELECT 3\nSELECT 5\nSELECT 6")  # Writing multiple lines to the file
+        with self.assertRaises(AssertionError) as cm:
+            with self.assertNumQueries(1):
+                connections["default"].cursor().execute("SELECT 1")
+                connections["default"].cursor().execute("SELECT 2")
+                connections["default"].cursor().execute("SELECT 4")
+                connections["default"].cursor().execute("SELECT 5")
+                connections["default"].cursor().execute("SELECT 6")
+        error_message = str(cm.exception)
+        self.assertIn("5 != 1 : 5 queries executed, 1 expected", error_message)
+        self.assertIn("Query was replaced:\n\tSELECT 4", error_message)
+        self.assertIn("See difference:", error_message)
+        self.assertIn(
+            f"diff {current_directory}/tests/sqllog/test_num_queries."
+            "TestNumQueriesMixin.test_file_comparison_with_existing_lines_replace.0.sqllog "
+            f"{current_directory}/tests/sqllog/test_num_queries."
+            "TestNumQueriesMixin.test_file_comparison_with_existing_lines_replace.0.sqllog.new",
+            error_message,
+        )
```

### Comparing `dj-test-queries-0.2.2/tox.ini` & `dj-test-queries-0.3.0/tox.ini`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,47 @@
 [tox]
 envlist =
-    {py35,py36,py37,py38}-django-22-ddt{381,400,420}
-    {py36,py37,py38}-django-30-ddt{381,400,420}
-    {py36,py37,py38}-django-31-ddt{381,400,420}
-    {py36,py37,py38,py39,py310}-django-32-ddt{381,400,420}
-    {py36,py37,py38,py39,py310}-django-40-ddt{381,400,420}
-    {py36,py37,py38,py39,py310,py311}-django-41-ddt{381,400,420}
-    {py36,py37,py38,py39,py310,py311}-django-42-ddt{381,400,420}
+    py{35,36,37,38}-django22-ddt{38,40,42,43}
+    py{36,37,38}-django30-ddt{38,40,42,43}
+    py{36,37,38}-django31-ddt{38,40,42,43}
+    py{36,37,38,39,310}-django32-ddt{38,40,42,43}
+    py{38,39,310}-django40-ddt{38,40,42,43}
+    py{38,39,310,311}-django41-ddt{38,40,42,43}
+    py{38,39,310,311,312}-django42-ddt{38,40,42,43}
+    py{310,311,312}-django50-ddt{38,40,42,43}
     flake8
     isort
     black
 
 [testenv]
 setenv =
     PYTHONPATH = {toxinidir}:{toxinidir}/test_queries
 commands =
     coverage erase
     coverage run --source test_queries runtests.py
     coverage report -m
     coverage xml
 deps =
     coverage
-    django-22: Django>=2.2,<2.3
-    django-30: Django>=3.0,<3.1
-    django-31: Django>=3.1,<3.2
-    django-32: Django>=3.2,<3.3
-    django-40: Django>=4.0,<4.1
-    django-41: Django>=4.1,<4.2
-    django-42: Django>=4.2,<4.3
-    ddt381: django-debug-toolbar==3.8.1
-    ddt400: django-debug-toolbar==4.0.0
-#   ddt410: django-debug-toolbar==4.1.0
-    ddt420: django-debug-toolbar==4.2.0
     -r{toxinidir}/requirements_test.txt
+    ddt38: django-debug-toolbar==3.8.*
+    ddt40: django-debug-toolbar==4.0.*
+#   ddt41: django-debug-toolbar==4.1.*
+    ddt42: django-debug-toolbar==4.2.*
+    ddt43: django-debug-toolbar==4.3.*
+    django22: Django>=2.2,<2.3
+    django30: Django>=3.0,<3.1
+    django31: Django>=3.1,<3.2
+    django32: Django>=3.2,<3.3
+    django40: Django>=4.0,<4.1
+    django41: Django>=4.1,<4.2
+    django42: Django>=4.2,<4.3
+    django50: Django>=5.0,<5.1
 basepython =
+    py312: python3.12
     py311: python3.11
     py310: python3.10
     py39: python3.9
     py38: python3.8
     py37: python3.7
     py36: python3.6
     py35: python3.5
```

