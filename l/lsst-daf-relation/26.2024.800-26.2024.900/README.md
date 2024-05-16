# Comparing `tmp/lsst-daf-relation-26.2024.800.tar.gz` & `tmp/lsst-daf-relation-26.2024.900.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst-daf-relation-26.2024.800.tar", last modified: Thu Feb 22 10:43:01 2024, max compression
+gzip compressed data, was "lsst-daf-relation-26.2024.900.tar", last modified: Thu Feb 29 10:20:53 2024, max compression
```

## Comparing `lsst-daf-relation-26.2024.800.tar` & `lsst-daf-relation-26.2024.900.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:01.429124 lsst-daf-relation-26.2024.800/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-02-22 10:43:01.429124 lsst-daf-relation-26.2024.800/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:01.417123 lsst-daf-relation-26.2024.800/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:01.417123 lsst-daf-relation-26.2024.800/python/lsst/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/python/lsst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:01.417123 lsst-daf-relation-26.2024.800/python/lsst/daf/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/python/lsst/daf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:01.421124 lsst-daf-relation-26.2024.800/python/lsst/daf/relation/
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/python/lsst/daf/relation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8332 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_binary_operation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:01.421124 lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_columns/
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_columns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_columns/_container.py
--rw-r--r--   0 runner    (1001) docker     (127)    18971 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_columns/_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)    11999 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_columns/_predicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_columns/_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (127)    16084 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_leaf_relation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5090 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_marker_relation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_materialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     7719 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_operation_relations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:01.425124 lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_operations/
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_operations/_calculation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_operations/_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_operations/_deduplication.py
--rw-r--r--   0 runner    (1001) docker     (127)    15498 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_operations/_join.py
--rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_operations/_projection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_operations/_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_operations/_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_operations/_sort.py
--rw-r--r--   0 runner    (1001) docker     (127)    11872 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)    31254 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_relation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)    20935 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_unary_operation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:01.425124 lsst-daf-relation-26.2024.800/python/lsst/daf/relation/iteration/
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/python/lsst/daf/relation/iteration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16769 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/python/lsst/daf/relation/iteration/_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     8844 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/python/lsst/daf/relation/iteration/_row_iterable.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/python/lsst/daf/relation/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:01.425124 lsst-daf-relation-26.2024.800/python/lsst/daf/relation/sql/
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/python/lsst/daf/relation/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39353 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/python/lsst/daf/relation/sql/_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/python/lsst/daf/relation/sql/_payload.py
--rw-r--r--   0 runner    (1001) docker     (127)    11366 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/python/lsst/daf/relation/sql/_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/python/lsst/daf/relation/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-22 10:43:01.000000 lsst-daf-relation-26.2024.800/python/lsst/daf/relation/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:01.429124 lsst-daf-relation-26.2024.800/python/lsst_daf_relation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-02-22 10:43:01.000000 lsst-daf-relation-26.2024.800/python/lsst_daf_relation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-02-22 10:43:01.000000 lsst-daf-relation-26.2024.800/python/lsst_daf_relation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 10:43:01.000000 lsst-daf-relation-26.2024.800/python/lsst_daf_relation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-02-22 10:43:01.000000 lsst-daf-relation-26.2024.800/python/lsst_daf_relation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-22 10:43:01.000000 lsst-daf-relation-26.2024.800/python/lsst_daf_relation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 10:43:01.000000 lsst-daf-relation-26.2024.800/python/lsst_daf_relation.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-22 10:43:01.429124 lsst-daf-relation-26.2024.800/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:01.429124 lsst-daf-relation-26.2024.800/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7787 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/tests/test_calculation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/tests/test_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)    16836 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/tests/test_column_expressions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8194 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/tests/test_deduplication.py
--rw-r--r--   0 runner    (1001) docker     (127)    11859 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/tests/test_diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (127)    10539 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/tests/test_join.py
--rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/tests/test_leaf_relation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/tests/test_materialization.py
--rw-r--r--   0 runner    (1001) docker     (127)    10970 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/tests/test_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8615 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/tests/test_projection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7965 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/tests/test_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12371 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/tests/test_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     8654 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/tests/test_sort.py
--rw-r--r--   0 runner    (1001) docker     (127)    33545 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/tests/test_sql_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-02-22 10:42:50.000000 lsst-daf-relation-26.2024.800/tests/test_transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:53.677351 lsst-daf-relation-26.2024.900/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-02-29 10:20:53.677351 lsst-daf-relation-26.2024.900/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:53.665351 lsst-daf-relation-26.2024.900/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:53.669351 lsst-daf-relation-26.2024.900/python/lsst/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/python/lsst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:53.669351 lsst-daf-relation-26.2024.900/python/lsst/daf/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/python/lsst/daf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:53.669351 lsst-daf-relation-26.2024.900/python/lsst/daf/relation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/python/lsst/daf/relation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8332 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_binary_operation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:53.669351 lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_columns/
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_columns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_columns/_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18971 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_columns/_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11999 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_columns/_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_columns/_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16084 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_leaf_relation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5090 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_marker_relation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_materialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7719 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_operation_relations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:53.673351 lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_operations/_calculation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_operations/_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_operations/_deduplication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15498 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_operations/_join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_operations/_projection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_operations/_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_operations/_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_operations/_sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11872 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31254 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_relation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20935 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_unary_operation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:53.673351 lsst-daf-relation-26.2024.900/python/lsst/daf/relation/iteration/
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/python/lsst/daf/relation/iteration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16769 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/python/lsst/daf/relation/iteration/_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8844 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/python/lsst/daf/relation/iteration/_row_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/python/lsst/daf/relation/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:53.673351 lsst-daf-relation-26.2024.900/python/lsst/daf/relation/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/python/lsst/daf/relation/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39353 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/python/lsst/daf/relation/sql/_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/python/lsst/daf/relation/sql/_payload.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11366 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/python/lsst/daf/relation/sql/_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/python/lsst/daf/relation/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-29 10:20:53.000000 lsst-daf-relation-26.2024.900/python/lsst/daf/relation/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:53.677351 lsst-daf-relation-26.2024.900/python/lsst_daf_relation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-02-29 10:20:53.000000 lsst-daf-relation-26.2024.900/python/lsst_daf_relation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-02-29 10:20:53.000000 lsst-daf-relation-26.2024.900/python/lsst_daf_relation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:20:53.000000 lsst-daf-relation-26.2024.900/python/lsst_daf_relation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-02-29 10:20:53.000000 lsst-daf-relation-26.2024.900/python/lsst_daf_relation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-29 10:20:53.000000 lsst-daf-relation-26.2024.900/python/lsst_daf_relation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:20:53.000000 lsst-daf-relation-26.2024.900/python/lsst_daf_relation.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-29 10:20:53.677351 lsst-daf-relation-26.2024.900/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:53.677351 lsst-daf-relation-26.2024.900/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7787 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/tests/test_calculation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/tests/test_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16836 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/tests/test_column_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8194 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/tests/test_deduplication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11859 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/tests/test_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10539 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/tests/test_join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/tests/test_leaf_relation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/tests/test_materialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10970 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/tests/test_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8615 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/tests/test_projection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7965 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/tests/test_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12371 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/tests/test_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8654 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/tests/test_sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33545 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/tests/test_sql_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-02-29 10:20:41.000000 lsst-daf-relation-26.2024.900/tests/test_transfer.py
```

### Comparing `lsst-daf-relation-26.2024.800/LICENSE` & `lsst-daf-relation-26.2024.900/LICENSE`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/PKG-INFO` & `lsst-daf-relation-26.2024.900/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-daf-relation
-Version: 26.2024.800
+Version: 26.2024.900
 Summary: An abstract system for operating on SQL and in-memory tables with relational algebra.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: GPLv3+ License
 Project-URL: Homepage, https://github.com/lsst/daf_relation
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `lsst-daf-relation-26.2024.800/README.md` & `lsst-daf-relation-26.2024.900/README.md`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/pyproject.toml` & `lsst-daf-relation-26.2024.900/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/python/lsst/daf/relation/__init__.py` & `lsst-daf-relation-26.2024.900/python/lsst/daf/relation/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_binary_operation.py` & `lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_binary_operation.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_columns/__init__.py` & `lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_columns/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_columns/_container.py` & `lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_columns/_container.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_columns/_expression.py` & `lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_columns/_expression.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_columns/_predicate.py` & `lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_columns/_predicate.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_columns/_tag.py` & `lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_columns/_tag.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_diagnostics.py` & `lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_diagnostics.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_engine.py` & `lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_engine.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_exceptions.py` & `lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_exceptions.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_leaf_relation.py` & `lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_leaf_relation.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_marker_relation.py` & `lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_marker_relation.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_materialization.py` & `lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_materialization.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_operation_relations.py` & `lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_operation_relations.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_operations/__init__.py` & `lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_operations/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_operations/_calculation.py` & `lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_operations/_calculation.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_operations/_chain.py` & `lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_operations/_chain.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_operations/_deduplication.py` & `lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_operations/_deduplication.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_operations/_join.py` & `lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_operations/_join.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_operations/_projection.py` & `lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_operations/_projection.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_operations/_selection.py` & `lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_operations/_selection.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_operations/_slice.py` & `lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_operations/_slice.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_operations/_sort.py` & `lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_operations/_sort.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_processor.py` & `lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_processor.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_relation.py` & `lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_relation.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_transfer.py` & `lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_transfer.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/python/lsst/daf/relation/_unary_operation.py` & `lsst-daf-relation-26.2024.900/python/lsst/daf/relation/_unary_operation.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/python/lsst/daf/relation/iteration/__init__.py` & `lsst-daf-relation-26.2024.900/python/lsst/daf/relation/iteration/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/python/lsst/daf/relation/iteration/_engine.py` & `lsst-daf-relation-26.2024.900/python/lsst/daf/relation/iteration/_engine.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/python/lsst/daf/relation/iteration/_row_iterable.py` & `lsst-daf-relation-26.2024.900/python/lsst/daf/relation/iteration/_row_iterable.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/python/lsst/daf/relation/sql/__init__.py` & `lsst-daf-relation-26.2024.900/python/lsst/daf/relation/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/python/lsst/daf/relation/sql/_engine.py` & `lsst-daf-relation-26.2024.900/python/lsst/daf/relation/sql/_engine.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/python/lsst/daf/relation/sql/_payload.py` & `lsst-daf-relation-26.2024.900/python/lsst/daf/relation/sql/_payload.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/python/lsst/daf/relation/sql/_select.py` & `lsst-daf-relation-26.2024.900/python/lsst/daf/relation/sql/_select.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/python/lsst/daf/relation/tests.py` & `lsst-daf-relation-26.2024.900/python/lsst/daf/relation/tests.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/python/lsst_daf_relation.egg-info/PKG-INFO` & `lsst-daf-relation-26.2024.900/python/lsst_daf_relation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-daf-relation
-Version: 26.2024.800
+Version: 26.2024.900
 Summary: An abstract system for operating on SQL and in-memory tables with relational algebra.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: GPLv3+ License
 Project-URL: Homepage, https://github.com/lsst/daf_relation
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `lsst-daf-relation-26.2024.800/python/lsst_daf_relation.egg-info/SOURCES.txt` & `lsst-daf-relation-26.2024.900/python/lsst_daf_relation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/tests/test_calculation.py` & `lsst-daf-relation-26.2024.900/tests/test_calculation.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/tests/test_chain.py` & `lsst-daf-relation-26.2024.900/tests/test_chain.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/tests/test_column_expressions.py` & `lsst-daf-relation-26.2024.900/tests/test_column_expressions.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/tests/test_deduplication.py` & `lsst-daf-relation-26.2024.900/tests/test_deduplication.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/tests/test_diagnostics.py` & `lsst-daf-relation-26.2024.900/tests/test_diagnostics.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/tests/test_join.py` & `lsst-daf-relation-26.2024.900/tests/test_join.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/tests/test_leaf_relation.py` & `lsst-daf-relation-26.2024.900/tests/test_leaf_relation.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/tests/test_materialization.py` & `lsst-daf-relation-26.2024.900/tests/test_materialization.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/tests/test_processor.py` & `lsst-daf-relation-26.2024.900/tests/test_processor.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/tests/test_projection.py` & `lsst-daf-relation-26.2024.900/tests/test_projection.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/tests/test_selection.py` & `lsst-daf-relation-26.2024.900/tests/test_selection.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/tests/test_slice.py` & `lsst-daf-relation-26.2024.900/tests/test_slice.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/tests/test_sort.py` & `lsst-daf-relation-26.2024.900/tests/test_sort.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/tests/test_sql_engine.py` & `lsst-daf-relation-26.2024.900/tests/test_sql_engine.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-relation-26.2024.800/tests/test_transfer.py` & `lsst-daf-relation-26.2024.900/tests/test_transfer.py`

 * *Files identical despite different names*

