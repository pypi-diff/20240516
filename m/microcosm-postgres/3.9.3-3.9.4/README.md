# Comparing `tmp/microcosm-postgres-3.9.3.tar.gz` & `tmp/microcosm-postgres-3.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/microcosm-postgres-3.9.3.tar", last modified: Fri Oct  6 08:50:53 2023, max compression
+gzip compressed data, was "dist/microcosm-postgres-3.9.4.tar", last modified: Wed Oct 25 15:17:17 2023, max compression
```

## Comparing `microcosm-postgres-3.9.3.tar` & `microcosm-postgres-3.9.4.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-10-06 08:50:53.000000 microcosm-postgres-3.9.3/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11357 2023-10-06 08:47:57.000000 microcosm-postgres-3.9.3/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-10-06 08:47:57.000000 microcosm-postgres-3.9.3/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)      427 2023-10-06 08:50:53.000000 microcosm-postgres-3.9.3/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4292 2023-10-06 08:47:57.000000 microcosm-postgres-3.9.3/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-10-06 08:50:53.000000 microcosm-postgres-3.9.3/microcosm_postgres/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-10-06 08:47:57.000000 microcosm-postgres-3.9.3/microcosm_postgres/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1038 2023-10-06 08:47:57.000000 microcosm-postgres-3.9.3/microcosm_postgres/cloning.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      117 2023-10-06 08:47:57.000000 microcosm-postgres-3.9.3/microcosm_postgres/constants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2465 2023-10-06 08:47:57.000000 microcosm-postgres-3.9.3/microcosm_postgres/context.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      531 2023-10-06 08:47:57.000000 microcosm-postgres-3.9.3/microcosm_postgres/createall.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4357 2023-10-06 08:47:57.000000 microcosm-postgres-3.9.3/microcosm_postgres/dag.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1026 2023-10-06 08:47:57.000000 microcosm-postgres-3.9.3/microcosm_postgres/diff.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-10-06 08:50:53.000000 microcosm-postgres-3.9.3/microcosm_postgres/encryption/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-10-06 08:47:57.000000 microcosm-postgres-3.9.3/microcosm_postgres/encryption/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       76 2023-10-06 08:47:57.000000 microcosm-postgres-3.9.3/microcosm_postgres/encryption/constants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4904 2023-10-06 08:47:57.000000 microcosm-postgres-3.9.3/microcosm_postgres/encryption/encryptor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      420 2023-10-06 08:47:57.000000 microcosm-postgres-3.9.3/microcosm_postgres/encryption/factories.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6483 2023-10-06 08:47:57.000000 microcosm-postgres-3.9.3/microcosm_postgres/encryption/models.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5206 2023-10-06 08:47:57.000000 microcosm-postgres-3.9.3/microcosm_postgres/encryption/providers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6040 2023-10-06 08:47:57.000000 microcosm-postgres-3.9.3/microcosm_postgres/encryption/registry.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3607 2023-10-06 08:47:57.000000 microcosm-postgres-3.9.3/microcosm_postgres/encryption/store.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-10-06 08:50:53.000000 microcosm-postgres-3.9.3/microcosm_postgres/encryption/v2/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-10-06 08:47:57.000000 microcosm-postgres-3.9.3/microcosm_postgres/encryption/v2/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8948 2023-10-06 08:47:57.000000 microcosm-postgres-3.9.3/microcosm_postgres/encryption/v2/column.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5728 2023-10-06 08:47:57.000000 microcosm-postgres-3.9.3/microcosm_postgres/encryption/v2/encoders.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6053 2023-10-06 08:47:57.000000 microcosm-postgres-3.9.3/microcosm_postgres/encryption/v2/encryptors.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2074 2023-10-06 08:47:57.000000 microcosm-postgres-3.9.3/microcosm_postgres/encryption/v2/utils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1613 2023-10-06 08:47:57.000000 microcosm-postgres-3.9.3/microcosm_postgres/errors.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-10-06 08:50:53.000000 microcosm-postgres-3.9.3/microcosm_postgres/factories/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-10-06 08:47:57.000000 microcosm-postgres-3.9.3/microcosm_postgres/factories/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7200 2023-10-06 08:47:57.000000 microcosm-postgres-3.9.3/microcosm_postgres/factories/engine.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1605 2023-10-06 08:47:57.000000 microcosm-postgres-3.9.3/microcosm_postgres/factories/engine_routing_strategy.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1227 2023-10-06 08:47:57.000000 microcosm-postgres-3.9.3/microcosm_postgres/factories/sessionmaker.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      276 2023-10-06 08:47:57.000000 microcosm-postgres-3.9.3/microcosm_postgres/factories/sessionmakers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5371 2023-10-06 08:47:57.000000 microcosm-postgres-3.9.3/microcosm_postgres/factories/shards.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      802 2023-10-06 08:47:57.000000 microcosm-postgres-3.9.3/microcosm_postgres/health.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      150 2023-10-06 08:47:57.000000 microcosm-postgres-3.9.3/microcosm_postgres/identifiers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2369 2023-10-06 08:47:57.000000 microcosm-postgres-3.9.3/microcosm_postgres/metrics.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8215 2023-10-06 08:47:57.000000 microcosm-postgres-3.9.3/microcosm_postgres/migrate.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5062 2023-10-06 08:47:57.000000 microcosm-postgres-3.9.3/microcosm_postgres/models.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2545 2023-10-06 08:47:57.000000 microcosm-postgres-3.9.3/microcosm_postgres/operations.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1086 2023-10-06 08:47:57.000000 microcosm-postgres-3.9.3/microcosm_postgres/sharded_subgraph.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1360 2023-10-06 08:47:57.000000 microcosm-postgres-3.9.3/microcosm_postgres/shards.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9517 2023-10-06 08:47:57.000000 microcosm-postgres-3.9.3/microcosm_postgres/store.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-10-06 08:50:53.000000 microcosm-postgres-3.9.3/microcosm_postgres/temporary/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       73 2023-10-06 08:47:57.000000 microcosm-postgres-3.9.3/microcosm_postgres/temporary/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      621 2023-10-06 08:47:57.000000 microcosm-postgres-3.9.3/microcosm_postgres/temporary/context.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1165 2023-10-06 08:47:57.000000 microcosm-postgres-3.9.3/microcosm_postgres/temporary/copy.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1880 2023-10-06 08:47:57.000000 microcosm-postgres-3.9.3/microcosm_postgres/temporary/factories.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2222 2023-10-06 08:47:57.000000 microcosm-postgres-3.9.3/microcosm_postgres/temporary/methods.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1096 2023-10-06 08:47:57.000000 microcosm-postgres-3.9.3/microcosm_postgres/toposort.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1948 2023-10-06 08:47:57.000000 microcosm-postgres-3.9.3/microcosm_postgres/types.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-10-06 08:50:53.000000 microcosm-postgres-3.9.3/microcosm_postgres.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      427 2023-10-06 08:50:53.000000 microcosm-postgres-3.9.3/microcosm_postgres.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1943 2023-10-06 08:50:53.000000 microcosm-postgres-3.9.3/microcosm_postgres.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-10-06 08:50:53.000000 microcosm-postgres-3.9.3/microcosm_postgres.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1036 2023-10-06 08:50:53.000000 microcosm-postgres-3.9.3/microcosm_postgres.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-10-06 08:50:53.000000 microcosm-postgres-3.9.3/microcosm_postgres.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)      353 2023-10-06 08:50:53.000000 microcosm-postgres-3.9.3/microcosm_postgres.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       19 2023-10-06 08:50:53.000000 microcosm-postgres-3.9.3/microcosm_postgres.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      817 2023-10-06 08:50:53.000000 microcosm-postgres-3.9.3/setup.cfg
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     2564 2023-10-06 08:47:57.000000 microcosm-postgres-3.9.3/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-10-25 15:17:17.000000 microcosm-postgres-3.9.4/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11357 2023-10-25 15:14:08.000000 microcosm-postgres-3.9.4/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-10-25 15:14:08.000000 microcosm-postgres-3.9.4/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      427 2023-10-25 15:17:17.000000 microcosm-postgres-3.9.4/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4292 2023-10-25 15:14:08.000000 microcosm-postgres-3.9.4/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-10-25 15:17:17.000000 microcosm-postgres-3.9.4/microcosm_postgres/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-10-25 15:14:08.000000 microcosm-postgres-3.9.4/microcosm_postgres/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1038 2023-10-25 15:14:08.000000 microcosm-postgres-3.9.4/microcosm_postgres/cloning.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      117 2023-10-25 15:14:08.000000 microcosm-postgres-3.9.4/microcosm_postgres/constants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2465 2023-10-25 15:14:08.000000 microcosm-postgres-3.9.4/microcosm_postgres/context.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      531 2023-10-25 15:14:08.000000 microcosm-postgres-3.9.4/microcosm_postgres/createall.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4357 2023-10-25 15:14:08.000000 microcosm-postgres-3.9.4/microcosm_postgres/dag.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1026 2023-10-25 15:14:08.000000 microcosm-postgres-3.9.4/microcosm_postgres/diff.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-10-25 15:17:17.000000 microcosm-postgres-3.9.4/microcosm_postgres/encryption/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-10-25 15:14:08.000000 microcosm-postgres-3.9.4/microcosm_postgres/encryption/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       76 2023-10-25 15:14:08.000000 microcosm-postgres-3.9.4/microcosm_postgres/encryption/constants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4904 2023-10-25 15:14:08.000000 microcosm-postgres-3.9.4/microcosm_postgres/encryption/encryptor.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      420 2023-10-25 15:14:08.000000 microcosm-postgres-3.9.4/microcosm_postgres/encryption/factories.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6483 2023-10-25 15:14:08.000000 microcosm-postgres-3.9.4/microcosm_postgres/encryption/models.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5206 2023-10-25 15:14:08.000000 microcosm-postgres-3.9.4/microcosm_postgres/encryption/providers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6040 2023-10-25 15:14:08.000000 microcosm-postgres-3.9.4/microcosm_postgres/encryption/registry.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3607 2023-10-25 15:14:08.000000 microcosm-postgres-3.9.4/microcosm_postgres/encryption/store.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-10-25 15:17:17.000000 microcosm-postgres-3.9.4/microcosm_postgres/encryption/v2/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-10-25 15:14:08.000000 microcosm-postgres-3.9.4/microcosm_postgres/encryption/v2/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9119 2023-10-25 15:14:08.000000 microcosm-postgres-3.9.4/microcosm_postgres/encryption/v2/column.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6216 2023-10-25 15:14:08.000000 microcosm-postgres-3.9.4/microcosm_postgres/encryption/v2/encoders.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6317 2023-10-25 15:14:08.000000 microcosm-postgres-3.9.4/microcosm_postgres/encryption/v2/encryptors.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       94 2023-10-25 15:14:08.000000 microcosm-postgres-3.9.4/microcosm_postgres/encryption/v2/errors.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2074 2023-10-25 15:14:08.000000 microcosm-postgres-3.9.4/microcosm_postgres/encryption/v2/utils.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1613 2023-10-25 15:14:08.000000 microcosm-postgres-3.9.4/microcosm_postgres/errors.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-10-25 15:17:17.000000 microcosm-postgres-3.9.4/microcosm_postgres/factories/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-10-25 15:14:08.000000 microcosm-postgres-3.9.4/microcosm_postgres/factories/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7200 2023-10-25 15:14:08.000000 microcosm-postgres-3.9.4/microcosm_postgres/factories/engine.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1605 2023-10-25 15:14:08.000000 microcosm-postgres-3.9.4/microcosm_postgres/factories/engine_routing_strategy.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1227 2023-10-25 15:14:08.000000 microcosm-postgres-3.9.4/microcosm_postgres/factories/sessionmaker.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      276 2023-10-25 15:14:08.000000 microcosm-postgres-3.9.4/microcosm_postgres/factories/sessionmakers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5371 2023-10-25 15:14:08.000000 microcosm-postgres-3.9.4/microcosm_postgres/factories/shards.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      802 2023-10-25 15:14:08.000000 microcosm-postgres-3.9.4/microcosm_postgres/health.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      150 2023-10-25 15:14:08.000000 microcosm-postgres-3.9.4/microcosm_postgres/identifiers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2369 2023-10-25 15:14:08.000000 microcosm-postgres-3.9.4/microcosm_postgres/metrics.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8215 2023-10-25 15:14:08.000000 microcosm-postgres-3.9.4/microcosm_postgres/migrate.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5062 2023-10-25 15:14:08.000000 microcosm-postgres-3.9.4/microcosm_postgres/models.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2545 2023-10-25 15:14:08.000000 microcosm-postgres-3.9.4/microcosm_postgres/operations.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1086 2023-10-25 15:14:08.000000 microcosm-postgres-3.9.4/microcosm_postgres/sharded_subgraph.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1360 2023-10-25 15:14:08.000000 microcosm-postgres-3.9.4/microcosm_postgres/shards.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9517 2023-10-25 15:14:08.000000 microcosm-postgres-3.9.4/microcosm_postgres/store.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-10-25 15:17:17.000000 microcosm-postgres-3.9.4/microcosm_postgres/temporary/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       73 2023-10-25 15:14:08.000000 microcosm-postgres-3.9.4/microcosm_postgres/temporary/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      621 2023-10-25 15:14:08.000000 microcosm-postgres-3.9.4/microcosm_postgres/temporary/context.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1165 2023-10-25 15:14:08.000000 microcosm-postgres-3.9.4/microcosm_postgres/temporary/copy.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1880 2023-10-25 15:14:08.000000 microcosm-postgres-3.9.4/microcosm_postgres/temporary/factories.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2222 2023-10-25 15:14:08.000000 microcosm-postgres-3.9.4/microcosm_postgres/temporary/methods.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1096 2023-10-25 15:14:08.000000 microcosm-postgres-3.9.4/microcosm_postgres/toposort.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1948 2023-10-25 15:14:08.000000 microcosm-postgres-3.9.4/microcosm_postgres/types.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-10-25 15:17:17.000000 microcosm-postgres-3.9.4/microcosm_postgres.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      427 2023-10-25 15:17:17.000000 microcosm-postgres-3.9.4/microcosm_postgres.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1986 2023-10-25 15:17:17.000000 microcosm-postgres-3.9.4/microcosm_postgres.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-10-25 15:17:17.000000 microcosm-postgres-3.9.4/microcosm_postgres.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1036 2023-10-25 15:17:17.000000 microcosm-postgres-3.9.4/microcosm_postgres.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-10-25 15:17:17.000000 microcosm-postgres-3.9.4/microcosm_postgres.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      353 2023-10-25 15:17:17.000000 microcosm-postgres-3.9.4/microcosm_postgres.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       19 2023-10-25 15:17:17.000000 microcosm-postgres-3.9.4/microcosm_postgres.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      817 2023-10-25 15:17:17.000000 microcosm-postgres-3.9.4/setup.cfg
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     2564 2023-10-25 15:14:08.000000 microcosm-postgres-3.9.4/setup.py
```

### Comparing `microcosm-postgres-3.9.3/LICENSE` & `microcosm-postgres-3.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.9.3/README.md` & `microcosm-postgres-3.9.4/README.md`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.9.3/microcosm_postgres/cloning.py` & `microcosm-postgres-3.9.4/microcosm_postgres/cloning.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.9.3/microcosm_postgres/context.py` & `microcosm-postgres-3.9.4/microcosm_postgres/context.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.9.3/microcosm_postgres/createall.py` & `microcosm-postgres-3.9.4/microcosm_postgres/createall.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.9.3/microcosm_postgres/dag.py` & `microcosm-postgres-3.9.4/microcosm_postgres/dag.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.9.3/microcosm_postgres/diff.py` & `microcosm-postgres-3.9.4/microcosm_postgres/diff.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.9.3/microcosm_postgres/encryption/encryptor.py` & `microcosm-postgres-3.9.4/microcosm_postgres/encryption/encryptor.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.9.3/microcosm_postgres/encryption/models.py` & `microcosm-postgres-3.9.4/microcosm_postgres/encryption/models.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.9.3/microcosm_postgres/encryption/providers.py` & `microcosm-postgres-3.9.4/microcosm_postgres/encryption/providers.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.9.3/microcosm_postgres/encryption/registry.py` & `microcosm-postgres-3.9.4/microcosm_postgres/encryption/registry.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.9.3/microcosm_postgres/encryption/store.py` & `microcosm-postgres-3.9.4/microcosm_postgres/encryption/store.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.9.3/microcosm_postgres/encryption/v2/column.py` & `microcosm-postgres-3.9.4/microcosm_postgres/encryption/v2/column.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 
 from sqlalchemy import ColumnElement, LargeBinary, String
 from sqlalchemy.dialects.postgresql import ARRAY
 from sqlalchemy.ext.hybrid import Comparator, hybrid_property
 from sqlalchemy.orm import InstrumentedAttribute, Mapped, mapped_column
 from sqlalchemy.sql.operators import in_op
 
+from microcosm_postgres.encryption.v2.errors import DecryptionError
+
 from .encoders import Encoder
 from .encryptors import Encryptor
 
 
 T = TypeVar("T")
 
 
@@ -166,16 +168,18 @@
         decoder_fn = encoder.decode
 
         def _prop(self):
             encrypted = getattr(self, encrypted_field)
 
             if encrypted is None:
                 return getattr(self, unencrypted_field)
-
-            return decoder_fn(decrypt_fn(encrypted))
+            try:
+                return decoder_fn(decrypt_fn(encrypted))
+            except DecryptionError:
+                return encoder.redacted_value
 
         def _prop_setter(self, value) -> None:
             # We ignore the type - should come back as a string
             # as we don't explicitly say use_array=True inside the encoder
             # Typing needs to be updated in all encoder functions to support
             # properly
             encoded = encoder_fn(value)  # type: ignore[arg-type]
```

### Comparing `microcosm-postgres-3.9.3/microcosm_postgres/encryption/v2/encoders.py` & `microcosm-postgres-3.9.4/microcosm_postgres/encryption/v2/encoders.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import json
-from datetime import datetime
+from datetime import datetime, timezone
 from decimal import Decimal
 from enum import Enum
 from typing import (
     Any,
     Callable,
     Generic,
     Literal,
@@ -22,14 +22,15 @@
 JSONType: TypeAlias = (
     "dict[str, JSONType] | list[JSONType] | str | int | float | bool | None"
 )
 
 
 class Encoder(Protocol[T]):
     sa_type: Any
+    redacted_value: T
 
     class EncodeException(Exception):
         status_code = 400
 
     class DecodeException(Exception):
         status_code = 400
 
@@ -68,119 +69,135 @@
             raise Encoder.DecodeException(f"Error decoding value: {e}")
 
     return wrapper
 
 
 class StringEncoder(Encoder[Any]):
     sa_type = sqlalchemy.String
+    redacted_value = "REDACTED"
 
     @encode_exception_wrapper
     def encode(self, value: Any, **kwargs) -> str:
         return str(value)
 
     @decode_exception_wrapper
     def decode(self, value: str, **kwargs) -> Any:
         return value
 
 
 class TextEncoder(Encoder[Any]):
     sa_type = sqlalchemy.Text
+    redacted_value = "REDACTED"
 
     @encode_exception_wrapper
     def encode(self, value: Any, **kwargs) -> str:
         return str(value)
 
     @decode_exception_wrapper
     def decode(self, value: str, **kwargs) -> Any:
         return value
 
 
 class IntEncoder(Encoder[int]):
     sa_type = sqlalchemy.Integer
+    redacted_value = -1
 
     @encode_exception_wrapper
     def encode(self, value: int, **kwargs) -> str:
         return str(value)
 
     @decode_exception_wrapper
     def decode(self, value: str, **kwargs) -> int:
         return int(value)
 
 
 class DecimalEncoder(Encoder[Decimal]):
     sa_type = sqlalchemy.Numeric(asdecimal=True)
+    redacted_value = Decimal(-1)
 
     @encode_exception_wrapper
     def encode(self, value: Decimal, **kwargs) -> str:
         return str(value)
 
     @decode_exception_wrapper
     def decode(self, value: str, **kwargs) -> Decimal:
         return Decimal(value)
 
 
 class DatetimeEncoder(Encoder[datetime]):
     sa_type = sqlalchemy.DateTime(timezone=True)
+    redacted_value = datetime(1970, 1, 1, tzinfo=timezone.utc)
 
     @encode_exception_wrapper
     def encode(self, value: datetime, **kwargs) -> str:
         return value.isoformat()
 
     @decode_exception_wrapper
     def decode(self, value: str, **kwargs) -> datetime:
         return datetime.fromisoformat(value)
 
 
 class ArrayEncoder(Encoder[list[T]], Generic[T]):
+
     def __init__(self, element_encoder: Encoder[T]):
         self.element_encoder = element_encoder
         self.sa_type = ARRAY(element_encoder.sa_type)
+        self.redacted_value = [self.element_encoder.redacted_value]
 
     @overload  # type: ignore[override]
-    def encode(self, value: list[T], keep_as_array: Literal[True], **kwargs) -> list[str]:
+    def encode(
+        self, value: list[T], keep_as_array: Literal[True], **kwargs
+    ) -> list[str]:
         ...
 
     @overload
     def encode(self, value: list[T], keep_as_array: Literal[False], **kwargs) -> str:
         ...
 
     @encode_exception_wrapper
-    def encode(self, value: list[T], keep_as_array: bool = False, **kwargs) -> list[str] | str:
+    def encode(
+        self, value: list[T], keep_as_array: bool = False, **kwargs
+    ) -> list[str] | str:
         raw = [self.element_encoder.encode(element) for element in value]
         if keep_as_array:
             assert isinstance(raw, list)
             return raw  # type: ignore[return-value]
         else:
             return json.dumps(raw)
 
     @decode_exception_wrapper
     def decode(self, value: str, **kwargs) -> list[T]:
         return [self.element_encoder.decode(v) for v in json.loads(value)]
 
 
 class JSONEncoder(Encoder[JSONType]):
     sa_type = JSONB(none_as_null=True)
+    redacted_value: JSONType = {"REDACTED": True}
 
     @encode_exception_wrapper
     def encode(self, value: JSONType, **kwargs) -> str:
         return json.dumps(value)
 
     @decode_exception_wrapper
     def decode(self, value: str, **kwargs) -> JSONType:
         return json.loads(value)
 
 
 class Nullable(Encoder[T | None], Generic[T]):
+
     def __init__(self, inner_encoder: Encoder[T]) -> None:
         self.inner_encoder = inner_encoder
         # Nullable encoder does not affect the sa_type
         self.sa_type = inner_encoder.sa_type
+        self.redacted_value = inner_encoder.redacted_value
 
     @encode_exception_wrapper
-    def encode(self, value: T | None, keep_as_array: bool = False, **kwargs) -> str | list[str]:
+    def encode(
+        self, value: T | None, keep_as_array: bool = False, **kwargs
+    ) -> str | list[str]:
         if value is None:
             return json.dumps(value)
 
         if keep_as_array:
             return self.inner_encoder.encode(value, keep_as_array=keep_as_array)
         else:
             return json.dumps(self.inner_encoder.encode(value))
@@ -197,18 +214,20 @@
 
 
 class EnumEncoder(Encoder[E], Generic[E]):
     """
     Encodes and decodes an enum by its name.
 
     """
+
     sa_type = sqlalchemy.String
 
     def __init__(self, enum: type[E]):
         self._enum = enum
+        self.redacted_value = list(self._enum)[0]
 
     @encode_exception_wrapper
     def encode(self, value: E, **kwargs) -> str:
         return value.name
 
     @decode_exception_wrapper
     def decode(self, value: str, **kwargs) -> E:
```

### Comparing `microcosm-postgres-3.9.3/microcosm_postgres/encryption/v2/encryptors.py` & `microcosm-postgres-3.9.4/microcosm_postgres/encryption/v2/encryptors.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,19 +8,21 @@
     Iterator,
     Literal,
     Protocol,
     TypeAlias,
     overload,
 )
 
+from aws_encryption_sdk.exceptions import DecryptKeyError
 from microcosm.object_graph import ObjectGraph
 
 from microcosm_postgres.constants import X_REQUEST_CLIENT_HEADER
 from microcosm_postgres.encryption.constants import ENCRYPTION_V2_DEFAULT_KEY
 from microcosm_postgres.encryption.encryptor import MultiTenantEncryptor, SingleTenantEncryptor
+from microcosm_postgres.encryption.v2.errors import DecryptionError
 
 
 class Encryptor(Protocol):
     def should_encrypt(self) -> bool:
         ...
 
     def encrypt(self, value: str) -> bytes | None:
@@ -43,15 +45,15 @@
         ...
 
     def beacon(self, value: str | list[str], use_array: bool = False) -> list[str] | str:
         """Hash value using the beacon key."""
         ...
 
 
-class PlainTextEncryptor(Encryptor):
+class PlainTextEncryptor(Encryptor, Protocol):
     def should_encrypt(self) -> bool:
         return False
 
     def encrypt(self, value: str) -> bytes | None:
         return None
 
     def decrypt(self, value: bytes) -> str | None:
@@ -159,18 +161,21 @@
         if encrypted is None:
             return None
         else:
             return encrypted[0]
 
     def decrypt(self, value: bytes) -> str | None:
         if self.encryptor_context is None:
-            raise self.EncryptorNotBound()
+            raise self.EncryptorNotBound("Decryption context is not set")
 
         context, encryptor = self.encryptor_context
-        return encryptor.decrypt(context, value)
+        try:
+            return encryptor.decrypt(context, value)
+        except DecryptKeyError as e:
+            raise DecryptionError() from e
 
     @overload
     def beacon(self, value: str, use_array: Literal[False]) -> str:
         ...
 
     @overload
     def beacon(self, value: list[str], use_array: Literal[True]) -> list[str]:
```

### Comparing `microcosm-postgres-3.9.3/microcosm_postgres/encryption/v2/utils.py` & `microcosm-postgres-3.9.4/microcosm_postgres/encryption/v2/utils.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.9.3/microcosm_postgres/errors.py` & `microcosm-postgres-3.9.4/microcosm_postgres/errors.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.9.3/microcosm_postgres/factories/engine.py` & `microcosm-postgres-3.9.4/microcosm_postgres/factories/engine.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.9.3/microcosm_postgres/factories/engine_routing_strategy.py` & `microcosm-postgres-3.9.4/microcosm_postgres/factories/engine_routing_strategy.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.9.3/microcosm_postgres/factories/sessionmaker.py` & `microcosm-postgres-3.9.4/microcosm_postgres/factories/sessionmaker.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.9.3/microcosm_postgres/factories/shards.py` & `microcosm-postgres-3.9.4/microcosm_postgres/factories/shards.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.9.3/microcosm_postgres/health.py` & `microcosm-postgres-3.9.4/microcosm_postgres/health.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.9.3/microcosm_postgres/metrics.py` & `microcosm-postgres-3.9.4/microcosm_postgres/metrics.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.9.3/microcosm_postgres/migrate.py` & `microcosm-postgres-3.9.4/microcosm_postgres/migrate.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.9.3/microcosm_postgres/models.py` & `microcosm-postgres-3.9.4/microcosm_postgres/models.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.9.3/microcosm_postgres/operations.py` & `microcosm-postgres-3.9.4/microcosm_postgres/operations.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.9.3/microcosm_postgres/sharded_subgraph.py` & `microcosm-postgres-3.9.4/microcosm_postgres/sharded_subgraph.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.9.3/microcosm_postgres/shards.py` & `microcosm-postgres-3.9.4/microcosm_postgres/shards.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.9.3/microcosm_postgres/store.py` & `microcosm-postgres-3.9.4/microcosm_postgres/store.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.9.3/microcosm_postgres/temporary/context.py` & `microcosm-postgres-3.9.4/microcosm_postgres/temporary/context.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.9.3/microcosm_postgres/temporary/copy.py` & `microcosm-postgres-3.9.4/microcosm_postgres/temporary/copy.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.9.3/microcosm_postgres/temporary/factories.py` & `microcosm-postgres-3.9.4/microcosm_postgres/temporary/factories.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.9.3/microcosm_postgres/temporary/methods.py` & `microcosm-postgres-3.9.4/microcosm_postgres/temporary/methods.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.9.3/microcosm_postgres/toposort.py` & `microcosm-postgres-3.9.4/microcosm_postgres/toposort.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.9.3/microcosm_postgres/types.py` & `microcosm-postgres-3.9.4/microcosm_postgres/types.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.9.3/microcosm_postgres.egg-info/SOURCES.txt` & `microcosm-postgres-3.9.4/microcosm_postgres.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 microcosm_postgres/encryption/providers.py
 microcosm_postgres/encryption/registry.py
 microcosm_postgres/encryption/store.py
 microcosm_postgres/encryption/v2/__init__.py
 microcosm_postgres/encryption/v2/column.py
 microcosm_postgres/encryption/v2/encoders.py
 microcosm_postgres/encryption/v2/encryptors.py
+microcosm_postgres/encryption/v2/errors.py
 microcosm_postgres/encryption/v2/utils.py
 microcosm_postgres/factories/__init__.py
 microcosm_postgres/factories/engine.py
 microcosm_postgres/factories/engine_routing_strategy.py
 microcosm_postgres/factories/sessionmaker.py
 microcosm_postgres/factories/sessionmakers.py
 microcosm_postgres/factories/shards.py
```

### Comparing `microcosm-postgres-3.9.3/microcosm_postgres.egg-info/entry_points.txt` & `microcosm-postgres-3.9.4/microcosm_postgres.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.9.3/setup.cfg` & `microcosm-postgres-3.9.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.9.3/setup.py` & `microcosm-postgres-3.9.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import find_packages, setup
 
 
 project = "microcosm-postgres"
-version = "3.9.3"
+version = "3.9.4"
 
 setup(
     name=project,
     version=version,
     description="Opinionated persistence with PostgreSQL",
     author="Globality Engineering",
     author_email="engineering@globality.com",
```

