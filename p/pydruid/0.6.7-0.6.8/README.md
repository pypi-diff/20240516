# Comparing `tmp/pydruid-0.6.7.tar.gz` & `tmp/pydruid-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydruid-0.6.7.tar", last modified: Mon Apr 29 19:34:54 2024, max compression
+gzip compressed data, was "pydruid-0.6.8.tar", last modified: Mon Apr 29 21:20:39 2024, max compression
```

## Comparing `pydruid-0.6.7.tar` & `pydruid-0.6.8.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 beto       (501) staff       (20)        0 2024-04-29 19:34:54.466992 pydruid-0.6.7/
--rw-r--r--   0 beto       (501) staff       (20)      150 2020-12-09 19:07:01.000000 pydruid-0.6.7/.flake8
--rw-r--r--   0 beto       (501) staff       (20)      137 2020-12-09 19:07:01.000000 pydruid-0.6.7/.gitignore
--rw-r--r--   0 beto       (501) staff       (20)      668 2024-04-29 19:31:26.000000 pydruid-0.6.7/.pre-commit-config.yaml
--rw-r--r--   0 beto       (501) staff       (20)      360 2020-12-09 19:07:01.000000 pydruid-0.6.7/.travis.yml
--rw-r--r--   0 beto       (501) staff       (20)    35132 2024-04-29 19:31:26.000000 pydruid-0.6.7/CHANGELOG.md
--rw-r--r--   0 beto       (501) staff       (20)      563 2020-12-09 19:07:01.000000 pydruid-0.6.7/LICENSE
--rw-r--r--   0 beto       (501) staff       (20)      127 2020-12-09 19:07:01.000000 pydruid-0.6.7/MANIFEST.in
--rw-r--r--   0 beto       (501) staff       (20)    12943 2024-04-29 19:34:54.467316 pydruid-0.6.7/PKG-INFO
--rw-r--r--   0 beto       (501) staff       (20)     9821 2020-12-09 19:07:01.000000 pydruid-0.6.7/README.md
--rw-r--r--   0 beto       (501) staff       (20)      570 2022-07-25 16:17:08.000000 pydruid-0.6.7/RELEASE.md
-drwxr-xr-x   0 beto       (501) staff       (20)        0 2024-04-29 19:34:54.454954 pydruid-0.6.7/docs/
--rw-r--r--   0 beto       (501) staff       (20)     6775 2020-12-09 19:07:01.000000 pydruid-0.6.7/docs/Makefile
-drwxr-xr-x   0 beto       (501) staff       (20)        0 2024-04-29 19:34:54.455669 pydruid-0.6.7/docs/figures/
--rw-r--r--   0 beto       (501) staff       (20)    26636 2020-12-09 19:07:01.000000 pydruid-0.6.7/docs/figures/avg_tweet_length.png
--rw-r--r--   0 beto       (501) staff       (20)    46319 2020-12-09 19:07:01.000000 pydruid-0.6.7/docs/figures/twitter_graph.png
-drwxr-xr-x   0 beto       (501) staff       (20)        0 2024-04-29 19:34:54.456384 pydruid-0.6.7/docs/source/
--rw-r--r--   0 beto       (501) staff       (20)     8401 2020-12-09 20:36:52.000000 pydruid-0.6.7/docs/source/conf.py
--rw-r--r--   0 beto       (501) staff       (20)     1339 2020-12-09 20:36:52.000000 pydruid-0.6.7/docs/source/index.rst
--rwxr-xr-x   0 beto       (501) staff       (20)      299 2022-11-02 22:28:56.000000 pydruid-0.6.7/gen_changelog.sh
-drwxr-xr-x   0 beto       (501) staff       (20)        0 2024-04-29 19:34:54.457909 pydruid-0.6.7/pydruid/
--rw-r--r--   0 beto       (501) staff       (20)        0 2020-12-09 19:07:01.000000 pydruid-0.6.7/pydruid/__init__.py
--rw-r--r--   0 beto       (501) staff       (20)     5875 2020-12-09 19:07:01.000000 pydruid-0.6.7/pydruid/async_client.py
--rwxr-xr-x   0 beto       (501) staff       (20)    22963 2020-12-09 19:07:01.000000 pydruid-0.6.7/pydruid/client.py
--rw-r--r--   0 beto       (501) staff       (20)     4461 2020-12-09 19:07:01.000000 pydruid-0.6.7/pydruid/console.py
-drwxr-xr-x   0 beto       (501) staff       (20)        0 2024-04-29 19:34:54.461089 pydruid-0.6.7/pydruid/db/
--rw-r--r--   0 beto       (501) staff       (20)      652 2020-12-09 19:07:01.000000 pydruid-0.6.7/pydruid/db/__init__.py
--rw-r--r--   0 beto       (501) staff       (20)    12015 2024-04-29 19:31:26.000000 pydruid-0.6.7/pydruid/db/api.py
--rw-r--r--   0 beto       (501) staff       (20)      475 2024-04-29 19:31:26.000000 pydruid-0.6.7/pydruid/db/exceptions.py
--rw-r--r--   0 beto       (501) staff       (20)     7187 2024-04-29 19:31:26.000000 pydruid-0.6.7/pydruid/db/sqlalchemy.py
--rw-r--r--   0 beto       (501) staff       (20)    17347 2024-04-29 19:31:26.000000 pydruid-0.6.7/pydruid/query.py
-drwxr-xr-x   0 beto       (501) staff       (20)        0 2024-04-29 19:34:54.463387 pydruid-0.6.7/pydruid/utils/
--rw-r--r--   0 beto       (501) staff       (20)        0 2020-12-09 19:07:01.000000 pydruid-0.6.7/pydruid/utils/__init__.py
--rw-r--r--   0 beto       (501) staff       (20)     3069 2024-04-29 19:31:26.000000 pydruid-0.6.7/pydruid/utils/aggregators.py
--rw-r--r--   0 beto       (501) staff       (20)     5541 2020-12-09 19:07:01.000000 pydruid-0.6.7/pydruid/utils/dimensions.py
--rw-r--r--   0 beto       (501) staff       (20)    10600 2020-12-09 19:07:01.000000 pydruid-0.6.7/pydruid/utils/filters.py
--rw-r--r--   0 beto       (501) staff       (20)     3544 2020-12-09 19:07:01.000000 pydruid-0.6.7/pydruid/utils/having.py
--rw-r--r--   0 beto       (501) staff       (20)     7007 2024-04-29 19:31:26.000000 pydruid-0.6.7/pydruid/utils/postaggregator.py
--rw-r--r--   0 beto       (501) staff       (20)     1359 2020-12-09 19:07:01.000000 pydruid-0.6.7/pydruid/utils/query_utils.py
-drwxr-xr-x   0 beto       (501) staff       (20)        0 2024-04-29 19:34:54.459819 pydruid-0.6.7/pydruid.egg-info/
--rw-r--r--   0 beto       (501) staff       (20)    12943 2024-04-29 19:34:54.000000 pydruid-0.6.7/pydruid.egg-info/PKG-INFO
--rw-r--r--   0 beto       (501) staff       (20)     1206 2024-04-29 19:34:54.000000 pydruid-0.6.7/pydruid.egg-info/SOURCES.txt
--rw-r--r--   0 beto       (501) staff       (20)        1 2024-04-29 19:34:54.000000 pydruid-0.6.7/pydruid.egg-info/dependency_links.txt
--rw-r--r--   0 beto       (501) staff       (20)      226 2024-04-29 19:34:54.000000 pydruid-0.6.7/pydruid.egg-info/entry_points.txt
--rw-r--r--   0 beto       (501) staff       (20)      115 2024-04-29 19:34:54.000000 pydruid-0.6.7/pydruid.egg-info/requires.txt
--rw-r--r--   0 beto       (501) staff       (20)        8 2024-04-29 19:34:54.000000 pydruid-0.6.7/pydruid.egg-info/top_level.txt
--rwxr-xr-x   0 beto       (501) staff       (20)       77 2020-12-09 19:07:01.000000 pydruid-0.6.7/pypi_push.sh
--rw-r--r--   0 beto       (501) staff       (20)       75 2020-12-09 19:07:01.000000 pydruid-0.6.7/requirements-dev.in
--rw-r--r--   0 beto       (501) staff       (20)     2714 2020-12-09 19:07:01.000000 pydruid-0.6.7/requirements-dev.txt
--rw-r--r--   0 beto       (501) staff       (20)       34 2020-12-09 19:07:01.000000 pydruid-0.6.7/requirements.in
--rw-r--r--   0 beto       (501) staff       (20)      757 2020-12-09 19:07:01.000000 pydruid-0.6.7/requirements.txt
--rw-r--r--   0 beto       (501) staff       (20)      451 2024-04-29 19:34:54.468439 pydruid-0.6.7/setup.cfg
--rw-r--r--   0 beto       (501) staff       (20)     1734 2024-04-29 19:31:55.000000 pydruid-0.6.7/setup.py
-drwxr-xr-x   0 beto       (501) staff       (20)        0 2024-04-29 19:34:54.464360 pydruid-0.6.7/tests/
-drwxr-xr-x   0 beto       (501) staff       (20)        0 2024-04-29 19:34:54.465042 pydruid-0.6.7/tests/db/
--rw-r--r--   0 beto       (501) staff       (20)     5061 2024-04-29 19:31:26.000000 pydruid-0.6.7/tests/db/test_cursor.py
--rw-r--r--   0 beto       (501) staff       (20)     1492 2020-12-09 19:07:01.000000 pydruid-0.6.7/tests/db/test_rows_from_chunks.py
--rw-r--r--   0 beto       (501) staff       (20)     5627 2020-12-09 20:36:52.000000 pydruid-0.6.7/tests/test_async_client.py
--rw-r--r--   0 beto       (501) staff       (20)     6305 2020-12-09 20:36:52.000000 pydruid-0.6.7/tests/test_client.py
--rw-r--r--   0 beto       (501) staff       (20)    11554 2024-04-29 19:31:26.000000 pydruid-0.6.7/tests/test_query.py
-drwxr-xr-x   0 beto       (501) staff       (20)        0 2024-04-29 19:34:54.466700 pydruid-0.6.7/tests/utils/
--rw-r--r--   0 beto       (501) staff       (20)     8582 2020-12-09 19:07:01.000000 pydruid-0.6.7/tests/utils/test_aggregators.py
--rw-r--r--   0 beto       (501) staff       (20)    11885 2020-12-09 19:07:01.000000 pydruid-0.6.7/tests/utils/test_dimensions.py
--rw-r--r--   0 beto       (501) staff       (20)    16142 2020-12-09 19:07:01.000000 pydruid-0.6.7/tests/utils/test_filters.py
--rw-r--r--   0 beto       (501) staff       (20)     3840 2020-12-09 19:07:01.000000 pydruid-0.6.7/tests/utils/test_having.py
--rw-r--r--   0 beto       (501) staff       (20)      896 2020-12-09 19:07:01.000000 pydruid-0.6.7/tests/utils/test_query_utils.py
--rw-r--r--   0 beto       (501) staff       (20)      459 2020-12-09 19:07:01.000000 pydruid-0.6.7/tox.ini
+drwxr-xr-x   0 beto       (501) staff       (20)        0 2024-04-29 21:20:39.744965 pydruid-0.6.8/
+-rw-r--r--   0 beto       (501) staff       (20)      150 2020-12-09 19:07:01.000000 pydruid-0.6.8/.flake8
+-rw-r--r--   0 beto       (501) staff       (20)      137 2020-12-09 19:07:01.000000 pydruid-0.6.8/.gitignore
+-rw-r--r--   0 beto       (501) staff       (20)      668 2024-04-29 19:31:26.000000 pydruid-0.6.8/.pre-commit-config.yaml
+-rw-r--r--   0 beto       (501) staff       (20)      360 2020-12-09 19:07:01.000000 pydruid-0.6.8/.travis.yml
+-rw-r--r--   0 beto       (501) staff       (20)    35132 2024-04-29 19:31:26.000000 pydruid-0.6.8/CHANGELOG.md
+-rw-r--r--   0 beto       (501) staff       (20)      563 2020-12-09 19:07:01.000000 pydruid-0.6.8/LICENSE
+-rw-r--r--   0 beto       (501) staff       (20)      127 2020-12-09 19:07:01.000000 pydruid-0.6.8/MANIFEST.in
+-rw-r--r--   0 beto       (501) staff       (20)    12943 2024-04-29 21:20:39.745348 pydruid-0.6.8/PKG-INFO
+-rw-r--r--   0 beto       (501) staff       (20)     9821 2020-12-09 19:07:01.000000 pydruid-0.6.8/README.md
+-rw-r--r--   0 beto       (501) staff       (20)      570 2022-07-25 16:17:08.000000 pydruid-0.6.8/RELEASE.md
+drwxr-xr-x   0 beto       (501) staff       (20)        0 2024-04-29 21:20:39.729797 pydruid-0.6.8/docs/
+-rw-r--r--   0 beto       (501) staff       (20)     6775 2020-12-09 19:07:01.000000 pydruid-0.6.8/docs/Makefile
+drwxr-xr-x   0 beto       (501) staff       (20)        0 2024-04-29 21:20:39.730683 pydruid-0.6.8/docs/figures/
+-rw-r--r--   0 beto       (501) staff       (20)    26636 2020-12-09 19:07:01.000000 pydruid-0.6.8/docs/figures/avg_tweet_length.png
+-rw-r--r--   0 beto       (501) staff       (20)    46319 2020-12-09 19:07:01.000000 pydruid-0.6.8/docs/figures/twitter_graph.png
+drwxr-xr-x   0 beto       (501) staff       (20)        0 2024-04-29 21:20:39.731353 pydruid-0.6.8/docs/source/
+-rw-r--r--   0 beto       (501) staff       (20)     8401 2020-12-09 20:36:52.000000 pydruid-0.6.8/docs/source/conf.py
+-rw-r--r--   0 beto       (501) staff       (20)     1339 2020-12-09 20:36:52.000000 pydruid-0.6.8/docs/source/index.rst
+-rwxr-xr-x   0 beto       (501) staff       (20)      299 2022-11-02 22:28:56.000000 pydruid-0.6.8/gen_changelog.sh
+drwxr-xr-x   0 beto       (501) staff       (20)        0 2024-04-29 21:20:39.733010 pydruid-0.6.8/pydruid/
+-rw-r--r--   0 beto       (501) staff       (20)        0 2020-12-09 19:07:01.000000 pydruid-0.6.8/pydruid/__init__.py
+-rw-r--r--   0 beto       (501) staff       (20)     5875 2020-12-09 19:07:01.000000 pydruid-0.6.8/pydruid/async_client.py
+-rwxr-xr-x   0 beto       (501) staff       (20)    22963 2020-12-09 19:07:01.000000 pydruid-0.6.8/pydruid/client.py
+-rw-r--r--   0 beto       (501) staff       (20)     4461 2020-12-09 19:07:01.000000 pydruid-0.6.8/pydruid/console.py
+drwxr-xr-x   0 beto       (501) staff       (20)        0 2024-04-29 21:20:39.736677 pydruid-0.6.8/pydruid/db/
+-rw-r--r--   0 beto       (501) staff       (20)      652 2020-12-09 19:07:01.000000 pydruid-0.6.8/pydruid/db/__init__.py
+-rw-r--r--   0 beto       (501) staff       (20)    12010 2024-04-29 21:18:45.000000 pydruid-0.6.8/pydruid/db/api.py
+-rw-r--r--   0 beto       (501) staff       (20)      475 2024-04-29 19:31:26.000000 pydruid-0.6.8/pydruid/db/exceptions.py
+-rw-r--r--   0 beto       (501) staff       (20)     7187 2024-04-29 19:31:26.000000 pydruid-0.6.8/pydruid/db/sqlalchemy.py
+-rw-r--r--   0 beto       (501) staff       (20)    17347 2024-04-29 19:31:26.000000 pydruid-0.6.8/pydruid/query.py
+drwxr-xr-x   0 beto       (501) staff       (20)        0 2024-04-29 21:20:39.739566 pydruid-0.6.8/pydruid/utils/
+-rw-r--r--   0 beto       (501) staff       (20)        0 2020-12-09 19:07:01.000000 pydruid-0.6.8/pydruid/utils/__init__.py
+-rw-r--r--   0 beto       (501) staff       (20)     3069 2024-04-29 19:31:26.000000 pydruid-0.6.8/pydruid/utils/aggregators.py
+-rw-r--r--   0 beto       (501) staff       (20)     5541 2020-12-09 19:07:01.000000 pydruid-0.6.8/pydruid/utils/dimensions.py
+-rw-r--r--   0 beto       (501) staff       (20)    10600 2020-12-09 19:07:01.000000 pydruid-0.6.8/pydruid/utils/filters.py
+-rw-r--r--   0 beto       (501) staff       (20)     3544 2020-12-09 19:07:01.000000 pydruid-0.6.8/pydruid/utils/having.py
+-rw-r--r--   0 beto       (501) staff       (20)     7007 2024-04-29 19:31:26.000000 pydruid-0.6.8/pydruid/utils/postaggregator.py
+-rw-r--r--   0 beto       (501) staff       (20)     1359 2020-12-09 19:07:01.000000 pydruid-0.6.8/pydruid/utils/query_utils.py
+drwxr-xr-x   0 beto       (501) staff       (20)        0 2024-04-29 21:20:39.734945 pydruid-0.6.8/pydruid.egg-info/
+-rw-r--r--   0 beto       (501) staff       (20)    12943 2024-04-29 21:20:39.000000 pydruid-0.6.8/pydruid.egg-info/PKG-INFO
+-rw-r--r--   0 beto       (501) staff       (20)     1206 2024-04-29 21:20:39.000000 pydruid-0.6.8/pydruid.egg-info/SOURCES.txt
+-rw-r--r--   0 beto       (501) staff       (20)        1 2024-04-29 21:20:39.000000 pydruid-0.6.8/pydruid.egg-info/dependency_links.txt
+-rw-r--r--   0 beto       (501) staff       (20)      226 2024-04-29 21:20:39.000000 pydruid-0.6.8/pydruid.egg-info/entry_points.txt
+-rw-r--r--   0 beto       (501) staff       (20)      115 2024-04-29 21:20:39.000000 pydruid-0.6.8/pydruid.egg-info/requires.txt
+-rw-r--r--   0 beto       (501) staff       (20)        8 2024-04-29 21:20:39.000000 pydruid-0.6.8/pydruid.egg-info/top_level.txt
+-rwxr-xr-x   0 beto       (501) staff       (20)       77 2020-12-09 19:07:01.000000 pydruid-0.6.8/pypi_push.sh
+-rw-r--r--   0 beto       (501) staff       (20)       75 2020-12-09 19:07:01.000000 pydruid-0.6.8/requirements-dev.in
+-rw-r--r--   0 beto       (501) staff       (20)     2714 2020-12-09 19:07:01.000000 pydruid-0.6.8/requirements-dev.txt
+-rw-r--r--   0 beto       (501) staff       (20)       34 2020-12-09 19:07:01.000000 pydruid-0.6.8/requirements.in
+-rw-r--r--   0 beto       (501) staff       (20)      757 2020-12-09 19:07:01.000000 pydruid-0.6.8/requirements.txt
+-rw-r--r--   0 beto       (501) staff       (20)      451 2024-04-29 21:20:39.746317 pydruid-0.6.8/setup.cfg
+-rw-r--r--   0 beto       (501) staff       (20)     1734 2024-04-29 21:20:08.000000 pydruid-0.6.8/setup.py
+drwxr-xr-x   0 beto       (501) staff       (20)        0 2024-04-29 21:20:39.741134 pydruid-0.6.8/tests/
+drwxr-xr-x   0 beto       (501) staff       (20)        0 2024-04-29 21:20:39.742037 pydruid-0.6.8/tests/db/
+-rw-r--r--   0 beto       (501) staff       (20)     4893 2024-04-29 21:18:45.000000 pydruid-0.6.8/tests/db/test_cursor.py
+-rw-r--r--   0 beto       (501) staff       (20)     1492 2020-12-09 19:07:01.000000 pydruid-0.6.8/tests/db/test_rows_from_chunks.py
+-rw-r--r--   0 beto       (501) staff       (20)     5627 2020-12-09 20:36:52.000000 pydruid-0.6.8/tests/test_async_client.py
+-rw-r--r--   0 beto       (501) staff       (20)     6305 2020-12-09 20:36:52.000000 pydruid-0.6.8/tests/test_client.py
+-rw-r--r--   0 beto       (501) staff       (20)    11554 2024-04-29 19:31:26.000000 pydruid-0.6.8/tests/test_query.py
+drwxr-xr-x   0 beto       (501) staff       (20)        0 2024-04-29 21:20:39.744560 pydruid-0.6.8/tests/utils/
+-rw-r--r--   0 beto       (501) staff       (20)     8582 2020-12-09 19:07:01.000000 pydruid-0.6.8/tests/utils/test_aggregators.py
+-rw-r--r--   0 beto       (501) staff       (20)    11885 2020-12-09 19:07:01.000000 pydruid-0.6.8/tests/utils/test_dimensions.py
+-rw-r--r--   0 beto       (501) staff       (20)    16142 2020-12-09 19:07:01.000000 pydruid-0.6.8/tests/utils/test_filters.py
+-rw-r--r--   0 beto       (501) staff       (20)     3840 2020-12-09 19:07:01.000000 pydruid-0.6.8/tests/utils/test_having.py
+-rw-r--r--   0 beto       (501) staff       (20)      896 2020-12-09 19:07:01.000000 pydruid-0.6.8/tests/utils/test_query_utils.py
+-rw-r--r--   0 beto       (501) staff       (20)      459 2020-12-09 19:07:01.000000 pydruid-0.6.8/tox.ini
```

### Comparing `pydruid-0.6.7/.pre-commit-config.yaml` & `pydruid-0.6.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.7/CHANGELOG.md` & `pydruid-0.6.8/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.7/LICENSE` & `pydruid-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.7/PKG-INFO` & `pydruid-0.6.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydruid
-Version: 0.6.7
+Version: 0.6.8
 Summary: A Python connector for Druid.
 Home-page: https://druid.apache.org
 Author: Druid Developers
 Author-email: druid-development@googlegroups.com
 License: Apache License, Version 2.0
 Project-URL: Bug Tracker, https://github.com/druid-io/pydruid/issues
 Project-URL: Documentation, https://pythonhosted.org/pydruid/
```

### Comparing `pydruid-0.6.7/README.md` & `pydruid-0.6.8/README.md`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.7/RELEASE.md` & `pydruid-0.6.8/RELEASE.md`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.7/docs/Makefile` & `pydruid-0.6.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.7/docs/figures/avg_tweet_length.png` & `pydruid-0.6.8/docs/figures/avg_tweet_length.png`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.7/docs/figures/twitter_graph.png` & `pydruid-0.6.8/docs/figures/twitter_graph.png`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.7/docs/source/conf.py` & `pydruid-0.6.8/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.7/docs/source/index.rst` & `pydruid-0.6.8/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.7/pydruid/async_client.py` & `pydruid-0.6.8/pydruid/async_client.py`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.7/pydruid/client.py` & `pydruid-0.6.8/pydruid/client.py`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.7/pydruid/console.py` & `pydruid-0.6.8/pydruid/console.py`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.7/pydruid/db/__init__.py` & `pydruid-0.6.8/pydruid/db/__init__.py`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.7/pydruid/db/api.py` & `pydruid-0.6.8/pydruid/db/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -425,15 +425,15 @@
             "[{rows}]".format(rows=rows), object_pairs_hook=OrderedDict
         ):
             yield row
 
 
 def apply_parameters(operation, parameters):
     if not parameters:
-        return operation % ()
+        return operation
 
     escaped_parameters = {key: escape(value) for key, value in parameters.items()}
     return operation % escaped_parameters
 
 
 def escape(value):
     """
```

### Comparing `pydruid-0.6.7/pydruid/db/sqlalchemy.py` & `pydruid-0.6.8/pydruid/db/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.7/pydruid/query.py` & `pydruid-0.6.8/pydruid/query.py`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.7/pydruid/utils/aggregators.py` & `pydruid-0.6.8/pydruid/utils/aggregators.py`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.7/pydruid/utils/dimensions.py` & `pydruid-0.6.8/pydruid/utils/dimensions.py`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.7/pydruid/utils/filters.py` & `pydruid-0.6.8/pydruid/utils/filters.py`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.7/pydruid/utils/having.py` & `pydruid-0.6.8/pydruid/utils/having.py`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.7/pydruid/utils/postaggregator.py` & `pydruid-0.6.8/pydruid/utils/postaggregator.py`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.7/pydruid/utils/query_utils.py` & `pydruid-0.6.8/pydruid/utils/query_utils.py`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.7/pydruid.egg-info/PKG-INFO` & `pydruid-0.6.8/pydruid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydruid
-Version: 0.6.7
+Version: 0.6.8
 Summary: A Python connector for Druid.
 Home-page: https://druid.apache.org
 Author: Druid Developers
 Author-email: druid-development@googlegroups.com
 License: Apache License, Version 2.0
 Project-URL: Bug Tracker, https://github.com/druid-io/pydruid/issues
 Project-URL: Documentation, https://pythonhosted.org/pydruid/
```

### Comparing `pydruid-0.6.7/pydruid.egg-info/SOURCES.txt` & `pydruid-0.6.8/pydruid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.7/requirements-dev.txt` & `pydruid-0.6.8/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.7/requirements.txt` & `pydruid-0.6.8/requirements.txt`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.7/setup.py` & `pydruid-0.6.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 }
 
 with io.open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="pydruid",
-    version="0.6.7",
+    version="0.6.8",
     author="Druid Developers",
     author_email="druid-development@googlegroups.com",
     packages=find_packages(),
     url="https://druid.apache.org",
     project_urls={
         "Bug Tracker": "https://github.com/druid-io/pydruid/issues",
         "Documentation": "https://pythonhosted.org/pydruid/",
```

### Comparing `pydruid-0.6.7/tests/db/test_cursor.py` & `pydruid-0.6.8/tests/db/test_cursor.py`

 * *Files 4% similar despite different names*

```diff
@@ -117,19 +117,19 @@
         cursor.execute(query)
         result = cursor.fetchall()
         self.assertEqual(result, [Row(_0="alice")])
         self.assertEqual(cursor.description, [("_name", None)])
 
     def test_apply_parameters(self):
         self.assertEqual(
-            apply_parameters('SELECT 100 AS "100%%"', None), 'SELECT 100 AS "100%"'
+            apply_parameters('SELECT 100 AS "100%"', None), 'SELECT 100 AS "100%"'
         )
 
         self.assertEqual(
-            apply_parameters('SELECT 100 AS "100%%"', {}), 'SELECT 100 AS "100%"'
+            apply_parameters('SELECT 100 AS "100%"', {}), 'SELECT 100 AS "100%"'
         )
 
         self.assertEqual(
             apply_parameters('SELECT %(key)s AS "100%%"', {"key": 100}),
             'SELECT 100 AS "100%"',
         )
 
@@ -143,15 +143,10 @@
             apply_parameters("SELECT %(key)s", {"key": True}), "SELECT TRUE"
         )
 
         self.assertEqual(
             apply_parameters("SELECT %(key)s", {"key": False}), "SELECT FALSE"
         )
 
-        self.assertEqual(
-            apply_parameters("SELECT * FROM t WHERE name LIKE '%%a'", None),
-            "SELECT * FROM t WHERE name LIKE '%a'",
-        )
-
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `pydruid-0.6.7/tests/db/test_rows_from_chunks.py` & `pydruid-0.6.8/tests/db/test_rows_from_chunks.py`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.7/tests/test_async_client.py` & `pydruid-0.6.8/tests/test_async_client.py`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.7/tests/test_client.py` & `pydruid-0.6.8/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.7/tests/test_query.py` & `pydruid-0.6.8/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.7/tests/utils/test_aggregators.py` & `pydruid-0.6.8/tests/utils/test_aggregators.py`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.7/tests/utils/test_dimensions.py` & `pydruid-0.6.8/tests/utils/test_dimensions.py`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.7/tests/utils/test_filters.py` & `pydruid-0.6.8/tests/utils/test_filters.py`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.7/tests/utils/test_having.py` & `pydruid-0.6.8/tests/utils/test_having.py`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.7/tests/utils/test_query_utils.py` & `pydruid-0.6.8/tests/utils/test_query_utils.py`

 * *Files identical despite different names*

