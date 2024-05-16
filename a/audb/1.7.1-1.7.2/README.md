# Comparing `tmp/audb-1.7.1.tar.gz` & `tmp/audb-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audb-1.7.1.tar", last modified: Tue May 14 11:55:06 2024, max compression
+gzip compressed data, was "audb-1.7.2.tar", last modified: Thu May 16 12:59:56 2024, max compression
```

## Comparing `audb-1.7.1.tar` & `audb-1.7.2.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:55:06.929911 audb-1.7.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:55:06.913910 audb-1.7.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:55:06.917910 audb-1.7.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-14 11:54:56.000000 audb-1.7.1/.github/workflows/doc.yml
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-14 11:54:56.000000 audb-1.7.1/.github/workflows/linter.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-05-14 11:54:56.000000 audb-1.7.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-14 11:54:56.000000 audb-1.7.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-14 11:54:56.000000 audb-1.7.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-14 11:54:56.000000 audb-1.7.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    15441 2024-05-14 11:54:56.000000 audb-1.7.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-14 11:54:56.000000 audb-1.7.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-14 11:54:56.000000 audb-1.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-05-14 11:55:06.929911 audb-1.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-14 11:54:56.000000 audb-1.7.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:55:06.917910 audb-1.7.1/audb/
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-14 11:54:56.000000 audb-1.7.1/audb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:55:06.921910 audb-1.7.1/audb/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:54:56.000000 audb-1.7.1/audb/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19819 2024-05-14 11:54:56.000000 audb-1.7.1/audb/core/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-14 11:54:56.000000 audb-1.7.1/audb/core/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-05-14 11:54:56.000000 audb-1.7.1/audb/core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-14 11:54:56.000000 audb-1.7.1/audb/core/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-14 11:54:56.000000 audb-1.7.1/audb/core/define.py
--rw-r--r--   0 runner    (1001) docker     (127)    23145 2024-05-14 11:54:56.000000 audb-1.7.1/audb/core/dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:55:06.921910 audb-1.7.1/audb/core/etc/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-14 11:54:56.000000 audb-1.7.1/audb/core/etc/audb.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-05-14 11:54:56.000000 audb-1.7.1/audb/core/flavor.py
--rw-r--r--   0 runner    (1001) docker     (127)    18125 2024-05-14 11:54:56.000000 audb-1.7.1/audb/core/info.py
--rw-r--r--   0 runner    (1001) docker     (127)    49570 2024-05-14 11:54:56.000000 audb-1.7.1/audb/core/load.py
--rw-r--r--   0 runner    (1001) docker     (127)    11685 2024-05-14 11:54:56.000000 audb-1.7.1/audb/core/load_to.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-14 11:54:56.000000 audb-1.7.1/audb/core/lock.py
--rw-r--r--   0 runner    (1001) docker     (127)    27377 2024-05-14 11:54:56.000000 audb-1.7.1/audb/core/publish.py
--rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-05-14 11:54:56.000000 audb-1.7.1/audb/core/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-14 11:54:56.000000 audb-1.7.1/audb/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:55:06.921910 audb-1.7.1/audb/info/
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-14 11:54:56.000000 audb-1.7.1/audb/info/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:55:06.929911 audb-1.7.1/audb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-05-14 11:55:06.000000 audb-1.7.1/audb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-14 11:55:06.000000 audb-1.7.1/audb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 11:55:06.000000 audb-1.7.1/audb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-14 11:55:06.000000 audb-1.7.1/audb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-14 11:55:06.000000 audb-1.7.1/audb.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:55:06.925910 audb-1.7.1/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)    10230 2024-05-14 11:54:56.000000 audb-1.7.1/benchmarks/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    11749 2024-05-14 11:54:56.000000 audb-1.7.1/benchmarks/benchmark-dependencies-methods.py
--rw-r--r--   0 runner    (1001) docker     (127)    18387 2024-05-14 11:54:56.000000 audb-1.7.1/benchmarks/benchmark-dependencies-save-and-load.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-14 11:54:56.000000 audb-1.7.1/benchmarks/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:55:06.925910 audb-1.7.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:55:06.925910 audb-1.7.1/docs/api-src/
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-14 11:54:56.000000 audb-1.7.1/docs/api-src/audb.info.rst
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-14 11:54:56.000000 audb-1.7.1/docs/api-src/audb.rst
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-14 11:54:56.000000 audb-1.7.1/docs/authentication.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-14 11:54:56.000000 audb-1.7.1/docs/caching.rst
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-14 11:54:56.000000 audb-1.7.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-05-14 11:54:56.000000 audb-1.7.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-14 11:54:56.000000 audb-1.7.1/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-14 11:54:56.000000 audb-1.7.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-05-14 11:54:56.000000 audb-1.7.1/docs/dependencies.rst
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 11:54:56.000000 audb-1.7.1/docs/genindex.rst
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-14 11:54:56.000000 audb-1.7.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-14 11:54:56.000000 audb-1.7.1/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7162 2024-05-14 11:54:56.000000 audb-1.7.1/docs/load.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-14 11:54:56.000000 audb-1.7.1/docs/overview.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:55:06.925910 audb-1.7.1/docs/pics/
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-14 11:54:56.000000 audb-1.7.1/docs/pics/load.dot
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-14 11:54:56.000000 audb-1.7.1/docs/pics/publish.dot
--rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-05-14 11:54:56.000000 audb-1.7.1/docs/publish.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-14 11:54:56.000000 audb-1.7.1/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-14 11:54:56.000000 audb-1.7.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-05-14 11:54:56.000000 audb-1.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 11:54:56.000000 audb-1.7.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 11:55:06.929911 audb-1.7.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:55:06.929911 audb-1.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-05-14 11:54:56.000000 audb-1.7.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-14 11:54:56.000000 audb-1.7.1/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-14 11:54:56.000000 audb-1.7.1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-14 11:54:56.000000 audb-1.7.1/tests/test_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-05-14 11:54:56.000000 audb-1.7.1/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-05-14 11:54:56.000000 audb-1.7.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-05-14 11:54:56.000000 audb-1.7.1/tests/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)    14774 2024-05-14 11:54:56.000000 audb-1.7.1/tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     6139 2024-05-14 11:54:56.000000 audb-1.7.1/tests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8470 2024-05-14 11:54:56.000000 audb-1.7.1/tests/test_flavor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-05-14 11:54:56.000000 audb-1.7.1/tests/test_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    22670 2024-05-14 11:54:56.000000 audb-1.7.1/tests/test_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     7690 2024-05-14 11:54:56.000000 audb-1.7.1/tests/test_load_on_demand.py
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-05-14 11:54:56.000000 audb-1.7.1/tests/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)    12698 2024-05-14 11:54:56.000000 audb-1.7.1/tests/test_lock_db.py
--rw-r--r--   0 runner    (1001) docker     (127)    45603 2024-05-14 11:54:56.000000 audb-1.7.1/tests/test_publish.py
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-14 11:54:56.000000 audb-1.7.1/tests/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-14 11:54:56.000000 audb-1.7.1/tests/test_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:59:56.325500 audb-1.7.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:59:56.309500 audb-1.7.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:59:56.313500 audb-1.7.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-16 12:59:50.000000 audb-1.7.2/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-16 12:59:50.000000 audb-1.7.2/.github/workflows/linter.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-05-16 12:59:50.000000 audb-1.7.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-16 12:59:50.000000 audb-1.7.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-16 12:59:50.000000 audb-1.7.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-16 12:59:50.000000 audb-1.7.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    15612 2024-05-16 12:59:50.000000 audb-1.7.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-16 12:59:50.000000 audb-1.7.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-16 12:59:50.000000 audb-1.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-05-16 12:59:56.325500 audb-1.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-16 12:59:50.000000 audb-1.7.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:59:56.313500 audb-1.7.2/audb/
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-16 12:59:50.000000 audb-1.7.2/audb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:59:56.317500 audb-1.7.2/audb/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 12:59:50.000000 audb-1.7.2/audb/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19829 2024-05-16 12:59:50.000000 audb-1.7.2/audb/core/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-16 12:59:50.000000 audb-1.7.2/audb/core/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-05-16 12:59:50.000000 audb-1.7.2/audb/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-16 12:59:50.000000 audb-1.7.2/audb/core/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-16 12:59:50.000000 audb-1.7.2/audb/core/define.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23145 2024-05-16 12:59:50.000000 audb-1.7.2/audb/core/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:59:56.317500 audb-1.7.2/audb/core/etc/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-16 12:59:50.000000 audb-1.7.2/audb/core/etc/audb.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-05-16 12:59:50.000000 audb-1.7.2/audb/core/flavor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18125 2024-05-16 12:59:50.000000 audb-1.7.2/audb/core/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49570 2024-05-16 12:59:50.000000 audb-1.7.2/audb/core/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11685 2024-05-16 12:59:50.000000 audb-1.7.2/audb/core/load_to.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-16 12:59:50.000000 audb-1.7.2/audb/core/lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27377 2024-05-16 12:59:50.000000 audb-1.7.2/audb/core/publish.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-05-16 12:59:50.000000 audb-1.7.2/audb/core/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-16 12:59:50.000000 audb-1.7.2/audb/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:59:56.317500 audb-1.7.2/audb/info/
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-16 12:59:50.000000 audb-1.7.2/audb/info/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:59:56.325500 audb-1.7.2/audb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-05-16 12:59:56.000000 audb-1.7.2/audb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-16 12:59:56.000000 audb-1.7.2/audb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 12:59:56.000000 audb-1.7.2/audb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-16 12:59:56.000000 audb-1.7.2/audb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-16 12:59:56.000000 audb-1.7.2/audb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:59:56.317500 audb-1.7.2/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)    10230 2024-05-16 12:59:50.000000 audb-1.7.2/benchmarks/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11749 2024-05-16 12:59:50.000000 audb-1.7.2/benchmarks/benchmark-dependencies-methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18387 2024-05-16 12:59:50.000000 audb-1.7.2/benchmarks/benchmark-dependencies-save-and-load.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-16 12:59:50.000000 audb-1.7.2/benchmarks/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:59:56.321500 audb-1.7.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:59:56.321500 audb-1.7.2/docs/api-src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-16 12:59:50.000000 audb-1.7.2/docs/api-src/audb.info.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-16 12:59:50.000000 audb-1.7.2/docs/api-src/audb.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-16 12:59:50.000000 audb-1.7.2/docs/authentication.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-16 12:59:50.000000 audb-1.7.2/docs/caching.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-16 12:59:50.000000 audb-1.7.2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-05-16 12:59:50.000000 audb-1.7.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-16 12:59:50.000000 audb-1.7.2/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-16 12:59:50.000000 audb-1.7.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-05-16 12:59:50.000000 audb-1.7.2/docs/dependencies.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-16 12:59:50.000000 audb-1.7.2/docs/genindex.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-16 12:59:50.000000 audb-1.7.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-16 12:59:50.000000 audb-1.7.2/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7162 2024-05-16 12:59:50.000000 audb-1.7.2/docs/load.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-16 12:59:50.000000 audb-1.7.2/docs/overview.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:59:56.321500 audb-1.7.2/docs/pics/
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-16 12:59:50.000000 audb-1.7.2/docs/pics/load.dot
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-16 12:59:50.000000 audb-1.7.2/docs/pics/publish.dot
+-rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-05-16 12:59:50.000000 audb-1.7.2/docs/publish.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-16 12:59:50.000000 audb-1.7.2/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-16 12:59:50.000000 audb-1.7.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-05-16 12:59:50.000000 audb-1.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-16 12:59:50.000000 audb-1.7.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 12:59:56.325500 audb-1.7.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:59:56.325500 audb-1.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-05-16 12:59:50.000000 audb-1.7.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-16 12:59:50.000000 audb-1.7.2/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-16 12:59:50.000000 audb-1.7.2/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-16 12:59:50.000000 audb-1.7.2/tests/test_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-05-16 12:59:50.000000 audb-1.7.2/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-05-16 12:59:50.000000 audb-1.7.2/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-05-16 12:59:50.000000 audb-1.7.2/tests/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14774 2024-05-16 12:59:50.000000 audb-1.7.2/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6139 2024-05-16 12:59:50.000000 audb-1.7.2/tests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8470 2024-05-16 12:59:50.000000 audb-1.7.2/tests/test_flavor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-05-16 12:59:50.000000 audb-1.7.2/tests/test_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22670 2024-05-16 12:59:50.000000 audb-1.7.2/tests/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7690 2024-05-16 12:59:50.000000 audb-1.7.2/tests/test_load_on_demand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-05-16 12:59:50.000000 audb-1.7.2/tests/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12698 2024-05-16 12:59:50.000000 audb-1.7.2/tests/test_lock_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45603 2024-05-16 12:59:50.000000 audb-1.7.2/tests/test_publish.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-16 12:59:50.000000 audb-1.7.2/tests/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-16 12:59:50.000000 audb-1.7.2/tests/test_repository.py
```

### Comparing `audb-1.7.1/.github/workflows/doc.yml` & `audb-1.7.2/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/.github/workflows/linter.yml` & `audb-1.7.2/.github/workflows/linter.yml`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/.github/workflows/publish.yml` & `audb-1.7.2/.github/workflows/publish.yml`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         pip install -r docs/requirements.txt
 
     - name: Build documentation
       run: |
         python -m sphinx docs/ docs/_build/ -b html
 
     - name: Deploy documentation to Github pages
-      uses: peaceiris/actions-gh-pages@v3
+      uses: peaceiris/actions-gh-pages@v4
       with:
         github_token: ${{ secrets.GITHUB_TOKEN }}
         publish_dir: ./docs/_build
 
     # Github release
     - name: Read CHANGELOG
       id: changelog
```

### Comparing `audb-1.7.1/.github/workflows/test.yml` & `audb-1.7.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/.pre-commit-config.yaml` & `audb-1.7.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/CHANGELOG.rst` & `audb-1.7.2/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,22 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
 
+Version 1.7.2 (2024-05-16)
+--------------------------
+
+* Fixed: loading of dependency table from cache
+  under Python 3.8,
+  when stored by an older version of ``audb``
+
+
 Version 1.7.1 (2024-05-14)
 --------------------------
 
 * Fixed: require ``pandas>=2.0.1``
   for ``pyarrow`` based data types
```

### Comparing `audb-1.7.1/CONTRIBUTING.rst` & `audb-1.7.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/LICENSE` & `audb-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/PKG-INFO` & `audb-1.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audb
-Version: 1.7.1
+Version: 1.7.2
 Summary: Load and publish databases in audformat
 Author-email: Hagen Wierstorf <hwierstorf@audeering.com>, Johannes Wagner <jwagner@audeering.com>
 License: MIT License
         
         Copyright (c) 2018-present audEERING GmbH and Contributors
         
         Authors:
```

### Comparing `audb-1.7.1/README.rst` & `audb-1.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/audb/__init__.py` & `audb-1.7.2/audb/__init__.py`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/audb/core/api.py` & `audb-1.7.2/audb/core/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -267,15 +267,15 @@
     )
     cached_deps_file = os.path.join(db_root, define.CACHED_DEPENDENCIES_FILE)
 
     with FolderLock(db_root):
         try:
             deps = Dependencies()
             deps.load(cached_deps_file)
-        except (AttributeError, FileNotFoundError, ValueError, EOFError):
+        except (AttributeError, EOFError, FileNotFoundError, KeyError, ValueError):
             # If loading cached file fails, load again from backend
             backend_interface = utils.lookup_backend(name, version)
             deps = download_dependencies(backend_interface, name, version, verbose)
             # Store as pickle in cache
             deps.save(cached_deps_file)
 
     return deps
```

### Comparing `audb-1.7.1/audb/core/cache.py` & `audb-1.7.2/audb/core/cache.py`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/audb/core/config.py` & `audb-1.7.2/audb/core/config.py`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/audb/core/conftest.py` & `audb-1.7.2/audb/core/conftest.py`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/audb/core/define.py` & `audb-1.7.2/audb/core/define.py`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/audb/core/dependencies.py` & `audb-1.7.2/audb/core/dependencies.py`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/audb/core/flavor.py` & `audb-1.7.2/audb/core/flavor.py`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/audb/core/info.py` & `audb-1.7.2/audb/core/info.py`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/audb/core/load.py` & `audb-1.7.2/audb/core/load.py`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/audb/core/load_to.py` & `audb-1.7.2/audb/core/load_to.py`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/audb/core/lock.py` & `audb-1.7.2/audb/core/lock.py`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/audb/core/publish.py` & `audb-1.7.2/audb/core/publish.py`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/audb/core/repository.py` & `audb-1.7.2/audb/core/repository.py`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/audb/core/utils.py` & `audb-1.7.2/audb/core/utils.py`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/audb/info/__init__.py` & `audb-1.7.2/audb/info/__init__.py`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/audb.egg-info/PKG-INFO` & `audb-1.7.2/audb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audb
-Version: 1.7.1
+Version: 1.7.2
 Summary: Load and publish databases in audformat
 Author-email: Hagen Wierstorf <hwierstorf@audeering.com>, Johannes Wagner <jwagner@audeering.com>
 License: MIT License
         
         Copyright (c) 2018-present audEERING GmbH and Contributors
         
         Authors:
```

### Comparing `audb-1.7.1/audb.egg-info/SOURCES.txt` & `audb-1.7.2/audb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/benchmarks/README.md` & `audb-1.7.2/benchmarks/README.md`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/benchmarks/benchmark-dependencies-methods.py` & `audb-1.7.2/benchmarks/benchmark-dependencies-methods.py`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/benchmarks/benchmark-dependencies-save-and-load.py` & `audb-1.7.2/benchmarks/benchmark-dependencies-save-and-load.py`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/docs/api-src/audb.info.rst` & `audb-1.7.2/docs/api-src/audb.info.rst`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/docs/caching.rst` & `audb-1.7.2/docs/caching.rst`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/docs/conf.py` & `audb-1.7.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/docs/configuration.rst` & `audb-1.7.2/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/docs/dependencies.rst` & `audb-1.7.2/docs/dependencies.rst`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/docs/index.rst` & `audb-1.7.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/docs/install.rst` & `audb-1.7.2/docs/install.rst`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/docs/load.rst` & `audb-1.7.2/docs/load.rst`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/docs/overview.rst` & `audb-1.7.2/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/docs/pics/load.dot` & `audb-1.7.2/docs/pics/load.dot`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/docs/pics/publish.dot` & `audb-1.7.2/docs/pics/publish.dot`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/docs/publish.rst` & `audb-1.7.2/docs/publish.rst`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/docs/quickstart.rst` & `audb-1.7.2/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/pyproject.toml` & `audb-1.7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/tests/conftest.py` & `audb-1.7.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/tests/test_api.py` & `audb-1.7.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/tests/test_backend.py` & `audb-1.7.2/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/tests/test_cache.py` & `audb-1.7.2/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/tests/test_config.py` & `audb-1.7.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/tests/test_convert.py` & `audb-1.7.2/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/tests/test_dependencies.py` & `audb-1.7.2/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/tests/test_filter.py` & `audb-1.7.2/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/tests/test_flavor.py` & `audb-1.7.2/tests/test_flavor.py`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/tests/test_info.py` & `audb-1.7.2/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/tests/test_load.py` & `audb-1.7.2/tests/test_load.py`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/tests/test_load_on_demand.py` & `audb-1.7.2/tests/test_load_on_demand.py`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/tests/test_lock.py` & `audb-1.7.2/tests/test_lock.py`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/tests/test_lock_db.py` & `audb-1.7.2/tests/test_lock_db.py`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/tests/test_publish.py` & `audb-1.7.2/tests/test_publish.py`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/tests/test_remove.py` & `audb-1.7.2/tests/test_remove.py`

 * *Files identical despite different names*

### Comparing `audb-1.7.1/tests/test_repository.py` & `audb-1.7.2/tests/test_repository.py`

 * *Files identical despite different names*

