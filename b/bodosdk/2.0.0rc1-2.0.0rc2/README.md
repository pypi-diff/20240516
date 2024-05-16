# Comparing `tmp/bodosdk-2.0.0rc1.tar.gz` & `tmp/bodosdk-2.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bodosdk-2.0.0rc1.tar", last modified: Mon May  6 19:03:23 2024, max compression
+gzip compressed data, was "bodosdk-2.0.0rc2.tar", last modified: Tue May  7 12:10:12 2024, max compression
```

## Comparing `bodosdk-2.0.0rc1.tar` & `bodosdk-2.0.0rc2.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:03:23.538160 bodosdk-2.0.0rc1/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    93797 2024-05-06 19:03:23.538160 bodosdk-2.0.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16330 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:03:23.538160 bodosdk-2.0.0rc1/bodosdk/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-06 19:03:23.538160 bodosdk-2.0.0rc1/bodosdk/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:03:23.534160 bodosdk-2.0.0rc1/bodosdk/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/billing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/cloud_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/instance_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/job_tpl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:03:23.534160 bodosdk-2.0.0rc1/bodosdk/api/models/
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/models/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/models/cloud_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7508 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/models/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/models/instance_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     9846 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/models/job.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/models/secret_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/models/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/models/workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/request_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/secret_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     7470 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:03:23.538160 bodosdk-2.0.0rc1/bodosdk/clients/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/clients/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    12242 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/clients/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/clients/instance_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/clients/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/clients/job_tpl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/clients/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/clients/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/clients/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:03:23.538160 bodosdk-2.0.0rc1/bodosdk/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/db/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/deprecation_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    37725 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:03:23.538160 bodosdk-2.0.0rc1/bodosdk/models/
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/models/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     8166 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/models/cloud_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    45991 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/models/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/models/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    10881 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/models/instance_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    34045 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/models/job.py
--rw-r--r--   0 runner    (1001) docker     (127)    11080 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/models/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)     9703 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/models/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:03:23.538160 bodosdk-2.0.0rc1/bodosdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    93797 2024-05-06 19:03:23.000000 bodosdk-2.0.0rc1/bodosdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-06 19:03:23.000000 bodosdk-2.0.0rc1/bodosdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 19:03:23.000000 bodosdk-2.0.0rc1/bodosdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-06 19:03:23.000000 bodosdk-2.0.0rc1/bodosdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-06 19:03:23.000000 bodosdk-2.0.0rc1/bodosdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-06 19:03:23.538160 bodosdk-2.0.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:03:23.538160 bodosdk-2.0.0rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    80088 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:10:12.841275 bodosdk-2.0.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    93676 2024-05-07 12:10:12.837275 bodosdk-2.0.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16329 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:10:12.841275 bodosdk-2.0.0rc2/bodosdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-07 12:10:12.841275 bodosdk-2.0.0rc2/bodosdk/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:10:12.833275 bodosdk-2.0.0rc2/bodosdk/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/billing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/cloud_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/instance_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/job_tpl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:10:12.833275 bodosdk-2.0.0rc2/bodosdk/api/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/models/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/models/cloud_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7508 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/models/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/models/instance_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9846 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/models/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/models/secret_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/models/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/models/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/request_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/secret_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7470 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:10:12.833275 bodosdk-2.0.0rc2/bodosdk/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/clients/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12242 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/clients/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/clients/instance_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/clients/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/clients/job_tpl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/clients/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/clients/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/clients/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:10:12.833275 bodosdk-2.0.0rc2/bodosdk/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/db/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/deprecation_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37725 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:10:12.837275 bodosdk-2.0.0rc2/bodosdk/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/models/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8166 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/models/cloud_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45991 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/models/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/models/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10881 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/models/instance_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34045 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/models/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11080 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/models/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9703 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/models/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:10:12.837275 bodosdk-2.0.0rc2/bodosdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    93676 2024-05-07 12:10:12.000000 bodosdk-2.0.0rc2/bodosdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-07 12:10:12.000000 bodosdk-2.0.0rc2/bodosdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 12:10:12.000000 bodosdk-2.0.0rc2/bodosdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-07 12:10:12.000000 bodosdk-2.0.0rc2/bodosdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 12:10:12.000000 bodosdk-2.0.0rc2/bodosdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-07 12:10:12.841275 bodosdk-2.0.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:10:12.837275 bodosdk-2.0.0rc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80088 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/versioneer.py
```

### Comparing `bodosdk-2.0.0rc1/LICENSE` & `bodosdk-2.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc1/PKG-INFO` & `bodosdk-2.0.0rc2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: bodosdk
-Version: 2.0.0rc1
-Summary: Bodo Platform SDK 2.0.0RC1
+Version: 2.0.0rc2
+Summary: Bodo Platform SDK 2.0.0RC2
 Home-page: https://github.com/Bodo-inc/bodo-sdk
 Author: Bodo, Inc.
 Author-email: noreply@bodo.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -150,15 +150,15 @@
 my_workspace = BodoWorkspaceClient()
 my_cluster = my_workspace.ClusterClient.get("cluster_id")
 if my_cluster.status != 'STOPPED':
     my_cluster.stop(wait=True)
 my_cluster.update(instance_type='c5.2xlarge', workers_quantity=2)
 ```
 
-### Create Fisrst Job
+### Create First Job
 
 On running cluster you can schedule a job in very simple way:
 First on `https://platform.bodo.ai` navigate to notebook in your workspace and
 create following `test.py` file in your main directory:
 
 ```python
 import pandas as pd
@@ -597,267 +597,267 @@
 
  #INDEX 
 
 # bodosdk package contents
 
 <a id="module-bodosdk.clients.cluster"></a>
 
-### _class_ bodosdk.clients.cluster.ClusterClient(workspace_client: IBodoWorkspaceClient)
+### *class* bodosdk.clients.cluster.ClusterClient(workspace_client: IBodoWorkspaceClient)
 
 Bases: `IClusterClient`
 
 A client for managing cluster operations in a Bodo workspace.
 
 #### \_deprecated_methods
 
 A dictionary of deprecated methods.
 
-- **Type:**
+* **Type:**
   Dict
 
 #### \_images
 
 A list of available Bodo images.
 
-- **Type:**
+* **Type:**
   List[IBodoImage]
 
-- **Parameters:**
-  **workspace_client** (_IBodoWorkspaceClient_) – The workspace client used for operations.
+* **Parameters:**
+  **workspace_client** (*IBodoWorkspaceClient*) – The workspace client used for operations.
 
-#### _property_ Cluster _: [Cluster](#bodosdk.models.cluster.Cluster)_
+#### *property* Cluster *: [Cluster](#bodosdk.models.cluster.Cluster)*
 
 Provides access to cluster operations.
 
-- **Returns:**
+* **Returns:**
   An instance of Cluster for cluster operations.
-- **Return type:**
+* **Return type:**
   [Cluster](#bodosdk.models.cluster.Cluster)
 
-#### _property_ ClusterList _: [ClusterList](#bodosdk.models.cluster.ClusterList)_
+#### *property* ClusterList *: [ClusterList](#bodosdk.models.cluster.ClusterList)*
 
 Provides access to listing clusters.
 
-- **Returns:**
+* **Returns:**
   An instance of ClusterListAPIModel for listing clusters.
-- **Return type:**
+* **Return type:**
   [ClusterList](#bodosdk.models.cluster.ClusterList)
 
 #### connect(catalog: str, cluster_id: str)
 
 #### create(name: str, instance_type: str = None, workers_quantity: int = None, description: str | None = None, bodo_version: str = None, auto_stop: int | None = None, auto_pause: int | None = None, image_id: str | None = None, accelerated_networking: bool | None = None, auto_az: bool | None = None, use_spot_instance: bool | None = None, aws_deployment_subnet_id: str | None = None, availability_zone: str | None = None, instance_role: [InstanceRole](#bodosdk.models.instance_role.InstanceRole) | Dict | None = None, custom_tags: Dict | None = None)
 
 Creates a new cluster with the specified configuration.
 
-- **Parameters:**
-  - **name** (_str_) – The name of the cluster.
-  - **instance_type** (_str_ _,_ _optional_) – The type of instance to use for the cluster nodes.
-  - **workers_quantity** (_int_ _,_ _optional_) – The number of worker nodes in the cluster.
-  - **description** (_str_ _,_ _optional_) – A description of the cluster.
-  - **bodo_version** (_str_ _,_ _optional_) – The Bodo version to use for the cluster.
-  - **auto_stop** (_int_ _,_ _optional_) – The auto-stop time in minutes for the cluster.
-  - **auto_pause** (_int_ _,_ _optional_) – The auto-pause time in minutes for the cluster.
-  - **image_id** (_str_ _,_ _optional_) – The ID of the image to use for the cluster.
-  - **accelerated_networking** (_bool_ _,_ _optional_) – Whether to use accelerated networking.
-  - **auto_az** (_bool_ _,_ _optional_) – Whether to automatically select the availability zone.
-  - **use_spot_instance** (_bool_ _,_ _optional_) – Whether to use spot instances for the cluster.
-  - **aws_deployment_subnet_id** (_str_ _,_ _optional_) – The AWS deployment subnet ID.
-  - **availability_zone** (_str_ _,_ _optional_) – The availability zone for the cluster.
-  - **instance_role** ([_InstanceRole_](#bodosdk.models.instance_role.InstanceRole) _|_ _Dict_ _,_ _optional_) – The instance role or a custom role configuration.
-  - **custom_tags** (_Dict_ _,_ _optional_) – Custom tags to assign to the cluster resources.
-- **Returns:**
+* **Parameters:**
+  * **name** (*str*) – The name of the cluster.
+  * **instance_type** (*str* *,* *optional*) – The type of instance to use for the cluster nodes.
+  * **workers_quantity** (*int* *,* *optional*) – The number of worker nodes in the cluster.
+  * **description** (*str* *,* *optional*) – A description of the cluster.
+  * **bodo_version** (*str* *,* *optional*) – The Bodo version to use for the cluster.
+  * **auto_stop** (*int* *,* *optional*) – The auto-stop time in minutes for the cluster.
+  * **auto_pause** (*int* *,* *optional*) – The auto-pause time in minutes for the cluster.
+  * **image_id** (*str* *,* *optional*) – The ID of the image to use for the cluster.
+  * **accelerated_networking** (*bool* *,* *optional*) – Whether to use accelerated networking.
+  * **auto_az** (*bool* *,* *optional*) – Whether to automatically select the availability zone.
+  * **use_spot_instance** (*bool* *,* *optional*) – Whether to use spot instances for the cluster.
+  * **aws_deployment_subnet_id** (*str* *,* *optional*) – The AWS deployment subnet ID.
+  * **availability_zone** (*str* *,* *optional*) – The availability zone for the cluster.
+  * **instance_role** ([*InstanceRole*](#bodosdk.models.instance_role.InstanceRole) *|* *Dict* *,* *optional*) – The instance role or a custom role configuration.
+  * **custom_tags** (*Dict* *,* *optional*) – Custom tags to assign to the cluster resources.
+* **Returns:**
   The created Cluster object.
-- **Return type:**
+* **Return type:**
   [Cluster](#bodosdk.models.cluster.Cluster)
 
 #### get(id: str)
 
 Retrieves a cluster by its ID.
 
-- **Parameters:**
-  **id** (_str_) – The ID of the cluster to retrieve.
-- **Returns:**
+* **Parameters:**
+  **id** (*str*) – The ID of the cluster to retrieve.
+* **Returns:**
   The retrieved Cluster object.
-- **Return type:**
+* **Return type:**
   [Cluster](#bodosdk.models.cluster.Cluster)
 
 #### get_bodo_versions()
 
 Retrieves a list of available Bodo versions.
 
-- **Returns:**
+* **Returns:**
   A list of available Bodo versions.
-- **Return type:**
+* **Return type:**
   List[str]
 
 #### get_images()
 
 Retrieves a list of available images.
 
-- **Returns:**
+* **Returns:**
   A list of image IDs available for clusters.
-- **Return type:**
+* **Return type:**
   List[str]
 
 #### get_instance_types()
 
 Retrieves list of all supported instance types
 
-- **Returns:**
+* **Returns:**
   List[InstanceType]
 
-#### _property_ latest*bodo_version *: str\_
+#### *property* latest_bodo_version *: str*
 
 Retrieves the latest Bodo version available.
 
-- **Returns:**
+* **Returns:**
   The latest Bodo version.
-- **Return type:**
+* **Return type:**
   str
 
 #### list(filters: Dict | [ClusterFilter](#bodosdk.models.cluster.ClusterFilter) | None = None, order: Dict | None = None)
 
 Lists clusters based on the provided filters and order.
 
-- **Parameters:**
-  - **filters** (_Dict_ _|_ [_ClusterFilter_](#bodosdk.models.cluster.ClusterFilter) _,_ _optional_) – The filters to apply to the cluster listing.
-  - **order** (_Dict_ _,_ _optional_) – The order in which to list the clusters.
-- **Returns:**
+* **Parameters:**
+  * **filters** (*Dict* *|* [*ClusterFilter*](#bodosdk.models.cluster.ClusterFilter) *,* *optional*) – The filters to apply to the cluster listing.
+  * **order** (*Dict* *,* *optional*) – The order in which to list the clusters.
+* **Returns:**
   A list of clusters matching the criteria.
-- **Return type:**
+* **Return type:**
   [ClusterList](#bodosdk.models.cluster.ClusterList)
 
 #### pause(id: str, wait=False)
 
 Pauses the specified cluster.
 
-- **Parameters:**
-  **id** (_str_) – The ID of the cluster to pause.
-- **Returns:**
+* **Parameters:**
+  **id** (*str*) – The ID of the cluster to pause.
+* **Returns:**
   The paused Cluster object.
-- **Return type:**
+* **Return type:**
   [Cluster](#bodosdk.models.cluster.Cluster)
 
 #### remove(id: str, wait=False)
 
 Removes the specified cluster.
 
-- **Parameters:**
-  **id** (_str_) – The ID of the cluster to remove.
-- **Returns:**
+* **Parameters:**
+  **id** (*str*) – The ID of the cluster to remove.
+* **Returns:**
   None
 
 #### resume(id: str, wait=False)
 
 Resumes the specified paused cluster.
 
-- **Parameters:**
-  **id** (_str_) – The ID of the cluster to resume.
-- **Returns:**
+* **Parameters:**
+  **id** (*str*) – The ID of the cluster to resume.
+* **Returns:**
   The resumed Cluster object.
-- **Return type:**
+* **Return type:**
   [Cluster](#bodosdk.models.cluster.Cluster)
 
 #### scale(id: str, new_size: int)
 
 Scales the specified cluster to the new size.
 
-- **Parameters:**
-  - **id** (_str_) – The ID of the cluster to scale.
-  - **new_size** (_int_) – The new size for the cluster in terms of the number of worker nodes.
-- **Returns:**
+* **Parameters:**
+  * **id** (*str*) – The ID of the cluster to scale.
+  * **new_size** (*int*) – The new size for the cluster in terms of the number of worker nodes.
+* **Returns:**
   The scaled Cluster object.
-- **Return type:**
+* **Return type:**
   [Cluster](#bodosdk.models.cluster.Cluster)
 
 #### start(id: str, wait=False)
 
 Starts the specified stopped cluster.
 
-- **Parameters:**
-  **id** (_str_) – The ID of the cluster to start.
-- **Returns:**
+* **Parameters:**
+  **id** (*str*) – The ID of the cluster to start.
+* **Returns:**
   The started Cluster object.
-- **Return type:**
+* **Return type:**
   [Cluster](#bodosdk.models.cluster.Cluster)
 
 #### stop(id: str, wait=False)
 
 Stops the specified cluster.
 
-- **Parameters:**
-  **id** (_str_) – The ID of the cluster to stop.
-- **Returns:**
+* **Parameters:**
+  **id** (*str*) – The ID of the cluster to stop.
+* **Returns:**
   The stopped Cluster object.
-- **Return type:**
+* **Return type:**
   [Cluster](#bodosdk.models.cluster.Cluster)
 
 #### update(id: str, name: str | None = None, description: str | None = None, auto_stop: int | None = None, auto_pause: int | None = None, workers_quantity: int | None = None, instance_role: [InstanceRole](#bodosdk.models.instance_role.InstanceRole) | Dict | None = None, instance_type: str | None = None, bodo_version: str | None = None, auto_az: bool | None = None, availability_zone: str | None = None, custom_tags: Dict | None = None)
 
 Updates the specified cluster with the given configuration.
 
-- **Parameters:**
-  - **id** (_str_) – The ID of the cluster to update.
-  - **name** (_str_ _,_ _optional_) – The new name for the cluster.
-  - **description** (_str_ _,_ _optional_) – A new description for the cluster.
-  - **auto_stop** (_int_ _,_ _optional_) – The new auto-stop time in minutes.
-  - **auto_pause** (_int_ _,_ _optional_) – The new auto-pause time in minutes.
-  - **workers_quantity** (_int_ _,_ _optional_) – The new number of worker nodes.
-  - **instance_role** ([_InstanceRole_](#bodosdk.models.instance_role.InstanceRole) _|_ _Dict_ _,_ _optional_) – The new instance role or custom role configuration.
-  - **instance_type** (_str_ _,_ _optional_) – The new instance type for the cluster nodes.
-  - **bodo_version** (_str_ _,_ _optional_) – The new Bodo version for the cluster.
-  - **auto_az** (_bool_ _,_ _optional_) – Whether to automatically select the availability zone.
-  - **availability_zone** (_str_ _,_ _optional_) – The new availability zone for the cluster.
-  - **custom_tags** (_Dict_ _,_ _optional_) – New custom tags for the cluster resources.
-- **Returns:**
+* **Parameters:**
+  * **id** (*str*) – The ID of the cluster to update.
+  * **name** (*str* *,* *optional*) – The new name for the cluster.
+  * **description** (*str* *,* *optional*) – A new description for the cluster.
+  * **auto_stop** (*int* *,* *optional*) – The new auto-stop time in minutes.
+  * **auto_pause** (*int* *,* *optional*) – The new auto-pause time in minutes.
+  * **workers_quantity** (*int* *,* *optional*) – The new number of worker nodes.
+  * **instance_role** ([*InstanceRole*](#bodosdk.models.instance_role.InstanceRole) *|* *Dict* *,* *optional*) – The new instance role or custom role configuration.
+  * **instance_type** (*str* *,* *optional*) – The new instance type for the cluster nodes.
+  * **bodo_version** (*str* *,* *optional*) – The new Bodo version for the cluster.
+  * **auto_az** (*bool* *,* *optional*) – Whether to automatically select the availability zone.
+  * **availability_zone** (*str* *,* *optional*) – The new availability zone for the cluster.
+  * **custom_tags** (*Dict* *,* *optional*) – New custom tags for the cluster resources.
+* **Returns:**
   The updated Cluster object.
-- **Return type:**
+* **Return type:**
   [Cluster](#bodosdk.models.cluster.Cluster)
 
 #### wait_for_status(id: str, statuses: List, timeout: int | None = 300, tick: int | None = 30)
 
 Waits for the specified cluster to reach any of the given statuses within the timeout period.
 
-- **Parameters:**
-  - **id** (_str_) – The ID of the cluster to monitor.
-  - **statuses** (_List_) – The list of statuses to wait for.
-  - **timeout** (_int_ _,_ _optional_) – The timeout period in seconds.
-  - **tick** (_int_ _,_ _optional_) – The interval in seconds between status checks.
-- **Returns:**
+* **Parameters:**
+  * **id** (*str*) – The ID of the cluster to monitor.
+  * **statuses** (*List*) – The list of statuses to wait for.
+  * **timeout** (*int* *,* *optional*) – The timeout period in seconds.
+  * **tick** (*int* *,* *optional*) – The interval in seconds between status checks.
+* **Returns:**
   The Cluster object if it reaches the desired status within the timeout period.
-- **Return type:**
+* **Return type:**
   [Cluster](#bodosdk.models.cluster.Cluster)
 
 <a id="module-bodosdk.clients.instance_role"></a>
 
-### _class_ bodosdk.clients.instance_role.InstanceRoleClient(workspace_client: IBodoWorkspaceClient)
+### *class* bodosdk.clients.instance_role.InstanceRoleClient(workspace_client: IBodoWorkspaceClient)
 
 Bases: `IInstanceRoleClient`
 
-#### _property_ InstanceRole _: [InstanceRole](#bodosdk.models.instance_role.InstanceRole)_
+#### *property* InstanceRole *: [InstanceRole](#bodosdk.models.instance_role.InstanceRole)*
 
-#### _property_ InstanceRoleList _: [InstanceRoleList](#bodosdk.models.instance_role.InstanceRoleList)_
+#### *property* InstanceRoleList *: [InstanceRoleList](#bodosdk.models.instance_role.InstanceRoleList)*
 
 #### create(role_arn: str, description: str, name: str = None)
 
 #### delete(id: str)
 
 #### get(id: str)
 
 #### list(filters: Dict | [InstanceRoleFilter](#bodosdk.models.instance_role.InstanceRoleFilter) | None = None, order: Dict | None = None)
 
 <a id="module-bodosdk.clients.job"></a>
 
-### _class_ bodosdk.clients.job.JobClient(workspace_client: IBodoWorkspaceClient)
+### *class* bodosdk.clients.job.JobClient(workspace_client: IBodoWorkspaceClient)
 
 Bases: `IJobClient`
 
-#### _property_ JobRun _: [JobRun](#bodosdk.models.job.JobRun)_
+#### *property* JobRun *: [JobRun](#bodosdk.models.job.JobRun)*
 
-#### _property_ JobRunList _: [JobRunList](#bodosdk.models.job.JobRunList)_
+#### *property* JobRunList *: [JobRunList](#bodosdk.models.job.JobRunList)*
 
 #### cancel_job(id: str)
 
 #### cancel_jobs(filters: Dict | [JobFilter](#bodosdk.models.job.JobFilter) | None = None)
 
 #### get(id: str)
 
@@ -867,47 +867,47 @@
 
 #### run_sql_query(template_id: str = None, catalog: str = None, sql_query: str = None, cluster: dict | ICluster = None, name: str = None, args: dict = None, timeout: int = None, num_retries: int = None, delay_between_retries: int = None, retry_on_timeout: bool = None)
 
 #### wait_for_status(id: str, statuses: List[str], timeout: int = 3600, tick: int = 30)
 
 <a id="module-bodosdk.clients.job_tpl"></a>
 
-### _class_ bodosdk.clients.job_tpl.JobTemplateClient(workspace_client: IBodoWorkspaceClient)
+### *class* bodosdk.clients.job_tpl.JobTemplateClient(workspace_client: IBodoWorkspaceClient)
 
 Bases: `IJobTemplateClient`
 
-#### _property_ JobTemplate _: [JobTemplate](#bodosdk.models.job.JobTemplate)_
+#### *property* JobTemplate *: [JobTemplate](#bodosdk.models.job.JobTemplate)*
 
-#### _property_ JobTemplateList _: [JobTemplateList](#bodosdk.models.job.JobTemplateList)_
+#### *property* JobTemplateList *: [JobTemplateList](#bodosdk.models.job.JobTemplateList)*
 
 #### create(name: str = None, description: str = None, cluster: dict | ICluster = None, code_type: str = None, source: dict | IS3Source | IGitRepoSource | IWorkspaceSource | ITextSource = None, exec_file: str = None, exec_text: str = None, args: dict | str = None, env_vars: dict = None, timeout: int = None, num_retries: int = None, delay_between_retries: int = None, retry_on_timeout: bool = None, catalog: str = None)
 
 #### get(id: str)
 
 #### list(filters: Dict = None)
 
 #### remove(id: str)
 
 <a id="module-bodosdk.clients.organization"></a>
 
-### _class_ bodosdk.clients.organization.BodoOrganizationClient(client_id=None, secret_key=None, api_url='https://api.bodo.ai/api', auth_url='https://auth.bodo.ai', print_logs=False)
+### *class* bodosdk.clients.organization.BodoOrganizationClient(client_id=None, secret_key=None, api_url='https://api.bodo.ai/api', auth_url='https://auth.bodo.ai', print_logs=False)
 
 Bases: `IBodoOrganizationClient`
 
-#### _property_ AwsCloudConfig _: [AwsCloudConfig](#bodosdk.models.cloud_config.AwsCloudConfig)_
+#### *property* AwsCloudConfig *: [AwsCloudConfig](#bodosdk.models.cloud_config.AwsCloudConfig)*
 
-#### _property_ AzureCloudConfig _: [AzureCloudConfig](#bodosdk.models.cloud_config.AzureCloudConfig)_
+#### *property* AzureCloudConfig *: [AzureCloudConfig](#bodosdk.models.cloud_config.AzureCloudConfig)*
 
-#### _property_ CloudConfig _: [CloudConfigBase](#bodosdk.models.cloud_config.CloudConfigBase)_
+#### *property* CloudConfig *: [CloudConfigBase](#bodosdk.models.cloud_config.CloudConfigBase)*
 
-#### _property_ CloudConfigList _: [CloudConfigList](#bodosdk.models.cloud_config.CloudConfigList)_
+#### *property* CloudConfigList *: [CloudConfigList](#bodosdk.models.cloud_config.CloudConfigList)*
 
-#### _property_ Workspace _: [Workspace](#bodosdk.models.workspace.Workspace)_
+#### *property* Workspace *: [Workspace](#bodosdk.models.workspace.Workspace)*
 
-#### _property_ WorkspaceList _: [WorkspaceList](#bodosdk.models.workspace.WorkspaceList)_
+#### *property* WorkspaceList *: [WorkspaceList](#bodosdk.models.workspace.WorkspaceList)*
 
 #### create_workspace(name: str, region: str, storage_endpoint_enabled: bool, cloud_config_id: str = None, vpc_id: str | None = None, public_subnets_ids: List[str] | None = None, private_subnets_ids: List[str] | None = None, custom_tags: dict | None = None)
 
 #### delete_workspace(id)
 
 #### get_cloud_config(id)
 
@@ -915,2277 +915,2271 @@
 
 #### list_cloud_configs(filters: dict | None = None)
 
 #### list_workspaces(filters: [WorkspaceFilter](#bodosdk.models.workspace.WorkspaceFilter) | dict | None = None)
 
 <a id="module-bodosdk.clients.workspace"></a>
 
-### _class_ bodosdk.clients.workspace.BodoWorkspaceClient(client_id=None, secret_key=None, api_url='https://api.bodo.ai/api', auth_url='https://auth.bodo.ai', print_logs=False)
+### *class* bodosdk.clients.workspace.BodoWorkspaceClient(client_id=None, secret_key=None, api_url='https://api.bodo.ai/api', auth_url='https://auth.bodo.ai', print_logs=False)
 
 Bases: `IBodoWorkspaceClient`
 
-#### ClusterClient _: IClusterClient_
+#### ClusterClient *: IClusterClient*
 
-#### JobClient _: IJobClient_
+#### JobClient *: IJobClient*
 
-#### JobTemplateClient _: IJobTemplateClient_
+#### JobTemplateClient *: IJobTemplateClient*
 
-#### _property_ workspace*data *: IWorkspace\_
+#### *property* workspace_data *: IWorkspace*
 
-#### _property_ workspace*id *: str\_
+#### *property* workspace_id *: str*
 
 <a id="module-bodosdk.models.catalog"></a>
 
-### _class_ bodosdk.models.catalog.Catalog(workspace_client: IBodoWorkspaceClient = None, \*, uuid: str | None = None, name: str | None = None, description: str | None = None, catalogType: str | None = None, details: [SnowflakeDetails](#bodosdk.models.catalog.SnowflakeDetails) | dict | None = None)
+### *class* bodosdk.models.catalog.Catalog(workspace_client: IBodoWorkspaceClient = None, \*, uuid: str | None = None, name: str | None = None, description: str | None = None, catalogType: str | None = None, details: [SnowflakeDetails](#bodosdk.models.catalog.SnowflakeDetails) | dict | None = None)
 
 Bases: `SDKBaseModel`, `ICatalog`
 
 #### delete()
 
-### _class_ bodosdk.models.catalog.CatalogFilter(\*, names: List[str] | None = None, ids: List[str] | None = None)
+### *class* bodosdk.models.catalog.CatalogFilter(\*, names: List[str] | None = None, ids: List[str] | None = None)
 
 Bases: `SDKBaseModel`, `ICatalogFilter`
 
-#### ids _: List[str] | None_
+#### ids *: List[str] | None*
 
-#### names _: List[str] | None_
+#### names *: List[str] | None*
 
-### _class_ bodosdk.models.catalog.CatalogList(workspace_client: IBodoWorkspaceClient = None, \*, page: int | None = 0, pageSize: int | None = 10, total: int | None = None, order: dict | None = None, filters: dict | [CatalogFilter](#bodosdk.models.catalog.CatalogFilter) | None = None)
+### *class* bodosdk.models.catalog.CatalogList(workspace_client: IBodoWorkspaceClient = None, \*, page: int | None = 0, pageSize: int | None = 10, total: int | None = None, order: dict | None = None, filters: dict | [CatalogFilter](#bodosdk.models.catalog.CatalogFilter) | None = None)
 
 Bases: `ICatalogList`, `SDKBaseModel`
 
-#### _class_ Config
+#### *class* Config
 
 Bases: `object`
 
 Configuration for Pydantic models.
 [https://docs.pydantic.dev/latest/api/config/](https://docs.pydantic.dev/latest/api/config/)
 
-#### allow*population_by_field_name *= True\_
+#### allow_population_by_field_name *= True*
 
-#### extra _= 'forbid'_
+#### extra *= 'forbid'*
 
 #### delete()
 
-#### filters _: dict | [CatalogFilter](#bodosdk.models.catalog.CatalogFilter) | None_
+#### filters *: dict | [CatalogFilter](#bodosdk.models.catalog.CatalogFilter) | None*
 
-#### order _: dict | None_
+#### order *: dict | None*
 
-#### page _: int | None_
+#### page *: int | None*
 
-#### page*size *: int | None\_
+#### page_size *: int | None*
 
-#### total _: int | None_
+#### total *: int | None*
 
-### _class_ bodosdk.models.catalog.SnowflakeDetails(\*, port: int | None = None, db_schema: str | None = None, database: str | None = None, userRole: str | None = None, username: str | None = None, warehouse: str | None = None, accountName: str | None = None, password: str | None = None)
+### *class* bodosdk.models.catalog.SnowflakeDetails(\*, port: int | None = None, db_schema: str | None = None, database: str | None = None, userRole: str | None = None, username: str | None = None, warehouse: str | None = None, accountName: str | None = None, password: str | None = None)
 
 Bases: `SDKBaseModel`
 
-#### account*name *: str | None\_
+#### account_name *: str | None*
 
-#### database _: str | None_
+#### database *: str | None*
 
-#### db*schema *: str | None\_
+#### db_schema *: str | None*
 
-#### password _: str | None_
+#### password *: str | None*
 
-#### port _: int | None_
+#### port *: int | None*
 
-#### user*role *: str | None\_
+#### user_role *: str | None*
 
-#### username _: str | None_
+#### username *: str | None*
 
-#### warehouse _: str | None_
+#### warehouse *: str | None*
 
 <a id="module-bodosdk.models.cloud_config"></a>
 
-### _class_ bodosdk.models.cloud_config.AwsCloudConfig(org_client: IBodoOrganizationClient = None, \*, cloudProvider: str | None = None, name: str | None = None, status: str | None = None, organizationUUID: str | None = None, customTags: dict | None = None, uuid: str | UUID | None = None, awsProviderData: [AwsProviderData](#bodosdk.models.cloud_config.AwsProviderData) | None = None)
+### *class* bodosdk.models.cloud_config.AwsCloudConfig(org_client: IBodoOrganizationClient = None, \*, cloudProvider: str | None = None, name: str | None = None, status: str | None = None, organizationUUID: str | None = None, customTags: dict | None = None, uuid: str | UUID | None = None, awsProviderData: [AwsProviderData](#bodosdk.models.cloud_config.AwsProviderData) | None = None)
 
 Bases: [`CloudConfigBase`](#bodosdk.models.cloud_config.CloudConfigBase), `IAwsCloudConfig`
 
-#### data _: [AwsProviderData](#bodosdk.models.cloud_config.AwsProviderData) | None_
+#### data *: [AwsProviderData](#bodosdk.models.cloud_config.AwsProviderData) | None*
 
-### _class_ bodosdk.models.cloud_config.AwsProviderData(\*, roleArn: str | None = None, tfBucketName: str | None = None, tfDynamoDbTableName: str | None = None, tfBackendRegion: str | None = None, externalId: str | None = None, accountId: str | None = None)
+### *class* bodosdk.models.cloud_config.AwsProviderData(\*, roleArn: str | None = None, tfBucketName: str | None = None, tfDynamoDbTableName: str | None = None, tfBackendRegion: str | None = None, externalId: str | None = None, accountId: str | None = None)
 
 Bases: `SDKBaseModel`, `IAwsProviderData`
 
-#### account*id *: str | None\_
+#### account_id *: str | None*
 
-#### external*id *: str | None\_
+#### external_id *: str | None*
 
-#### role*arn *: str | None\_
+#### role_arn *: str | None*
 
-#### tf*backend_region *: str | None\_
+#### tf_backend_region *: str | None*
 
-#### tf*bucket_name *: str | None\_
+#### tf_bucket_name *: str | None*
 
-#### tf*dynamo_db_table_name *: str | None\_
+#### tf_dynamo_db_table_name *: str | None*
 
-### _class_ bodosdk.models.cloud_config.AzureCloudConfig(org_client: IBodoOrganizationClient = None, \*, cloudProvider: str | None = None, name: str | None = None, status: str | None = None, organizationUUID: str | None = None, customTags: dict | None = None, uuid: str | UUID | None = None, azureProviderData: [AzureProviderData](#bodosdk.models.cloud_config.AzureProviderData) | None = None)
+### *class* bodosdk.models.cloud_config.AzureCloudConfig(org_client: IBodoOrganizationClient = None, \*, cloudProvider: str | None = None, name: str | None = None, status: str | None = None, organizationUUID: str | None = None, customTags: dict | None = None, uuid: str | UUID | None = None, azureProviderData: [AzureProviderData](#bodosdk.models.cloud_config.AzureProviderData) | None = None)
 
 Bases: [`CloudConfigBase`](#bodosdk.models.cloud_config.CloudConfigBase), `IAzureCloudConfig`
 
-#### data _: [AzureProviderData](#bodosdk.models.cloud_config.AzureProviderData) | None_
+#### data *: [AzureProviderData](#bodosdk.models.cloud_config.AzureProviderData) | None*
 
-### _class_ bodosdk.models.cloud_config.AzureProviderData(\*, tfBackendRegion: str | None = None, resourceGroup: str | None = None, subscriptionId: str | None = None, tenantId: str | None = None, tfStorageAccountName: str | None = None, applicationId: str | None = None)
+### *class* bodosdk.models.cloud_config.AzureProviderData(\*, tfBackendRegion: str | None = None, resourceGroup: str | None = None, subscriptionId: str | None = None, tenantId: str | None = None, tfStorageAccountName: str | None = None, applicationId: str | None = None)
 
 Bases: `SDKBaseModel`, `IAzureProviderData`
 
-#### application*id *: str | None\_
+#### application_id *: str | None*
 
-#### resource*group *: str | None\_
+#### resource_group *: str | None*
 
-#### subscription*id *: str | None\_
+#### subscription_id *: str | None*
 
-#### tenant*id *: str | None\_
+#### tenant_id *: str | None*
 
-#### tf*backend_region *: str | None\_
+#### tf_backend_region *: str | None*
 
-#### tf*storage_account_name *: str | None\_
+#### tf_storage_account_name *: str | None*
 
-### _class_ bodosdk.models.cloud_config.CloudConfigBase(org_client: IBodoOrganizationClient = None, \*, cloudProvider: str | None = None, name: str | None = None, status: str | None = None, organizationUUID: str | None = None, customTags: dict | None = None, uuid: str | UUID | None = None, data: [AwsProviderData](#bodosdk.models.cloud_config.AwsProviderData) | [AzureProviderData](#bodosdk.models.cloud_config.AzureProviderData) | None = None)
+### *class* bodosdk.models.cloud_config.CloudConfigBase(org_client: IBodoOrganizationClient = None, \*, cloudProvider: str | None = None, name: str | None = None, status: str | None = None, organizationUUID: str | None = None, customTags: dict | None = None, uuid: str | UUID | None = None, data: [AwsProviderData](#bodosdk.models.cloud_config.AwsProviderData) | [AzureProviderData](#bodosdk.models.cloud_config.AzureProviderData) | None = None)
 
 Bases: `SDKBaseModel`, `ICloudConfig`
 
-#### cloud*provider *: str | None\_
+#### cloud_provider *: str | None*
 
-#### custom*tags *: dict | None\_
+#### custom_tags *: dict | None*
 
-#### data _: [AwsProviderData](#bodosdk.models.cloud_config.AwsProviderData) | [AzureProviderData](#bodosdk.models.cloud_config.AzureProviderData) | None_
+#### data *: [AwsProviderData](#bodosdk.models.cloud_config.AwsProviderData) | [AzureProviderData](#bodosdk.models.cloud_config.AzureProviderData) | None*
 
 #### delete()
 
-#### _property_ id
+#### *property* id
 
-#### name _: str | None_
+#### name *: str | None*
 
-#### organization*uuid *: str | None\_
+#### organization_uuid *: str | None*
 
-#### status _: str | None_
+#### status *: str | None*
 
-#### uuid _: str | UUID | None_
+#### uuid *: str | UUID | None*
 
-### _class_ bodosdk.models.cloud_config.CloudConfigList(org_client: IBodoOrganizationClient = None, \*, page: int | None = 0, pageSize: int | None = 10, total: int | None = None, order: dict | None = None, filters: dict | None = None)
+### *class* bodosdk.models.cloud_config.CloudConfigList(org_client: IBodoOrganizationClient = None, \*, page: int | None = 0, pageSize: int | None = 10, total: int | None = None, order: dict | None = None, filters: dict | None = None)
 
 Bases: `ICloudConfigList`, `SDKBaseModel`
 
-#### _class_ Config
+#### *class* Config
 
 Bases: `object`
 
 Configuration for Pydantic models.
 [https://docs.pydantic.dev/latest/api/config/](https://docs.pydantic.dev/latest/api/config/)
 
-#### allow*population_by_field_name *= True\_
+#### allow_population_by_field_name *= True*
 
-#### extra _= 'forbid'_
+#### extra *= 'forbid'*
 
 #### delete()
 
-#### filters _: dict | None_
+#### filters *: dict | None*
 
-#### order _: dict | None_
+#### order *: dict | None*
 
-#### page _: int | None_
+#### page *: int | None*
 
-#### page*size *: int | None\_
+#### page_size *: int | None*
 
-#### total _: int | None_
+#### total *: int | None*
 
 <a id="module-bodosdk.models.cluster"></a>
 
-### _class_ bodosdk.models.cluster.BodoImage(\*, image_id: str, bodo_version: str)
+### *class* bodosdk.models.cluster.BodoImage(\*, image_id: str, bodo_version: str)
 
 Bases: `SDKBaseModel`
 
 Represents an image configuration for Bodo, encapsulating the image ID and the specific Bodo version.
 
 This class is a data model that holds information about a Bodo environment image.
 
 #### image_id
 
 The unique identifier for the Bodo image.
 
-- **Type:**
+* **Type:**
   str
 
 #### bodo_version
 
 The version of Bodo used in the image.
 
-- **Type:**
+* **Type:**
   str
 
-#### bodo*version *: str\_
+#### bodo_version *: str*
 
-#### image*id *: str\_
+#### image_id *: str*
 
-### _class_ bodosdk.models.cluster.Cluster(workspace_client: IBodoWorkspaceClient = None, \*, name: str | None = None, uuid: str | None = None, status: str | None = None, description: str | None = None, instanceType: str | None = None, workersQuantity: int | None = None, autoStop: int | None = None, autoPause: int | None = None, bodoVersion: str | None = None, imageId: str | None = None, coresPerWorker: int | None = None, acceleratedNetworking: bool | None = None, createdAt: datetime | None = None, updatedAt: datetime | None = None, isJobDedicated: bool | None = None, autoAZ: bool | None = None, useSpotInstance: bool | None = None, lastKnownActivity: datetime | None = None, inStateSince: datetime | None = None, clusterAgentVersion: str | None = None, clusterInitStatus: str | None = None, clusterHealthStatus: str | None = None, primaryAgentIP: str | None = None, awsDeploymentSubnetId: str | None = None, nodeMetadata: List[[NodeMetadata](#bodosdk.models.cluster.NodeMetadata)] | None = None, availabilityZone: str | None = None, instanceRole: [InstanceRole](#bodosdk.models.instance_role.InstanceRole) | None = None, workspace: dict | None = None, autoscalingIdentifier: str | None = None, lastAsgActivityId: str | None = None, nodesIp: List[str] | None = None, customTags: Dict | None = None)
+### *class* bodosdk.models.cluster.Cluster(workspace_client: IBodoWorkspaceClient = None, \*, name: str | None = None, uuid: str | None = None, status: str | None = None, description: str | None = None, instanceType: str | None = None, workersQuantity: int | None = None, autoStop: int | None = None, autoPause: int | None = None, bodoVersion: str | None = None, imageId: str | None = None, coresPerWorker: int | None = None, acceleratedNetworking: bool | None = None, createdAt: datetime | None = None, updatedAt: datetime | None = None, isJobDedicated: bool | None = None, autoAZ: bool | None = None, useSpotInstance: bool | None = None, lastKnownActivity: datetime | None = None, inStateSince: datetime | None = None, clusterAgentVersion: str | None = None, clusterInitStatus: str | None = None, clusterHealthStatus: str | None = None, primaryAgentIP: str | None = None, awsDeploymentSubnetId: str | None = None, nodeMetadata: List[[NodeMetadata](#bodosdk.models.cluster.NodeMetadata)] | None = None, availabilityZone: str | None = None, instanceRole: [InstanceRole](#bodosdk.models.instance_role.InstanceRole) | None = None, workspace: dict | None = None, autoscalingIdentifier: str | None = None, lastAsgActivityId: str | None = None, nodesIp: List[str] | None = None, customTags: Dict | None = None)
 
 Bases: `SDKBaseModel`, `ICluster`
 
 Represents a cluster in the SDK model, encapsulating various properties and operations
 related to a compute cluster.
 
 #### name
 
 The name of the cluster.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### uuid
 
 The unique identifier of the cluster.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### status
 
 The current status of the cluster (e.g., ‘RUNNING’, ‘STOPPED’).
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### description
 
 A description of the cluster.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### instance_type
 
 The type of instances used in the cluster (e.g., ‘c5.large’).
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### workers_quantity
 
 The number of worker nodes in the cluster.
 
-- **Type:**
+* **Type:**
   Optional[int]
 
 #### auto_stop
 
 The auto-stop configuration in minutes.
 The cluster automatically stops when idle for this duration.
 
-- **Type:**
+* **Type:**
   Optional[int]
 
 #### auto_pause
 
 The auto-pause configuration in minutes.
 The cluster automatically pauses when idle for this duration.
 
-- **Type:**
+* **Type:**
   Optional[int]
 
 #### bodo_version
 
 The version of Bodo being used in the cluster.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### image_id
 
 The ID of the image used for the cluster’s instances.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### cores_per_worker
 
 The number of CPU cores per worker node.
 
-- **Type:**
+* **Type:**
   Optional[int]
 
 #### accelerated_networking
 
 Whether accelerated networking is enabled.
 
-- **Type:**
+* **Type:**
   Optional[bool]
 
 #### created_at
 
 The creation timestamp of the cluster.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### updated_at
 
 The last update timestamp of the cluster.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### is_job_dedicated
 
 Whether the cluster is dedicated to a specific job.
 
-- **Type:**
+* **Type:**
   Optional[bool]
 
 #### auto_az
 
 Whether automatic availability zone selection is enabled.
 
-- **Type:**
+* **Type:**
   Optional[bool]
 
 #### use_spot_instance
 
 Whether spot instances are used for the cluster.
 
-- **Type:**
+* **Type:**
   Optional[bool]
 
 #### last_known_activity
 
 The last known activity timestamp of the cluster.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### in_state_since
 
 The timestamp since the cluster has been in its current state.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### cluster_agent_version
 
 The version of the cluster agent.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### cluster_init_status
 
 The initialization status of the cluster.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### cluster_health_status
 
 The health status of the cluster.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### primary_agent_ip
 
 The IP address of the primary agent in the cluster.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### aws_deployment_subnet_id
 
 The subnet ID used for deploying AWS resources.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### node_metadata
 
 Metadata information for each node in the cluster.
 
-- **Type:**
+* **Type:**
   Optional[List[[NodeMetadata](#bodosdk.models.cluster.NodeMetadata)]]
 
 #### availability_zone
 
 The AWS availability zone in which the cluster is located.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### instance_role
 
 The IAM role used by instances in the cluster.
 
-- **Type:**
+* **Type:**
   Optional[[InstanceRole](#bodosdk.models.instance_role.InstanceRole)]
 
 #### workspace
 
 A dictionary containing workspace-related information for the cluster.
 
-- **Type:**
+* **Type:**
   Optional[dict]
 
 #### autoscaling_identifier
 
 The identifier for autoscaling configuration.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### last_asg_activity_id
 
 The identifier of the last activity in the autoscaling group.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### nodes_ip
 
 A list of IP addresses for the nodes in the cluster.
 
-- **Type:**
+* **Type:**
   Optional[List[str]]
 
-#### accelerated*networking *: bool | None\_
+#### accelerated_networking *: bool | None*
 
-#### auto*az *: bool | None\_
+#### auto_az *: bool | None*
 
-#### auto*pause *: int | None\_
+#### auto_pause *: int | None*
 
-#### auto*stop *: int | None\_
+#### auto_stop *: int | None*
 
-#### autoscaling*identifier *: str | None\_
+#### autoscaling_identifier *: str | None*
 
-#### availability*zone *: str | None\_
+#### availability_zone *: str | None*
 
-#### aws*deployment_subnet_id *: str | None\_
+#### aws_deployment_subnet_id *: str | None*
 
-#### bodo*version *: str | None\_
+#### bodo_version *: str | None*
 
 #### cancel_jobs()
 
 Cancels all jobs associated with the cluster.
 
-- **Returns:**
+* **Returns:**
   The Cluster instance.
 
-#### cluster*agent_version *: str | None\_
+#### cluster_agent_version *: str | None*
 
-#### cluster*health_status *: str | None\_
+#### cluster_health_status *: str | None*
 
-#### cluster*init_status *: str | None\_
+#### cluster_init_status *: str | None*
 
 #### connect(catalog: str)
 
 Establishes a connection to the specified catalog from Cluster.
 
 This method is responsible for creating and returning a new Connection instance based on the provided catalog.
 
 Parameters:
 catalog (str): The name of the catalog to which the connection should be established.
 
 Returns:
 Connection: An instance of Connection initialized with the specified catalog and the current class instance.
 
-#### cores*per_worker *: int | None\_
+#### cores_per_worker *: int | None*
 
-#### created*at *: datetime | None\_
+#### created_at *: datetime | None*
 
-#### custom*tags *: Dict | None\_
+#### custom_tags *: Dict | None*
 
 #### delete(force: bool = False, mark_as_terminated: bool = False, wait: bool = False)
 
 Deletes the cluster, optionally forcing removal or marking as terminated.
 
-- **Parameters:**
-  - **force** – If True, forces the deletion of the cluster.
-  - **mark_as_terminated** – If True, marks the cluster as terminated instead of deleting.
-  - **wait** – If True, waits till cluster will be TERMINATED.
-- **Returns:**
+* **Parameters:**
+  * **force** – If True, forces the deletion of the cluster.
+  * **mark_as_terminated** – If True, marks the cluster as terminated instead of deleting.
+  * **wait** – If True, waits till cluster will be TERMINATED.
+* **Returns:**
   The Cluster instance, potentially updated to reflect its new state.
 
 Handles:
 : ResourceNotFound: Silently if the cluster is already deleted or not found.
 
-#### description _: str | None_
+#### description *: str | None*
 
-#### _property_ id _: str_
+#### *property* id *: str*
 
 The UUID of the cluster.
 
-- **Returns:**
+* **Returns:**
   The UUID string of the cluster.
 
-#### image*id *: str | None\_
+#### image_id *: str | None*
 
-#### in*state_since *: datetime | None\_
+#### in_state_since *: datetime | None*
 
-#### instance*role *: [InstanceRole](#bodosdk.models.instance_role.InstanceRole) | None\_
+#### instance_role *: [InstanceRole](#bodosdk.models.instance_role.InstanceRole) | None*
 
-#### instance*type *: str | None\_
+#### instance_type *: str | None*
 
-#### is*job_dedicated *: bool | None\_
+#### is_job_dedicated *: bool | None*
 
-#### last*asg_activity_id *: str | None\_
+#### last_asg_activity_id *: str | None*
 
-#### last*known_activity *: datetime | None\_
+#### last_known_activity *: datetime | None*
 
-#### name _: str | None_
+#### name *: str | None*
 
-#### node*metadata *: List[[NodeMetadata](#bodosdk.models.cluster.NodeMetadata)] | None\_
+#### node_metadata *: List[[NodeMetadata](#bodosdk.models.cluster.NodeMetadata)] | None*
 
-#### nodes*ip *: List[str] | None\_
+#### nodes_ip *: List[str] | None*
 
 #### pause(wait: bool = False)
 
 Pauses the cluster if it is running.
 
-- **Parameters:**
+* **Parameters:**
   **wait** – If True, waits till cluster will be PAUSED.
-- **Returns:**
+* **Returns:**
   The Cluster instance with updated status.
-- **Raises:**
+* **Raises:**
   **ConflictException** – If the cluster cannot be paused due to its current status.
 
-#### primary*agent_ip *: str | None\_
+#### primary_agent_ip *: str | None*
 
 #### resume(wait: bool = False)
 
 Resumes the cluster if it was paused or stopped.
 
-- **Parameters:**
+* **Parameters:**
   **wait** – If True, waits till cluster will be RUNNING.
-- **Returns:**
+* **Returns:**
   The Cluster instance with updated status.
-- **Raises:**
+* **Raises:**
   **ConflictException** – If the cluster cannot be resumed due to its current status.
 
 #### run_job(template_id: str = None, code_type: str = None, source: dict | IS3Source | IGitRepoSource | IWorkspaceSource | ITextSource = None, exec_file: str = None, args: dict | str = None, env_vars: dict = None, timeout: int = None, num_retries: int = None, delay_between_retries: int = None, retry_on_timeout: bool = None, name: str = None, catalog: str = None)
 
 Submits a batch job for execution using specified configurations and resources.
 
 This method creates and dispatches a job within a computing cluster, allowing for extensive customization of
 execution parameters including source data, runtime environment, and failure handling strategies.
 
-- **Parameters:**
-  - **template_id** (_str_ _,_ _optional_) – Identifier for the job template to use.
-  - **code_type** (_str_ _,_ _optional_) – Type of code to execute (e.g., Python, Java).
-  - **source** (_Union_ _[\*\*dict_ _,_ _IS3Source_ _,_ _IGitRepoSource_ _,_ _IWorkspaceSource_ _,_ _ITextSource_ _]_ _,_ _optional_) – Source of the code to be executed. Can be specified as a dictionary
+* **Parameters:**
+  * **template_id** (*str* *,* *optional*) – Identifier for the job template to use.
+  * **code_type** (*str* *,* *optional*) – Type of code to execute (e.g., Python, Java).
+  * **source** (*Union* *[**dict* *,* *IS3Source* *,* *IGitRepoSource* *,* *IWorkspaceSource* *,* *ITextSource* *]* *,* *optional*) – Source of the code to be executed. Can be specified as a dictionary
     or an instance of one of the predefined source interfaces.
-  - **exec_file** (_str_ _,_ _optional_) – Path to the executable file within the source.
-  - **args** (_Union_ _[\*\*dict_ _,_ _str_ _]_ _,_ _optional_) – Arguments to pass to the executable.
-  - **parameters.** (_Can be a string_ _or_ _a dictionary of_) –
-  - **env_vars** (_dict_ _,_ _optional_) – Environment variables to set for the job.
-  - **timeout** (_int_ _,_ _optional_) – Maximum runtime (in seconds) before the job is terminated.
-  - **num_retries** (_int_ _,_ _optional_) – Number of times to retry the job on failure.
-  - **delay_between_retries** (_int_ _,_ _optional_) – Time to wait between retries.
-  - **retry_on_timeout** (_bool_ _,_ _optional_) – Whether to retry the job if it times out.
-  - **name** (_str_ _,_ _optional_) – Name of the job.
-  - **catalog** (_str_ _,_ _optional_) – Catalog to log the job under.
-- **Returns:**
+  * **exec_file** (*str* *,* *optional*) – Path to the executable file within the source.
+  * **args** (*Union* *[**dict* *,* *str* *]* *,* *optional*) – Arguments to pass to the executable.
+  * **parameters.** (*Can be a string* *or* *a dictionary of*) –
+  * **env_vars** (*dict* *,* *optional*) – Environment variables to set for the job.
+  * **timeout** (*int* *,* *optional*) – Maximum runtime (in seconds) before the job is terminated.
+  * **num_retries** (*int* *,* *optional*) – Number of times to retry the job on failure.
+  * **delay_between_retries** (*int* *,* *optional*) – Time to wait between retries.
+  * **retry_on_timeout** (*bool* *,* *optional*) – Whether to retry the job if it times out.
+  * **name** (*str* *,* *optional*) – Name of the job.
+  * **catalog** (*str* *,* *optional*) – Catalog to log the job under.
+* **Returns:**
   An object representing the submitted job, capable of providing status and results.
-- **Return type:**
+* **Return type:**
   IJobRun
 
 #### run_sql_query(template_id: str = None, catalog: str = None, sql_query: str = None, name: str = None, args: dict = None, timeout: int = None, num_retries: int = None, delay_between_retries: int = None, retry_on_timeout: bool = None)
 
 > Submits an SQL query for execution on the cluster, returning a job run object.
 
 > This method handles the execution of an SQL query within a defined cluster environment.
 > It supports customization of execution parameters such as query arguments,
 > job name, execution timeouts, and retry strategies.
 
 > Parameters:
 > : template_id (str, optional): Identifier for the job template to use.
-> catalog (str, optional): Catalog under which to log the SQL job.
-> sql_query (str, optional): The SQL query string to be executed.
-> name (str, optional): Descriptive name for the SQL job.
-> args (dict, optional): Dictionary of arguments that are passed to the SQL query.
-> timeout (int, optional): Maximum allowable runtime in seconds before the job is terminated.
-> num_retries (int, optional): Number of times the job will be retried on failure.
-> delay_between_retries (int, optional): Interval in seconds between job retries.
-> retry_on_timeout (bool, optional): Whether to retry the job if it times out.
+>   catalog (str, optional): Catalog under which to log the SQL job.
+>   sql_query (str, optional): The SQL query string to be executed.
+>   name (str, optional): Descriptive name for the SQL job.
+>   args (dict, optional): Dictionary of arguments that are passed to the SQL query.
+>   timeout (int, optional): Maximum allowable runtime in seconds before the job is terminated.
+>   num_retries (int, optional): Number of times the job will be retried on failure.
+>   delay_between_retries (int, optional): Interval in seconds between job retries.
+>   retry_on_timeout (bool, optional): Whether to retry the job if it times out.
 
 > Returns:
 > : IJobRun: An object representing the status and result of the executed SQL job.
 
 ```
 `
 ```
 
 #### start(wait: bool = False)
 
 Starts the cluster.
 
-- **Parameters:**
+* **Parameters:**
   **wait** – If True, waits till cluster will be RUNNING.
-- **Returns:**
+* **Returns:**
   The Cluster instance with updated status.
 
-#### status _: str | None_
+#### status *: str | None*
 
 #### stop(wait: bool = False)
 
 Stops the cluster.
 
-- **Parameters:**
+* **Parameters:**
   **wait** – If True, waits till cluster will be STOPPED.
-- **Returns:**
+* **Returns:**
   The Cluster instance with updated status.
 
 #### update(auto_stop: int | None = None, auto_pause: int | None = None, description: str | None = None, name: str | None = None, workers_quantity: int | None = None, instance_role: [InstanceRole](#bodosdk.models.instance_role.InstanceRole) | None = None, instance_type: str | None = None, bodo_version: str | None = None, auto_az: bool | None = None, availability_zone: str | None = None, custom_tags: Dict | None = None)
 
 Updates the cluster’s configuration with the provided values.
 
-- **Parameters:**
-  - **auto_stop** – Optional; configures auto-stop feature.
-  - **auto_pause** – Optional; configures auto-pause feature.
-  - **description** – Optional; updates the cluster’s description.
-  - **name** – Optional; updates the cluster’s name.
-  - **workers_quantity** – Optional; updates the number of workers.
-  - **instance_role** – Optional; updates the instance role.
-  - **instance_type** – Optional; updates the instance type.
-  - **bodo_version** – Optional; updates the Bodo version.
-  - **auto_az** – Optional; enables/disables automatic availability zone selection.
-  - **availability_zone** – Optional; sets a specific availability zone.
-- **Returns:**
+* **Parameters:**
+  * **auto_stop** – Optional; configures auto-stop feature.
+  * **auto_pause** – Optional; configures auto-pause feature.
+  * **description** – Optional; updates the cluster’s description.
+  * **name** – Optional; updates the cluster’s name.
+  * **workers_quantity** – Optional; updates the number of workers.
+  * **instance_role** – Optional; updates the instance role.
+  * **instance_type** – Optional; updates the instance type.
+  * **bodo_version** – Optional; updates the Bodo version.
+  * **auto_az** – Optional; enables/disables automatic availability zone selection.
+  * **availability_zone** – Optional; sets a specific availability zone.
+* **Returns:**
   The updated Cluster instance.
 
-#### updated*at *: datetime | None\_
+#### updated_at *: datetime | None*
 
-#### use*spot_instance *: bool | None\_
+#### use_spot_instance *: bool | None*
 
-#### uuid _: str | None_
+#### uuid *: str | None*
 
 #### wait_for_status(statuses: List[str], timeout: int = 600, tick: int = 30)
 
 Waits for the cluster to reach one of the specified states within a given timeout.
 
-- **Parameters:**
-  - **statuses** – A list of states to wait for.
-  - **timeout** – The maximum time to wait before raising a TimeoutException.
-  - **tick** – The interval between checks.
-- **Returns:**
+* **Parameters:**
+  * **statuses** – A list of states to wait for.
+  * **timeout** – The maximum time to wait before raising a TimeoutException.
+  * **tick** – The interval between checks.
+* **Returns:**
   The Cluster instance, once it has reached one of the desired states.
-- **Raises:**
+* **Raises:**
   **TimeoutException** – If the cluster does not reach a desired state within the timeout.
 
-#### workers*quantity *: int | None\_
+#### workers_quantity *: int | None*
 
-#### workspace _: dict | None_
+#### workspace *: dict | None*
 
-### _class_ bodosdk.models.cluster.ClusterFilter(\*, uuids: List[str] | None = None, clusterNames: List[str] | None = None, statues: List[str] | None = None, tags: Dict | None = None)
+### *class* bodosdk.models.cluster.ClusterFilter(\*, uuids: List[str] | None = None, clusterNames: List[str] | None = None, statues: List[str] | None = None, tags: Dict | None = None)
 
 Bases: `SDKBaseModel`, `IClusterFilter`
 
 Represents a filter used to select clusters based on specific criteria.
 
 This class is used to construct filter criteria for querying clusters by their identifiers,
 names, statuses, or tags. It inherits from SDKBaseModel and implements the IClusterFilter interface.
 
 #### ids
 
 Optional list of cluster UUIDs. Default is an empty list.
 
-- **Type:**
+* **Type:**
   Optional[List[str]]
 
 #### cluster_names
 
 Optional list of cluster names to filter by. Default is an empty list.
 
-- **Type:**
+* **Type:**
   Optional[List[str]]
 
 #### statuses
 
 Optional list of cluster statuses to filter by. Default is an empty list.
 
-- **Type:**
+* **Type:**
   Optional[List[str]]
 
 #### tags
 
 Optional dictionary of tags for more fine-grained filtering.
 
-- **Type:**
+* **Type:**
   Optional[Dict]
 
 ### Default is an empty dictionary.
 
 Each attribute supports being set via their field name or by the specified alias in the Field definition.
 
-#### _class_ Config
+#### *class* Config
 
 Bases: `object`
 
 Configuration for Pydantic models.
 [https://docs.pydantic.dev/latest/api/config/](https://docs.pydantic.dev/latest/api/config/)
 
-#### allow*population_by_field_name *= True\_
+#### allow_population_by_field_name *= True*
 
-#### extra _= 'forbid'_
+#### extra *= 'forbid'*
 
-#### cluster*names *: List[str] | None\_
+#### cluster_names *: List[str] | None*
 
-#### ids _: List[str] | None_
+#### ids *: List[str] | None*
 
-#### statuses _: List[str] | None_
+#### statuses *: List[str] | None*
 
-#### tags _: Dict | None_
+#### tags *: Dict | None*
 
-### _class_ bodosdk.models.cluster.ClusterList(workspace_client: IBodoWorkspaceClient = None, \*, page: int | None = 0, pageSize: int | None = 10, total: int | None = None, order: Dict | None = None, filters: [ClusterFilter](#bodosdk.models.cluster.ClusterFilter) | dict | None = None)
+### *class* bodosdk.models.cluster.ClusterList(workspace_client: IBodoWorkspaceClient = None, \*, page: int | None = 0, pageSize: int | None = 10, total: int | None = None, order: Dict | None = None, filters: [ClusterFilter](#bodosdk.models.cluster.ClusterFilter) | dict | None = None)
 
 Bases: `IClusterList`, `SDKBaseModel`
 
 A model representing a list of clusters, providing pagination, filtering, and
 operations on clusters such as start, stop, delete, resume, and pause.
 
 #### page
 
 The current page number for pagination, starting from 0.
 
-- **Type:**
+* **Type:**
   Optional[int]
 
 #### page_size
 
 The number of items to be displayed per page.
 
-- **Type:**
+* **Type:**
   Optional[int]
 
 #### total
 
 The total number of items available across all pages.
 
-- **Type:**
+* **Type:**
   Optional[int]
 
 #### order
 
 Ordering information for listing clusters. Defaults to an empty dict.
 
-- **Type:**
+* **Type:**
   Optional[Dict]
 
 #### filters
 
 Filtering criteria to apply when fetching the cluster list.
 
-- **Type:**
+* **Type:**
   Optional[[ClusterFilter](#bodosdk.models.cluster.ClusterFilter)]
 
 #### \_clusters
 
 Internal list of cluster objects.
 
-- **Type:**
+* **Type:**
   List[ICluster]
 
 #### \_index
 
 Internal index to track the current position when iterating through clusters.
 
-- **Type:**
+* **Type:**
   int
 
-#### _class_ Config
+#### *class* Config
 
 Bases: `object`
 
 Configuration for Pydantic models.
 [https://docs.pydantic.dev/latest/api/config/](https://docs.pydantic.dev/latest/api/config/)
 
-#### allow*population_by_field_name *= True\_
+#### allow_population_by_field_name *= True*
 
-#### extra _= 'forbid'_
+#### extra *= 'forbid'*
 
 #### cancel_jobs()
 
 Cancels all jobs associated with the clusters.
 
-- **Returns:**
+* **Returns:**
   The ClusterList instance.
 
 #### delete(wait=False)
 
 Deletes each cluster in the list, updating the internal list with the result
 of each delete operation. This method effectively attempts to delete all clusters
 and returns the updated list.
 
-- **Returns:**
+* **Returns:**
   The current instance of ClusterList after attempting to delete
   : all clusters.
-- **Return type:**
+* **Return type:**
   [ClusterList](#bodosdk.models.cluster.ClusterList)
 
-#### filters _: [ClusterFilter](#bodosdk.models.cluster.ClusterFilter) | dict | None_
+#### filters *: [ClusterFilter](#bodosdk.models.cluster.ClusterFilter) | dict | None*
 
-#### order _: Dict | None_
+#### order *: Dict | None*
 
-#### page _: int | None_
+#### page *: int | None*
 
-#### page*size *: int | None\_
+#### page_size *: int | None*
 
 #### pause(wait=False)
 
 Attempts to pause each running cluster in the list. It handles exceptions gracefully,
 updating the list with the status of each cluster following the operation.
 
-- **Returns:**
+* **Returns:**
   The current instance of ClusterList after attempting to pause
   : all clusters.
-- **Return type:**
+* **Return type:**
   [ClusterList](#bodosdk.models.cluster.ClusterList)
 
 #### refresh()
 
 Refreshes the list of clusters by resetting the pagination and filter settings,
 then reloading the first page of clusters. This method effectively resets the
 ClusterList instance to its initial state, based on current filters and ordering.
 
-- **Returns:**
+* **Returns:**
   The current instance of ClusterList after reloading the first page
   : of clusters.
-- **Return type:**
+* **Return type:**
   [ClusterList](#bodosdk.models.cluster.ClusterList)
 
 #### resume(wait=False)
 
 Attempts to resume each paused or stopped cluster in the list. It handles exceptions
 gracefully, ensuring the list is updated with the status of each cluster after
 the operation.
 
-- **Returns:**
+* **Returns:**
   The current instance of ClusterList after attempting to resume
   : all clusters.
-- **Return type:**
+* **Return type:**
   [ClusterList](#bodosdk.models.cluster.ClusterList)
 
 #### run_job(template_id: str = None, code_type: str = None, source: dict | IS3Source | IGitRepoSource | IWorkspaceSource | ITextSource = None, exec_file: str = None, args: dict | str = None, env_vars: dict = None, timeout: int = None, num_retries: int = None, delay_between_retries: int = None, retry_on_timeout: bool = None, name: str = None, catalog: str = None)
 
 Executes a job across all clusters managed by the instance.
 
 This method supports multiple source types and configurations for executing jobs,
 including retries and custom environment variables.
 
-- **Parameters:**
-  - **template_id** (_str_ _,_ _optional_) – Identifier for the job template to be used.
-  - **code_type** (_str_ _,_ _optional_) – The type of code to execute (e.g., Python, Java).
-  - **source** (_Union_ _[\*\*dict_ _,_ _IS3Source_ _,_ _IGitRepoSource_ _,_ _IWorkspaceSource_ _,_ _ITextSource_ _]_ _,_ _optional_) –
-  - **retrieved.** (_The source from where the job's code will be_) –
-  - **exec_file** (_str_ _,_ _optional_) – Path to the main executable file within the source.
-  - **args** (_Union_ _[\*\*dict_ _,_ _str_ _]_ _,_ _optional_) – Arguments to pass to the job. Can be a dictionary or a
-  - **job.** (_string formatted as required by the_) –
-  - **env_vars** (_dict_ _,_ _optional_) – Environment variables to set for the job execution.
-  - **timeout** (_int_ _,_ _optional_) – Maximum time in seconds for the job to run before it is terminated.
-  - **num_retries** (_int_ _,_ _optional_) – Number of times to retry the job on failure.
-  - **delay_between_retries** (_int_ _,_ _optional_) – Time in seconds to wait between retries.
-  - **retry_on_timeout** (_bool_ _,_ _optional_) – Whether to retry the job if it times out.
-  - **name** (_str_ _,_ _optional_) – A name for the job run.
-  - **catalog** (_str_ _,_ _optional_) – Catalog identifier to specify a data catalog for the job.
-- **Returns:**
+* **Parameters:**
+  * **template_id** (*str* *,* *optional*) – Identifier for the job template to be used.
+  * **code_type** (*str* *,* *optional*) – The type of code to execute (e.g., Python, Java).
+  * **source** (*Union* *[**dict* *,* *IS3Source* *,* *IGitRepoSource* *,* *IWorkspaceSource* *,* *ITextSource* *]* *,* *optional*) –
+  * **retrieved.** (*The source from where the job's code will be*) –
+  * **exec_file** (*str* *,* *optional*) – Path to the main executable file within the source.
+  * **args** (*Union* *[**dict* *,* *str* *]* *,* *optional*) – Arguments to pass to the job. Can be a dictionary or a
+  * **job.** (*string formatted as required by the*) –
+  * **env_vars** (*dict* *,* *optional*) – Environment variables to set for the job execution.
+  * **timeout** (*int* *,* *optional*) – Maximum time in seconds for the job to run before it is terminated.
+  * **num_retries** (*int* *,* *optional*) – Number of times to retry the job on failure.
+  * **delay_between_retries** (*int* *,* *optional*) – Time in seconds to wait between retries.
+  * **retry_on_timeout** (*bool* *,* *optional*) – Whether to retry the job if it times out.
+  * **name** (*str* *,* *optional*) – A name for the job run.
+  * **catalog** (*str* *,* *optional*) – Catalog identifier to specify a data catalog for the job.
+* **Returns:**
   An object listing the UUIDs of jobs that were successfully initiated.
-- **Return type:**
+* **Return type:**
   IJobRunList
 
 Decorators:
 : @check_deprecation: Checks if the method or its parameters are deprecated.
 
 #### run_sql_query(template_id: str = None, catalog: str = None, sql_query: str = None, name: str = None, args: dict = None, timeout: int = None, num_retries: int = None, delay_between_retries: int = None, retry_on_timeout: bool = None)
 
 Executes an SQL job across all clusters managed by the instance.
 
 This method submits an SQL query for execution, allowing for additional configurations such as retries
 and setting execution timeouts.
 
-- **Parameters:**
-  - **template_id** (_str_ _,_ _optional_) – Identifier for the job template to be used.
-  - **catalog** (_str_ _,_ _optional_) – Catalog identifier to specify a data catalog for the SQL job.
-  - **sql_query** (_str_ _,_ _optional_) – The SQL query to execute.
-  - **name** (_str_ _,_ _optional_) – A name for the job run.
-  - **args** (_dict_ _,_ _optional_) – Additional arguments specific to the SQL job.
-  - **timeout** (_int_ _,_ _optional_) – Maximum time in seconds for the job to run before it is terminated.
-  - **num_retries** (_int_ _,_ _optional_) – Number of times to retry the job on failure.
-  - **delay_between_retries** (_int_ _,_ _optional_) – Time in seconds to wait between retries.
-  - **retry_on_timeout** (_bool_ _,_ _optional_) – Whether to retry the job if it times out.
-- **Returns:**
+* **Parameters:**
+  * **template_id** (*str* *,* *optional*) – Identifier for the job template to be used.
+  * **catalog** (*str* *,* *optional*) – Catalog identifier to specify a data catalog for the SQL job.
+  * **sql_query** (*str* *,* *optional*) – The SQL query to execute.
+  * **name** (*str* *,* *optional*) – A name for the job run.
+  * **args** (*dict* *,* *optional*) – Additional arguments specific to the SQL job.
+  * **timeout** (*int* *,* *optional*) – Maximum time in seconds for the job to run before it is terminated.
+  * **num_retries** (*int* *,* *optional*) – Number of times to retry the job on failure.
+  * **delay_between_retries** (*int* *,* *optional*) – Time in seconds to wait between retries.
+  * **retry_on_timeout** (*bool* *,* *optional*) – Whether to retry the job if it times out.
+* **Returns:**
   An object listing the UUIDs of SQL jobs that were successfully initiated.
-- **Return type:**
+* **Return type:**
   IJobRunList
 
 Decorators:
 : @check_deprecation: Checks if the method or its parameters are deprecated.
 
 #### start(wait=False)
 
 Attempts to start each stopped or paused cluster in the list. It handles exceptions
 gracefully, ensuring the list reflects the status of each cluster after the operation.
 
-- **Returns:**
+* **Returns:**
   The current instance of ClusterList after attempting to start
   : all clusters.
-- **Return type:**
+* **Return type:**
   [ClusterList](#bodosdk.models.cluster.ClusterList)
 
 #### stop(wait=False)
 
 Attempts to stop each running or starting cluster in the list. It handles exceptions
 gracefully, updating the list with the status of each cluster after the operation.
 
-- **Returns:**
+* **Returns:**
   The current instance of ClusterList after attempting to stop
   : all clusters.
-- **Return type:**
+* **Return type:**
   [ClusterList](#bodosdk.models.cluster.ClusterList)
 
-#### total _: int | None_
+#### total *: int | None*
 
 #### wait_for_status(statuses: List[str] = None, timeout: int = 600, tick: int = 60)
 
 Waits for each cluster in the list to reach one of the specified statuses, updating
 the list with the results. This method polls each cluster’s status until it matches
 one of the desired statuses or until the timeout is reached.
 
-- **Parameters:**
-  - **statuses** (_List_ _[\*\*str_ _]_ _,_ _optional_) – A list of status strings to wait for.
-  - **timeout** (_int_ _,_ _optional_) – The maximum time to wait for each cluster to reach the
+* **Parameters:**
+  * **statuses** (*List* *[**str* *]* *,* *optional*) – A list of status strings to wait for.
+  * **timeout** (*int* *,* *optional*) – The maximum time to wait for each cluster to reach the
     desired status, in seconds.
-  - **tick** (_int_ _,_ _optional_) – The interval between status checks, in seconds.
-- **Returns:**
+  * **tick** (*int* *,* *optional*) – The interval between status checks, in seconds.
+* **Returns:**
   The current instance of ClusterList after waiting for all clusters
   : to reach one of the specified statuses.
-- **Return type:**
+* **Return type:**
   [ClusterList](#bodosdk.models.cluster.ClusterList)
 
-### _class_ bodosdk.models.cluster.InstanceType(\*, name: str, vcpus: int, cores: int, memory: int, efa: bool | None = None, acceleratedNetworking: bool | None = None)
+### *class* bodosdk.models.cluster.InstanceType(\*, name: str, vcpus: int, cores: int, memory: int, efa: bool | None = None, acceleratedNetworking: bool | None = None)
 
 Bases: `SDKBaseModel`, `IInstanceType`
 
 Represents the specifications for a type of computing instance.
 
 This class defines a specific configuration of a computing instance,
 including its processing power and memory capabilities, as well as optional features related to networking.
 
 #### name
 
 The name or identifier of the instance type.
 
-- **Type:**
+* **Type:**
   str
 
 #### vcpus
 
 The number of virtual CPUs available in this instance type.
 
-- **Type:**
+* **Type:**
   int
 
 #### cores
 
 The number of physical cores available in this instance type.
 
-- **Type:**
+* **Type:**
   int
 
 #### memory
 
 The amount of RAM (in megabytes) available in this instance type.
 
-- **Type:**
+* **Type:**
   int
 
 #### efa
 
 Indicates whether Elastic Fabric Adapter (EFA) is supported. Defaults to None.
 
-- **Type:**
+* **Type:**
   Optional[bool]
 
 #### accelerated_networking
 
 Specifies if accelerated networking is enabled.
 
-- **Type:**
+* **Type:**
   Optional[bool]
 
 ### This is mapped to the JSON key 'acceleratedNetworking'. Defaults to None.
 
-#### accelerated*networking *: bool | None\_
+#### accelerated_networking *: bool | None*
 
-#### cores _: int_
+#### cores *: int*
 
-#### efa _: bool | None_
+#### efa *: bool | None*
 
-#### memory _: int_
+#### memory *: int*
 
-#### name _: str_
+#### name *: str*
 
-#### vcpus _: int_
+#### vcpus *: int*
 
-### _class_ bodosdk.models.cluster.NodeMetadata(\*, privateIP: str | None = None, instanceId: str | None = None)
+### *class* bodosdk.models.cluster.NodeMetadata(\*, privateIP: str | None = None, instanceId: str | None = None)
 
 Bases: `SDKBaseModel`
 
-#### instance*id *: str | None\_
+#### instance_id *: str | None*
 
-#### private*ip *: str | None\_
+#### private_ip *: str | None*
 
 <a id="module-bodosdk.db.connection"></a>
 
-### _class_ bodosdk.db.connection.Connection(catalog: str, cluster: ICluster, timeout=3600)
+### *class* bodosdk.db.connection.Connection(catalog: str, cluster: ICluster, timeout=3600)
 
 Bases: `object`
 
 #### cursor()
 
-### _class_ bodosdk.db.connection.Cursor(catalog: str, cluster: ICluster, timeout: int)
+### *class* bodosdk.db.connection.Cursor(catalog: str, cluster: ICluster, timeout: int)
 
 Bases: `object`
 
 #### execute(query: str, \*\*kwargs)
 
 #### execute_async(query: str, \*\*kwargs)
 
 #### fetchall()
 
 #### fetchmany(size)
 
 #### fetchone()
 
-### _exception_ bodosdk.db.connection.QueryError
+### *exception* bodosdk.db.connection.QueryError
 
 Bases: `Exception`
 
 <a id="module-bodosdk.models.job"></a>
 
-### _class_ bodosdk.models.job.GitRepoSource(\*, type: str = 'GIT', repoUrl: str, reference: str | None = '', username: str, token: str)
+### *class* bodosdk.models.job.GitRepoSource(\*, type: str = 'GIT', repoUrl: str, reference: str | None = '', username: str, token: str)
 
 Bases: `SDKBaseModel`
 
 Git repository source definition.
 
 …
 
 #### repo_url
 
 Git repository URL.
 
-- **Type:**
+* **Type:**
   str
 
 #### reference
 
 Git reference (branch, tag, commit hash). (Default: “”)
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### username
 
 Git username.
 
-- **Type:**
+* **Type:**
   str
 
 #### token
 
 Git token.
 
-- **Type:**
+* **Type:**
   str
 
-#### reference _: str | None_
+#### reference *: str | None*
 
-#### repo*url *: str\_
+#### repo_url *: str*
 
-#### token _: str_
+#### token *: str*
 
-#### type _: str_
+#### type *: str*
 
-#### username _: str_
+#### username *: str*
 
-### _class_ bodosdk.models.job.JobConfig(\*, type: str | None = None, source: [GitRepoSource](#bodosdk.models.job.GitRepoSource) | [WorkspaceSource](#bodosdk.models.job.WorkspaceSource) | [S3Source](#bodosdk.models.job.S3Source) | [TextSource](#bodosdk.models.job.TextSource) | None = None, sourceLocation: str | None = None, sqlQueryText: str | None = None, sqlQueryParameters: dict | None = None, args: dict | str | None = None, retryStrategy: [RetryStrategy](#bodosdk.models.job.RetryStrategy) | None = None, timeout: int | None = None, envVars: dict | None = None, catalog: str | None = None)
+### *class* bodosdk.models.job.JobConfig(\*, type: str | None = None, source: [GitRepoSource](#bodosdk.models.job.GitRepoSource) | [WorkspaceSource](#bodosdk.models.job.WorkspaceSource) | [S3Source](#bodosdk.models.job.S3Source) | [TextSource](#bodosdk.models.job.TextSource) | None = None, sourceLocation: str | None = None, sqlQueryText: str | None = None, sqlQueryParameters: dict | None = None, args: dict | str | None = None, retryStrategy: [RetryStrategy](#bodosdk.models.job.RetryStrategy) | None = None, timeout: int | None = None, envVars: dict | None = None, catalog: str | None = None)
 
 Bases: `SDKBaseModel`, `IJobConfig`
 
 Configures details for executing a job, including the execution source, file location, and execution parameters.
 
 #### type
 
 The type of job: PYTHON, SQL, IPYNB
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### source
 
-- **Type:**
+* **Type:**
   Optional[Union[[GitRepoSource](#bodosdk.models.job.GitRepoSource), [WorkspaceSource](#bodosdk.models.job.WorkspaceSource), [S3Source](#bodosdk.models.job.S3Source), [TextSource](#bodosdk.models.job.TextSource)]]
 
 ### The source from which the job is configured or executed.
 
 #### exec_file
 
 The location of the file to execute.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### exec_text
 
 The text containing script/code/sql to execute, valid for TextSource
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### sql_query_parameters
 
 Parameters to substitute within an SQL query.
 
-- **Type:**
+* **Type:**
   Optional[dict]
 
 #### args
 
 Additional arguments required for job execution.
 
-- **Type:**
+* **Type:**
   Optional[Union[dict, str]]
 
 ### Can be a dictionary or string.
 
 #### retry_strategy
 
-- **Type:**
+* **Type:**
   Optional[[RetryStrategy](#bodosdk.models.job.RetryStrategy)]
 
 ### Configuration for the job retry strategy.
 
 #### timeout
 
 The maximum time (in seconds) allowed for the job to run before it times out.
 
-- **Type:**
+* **Type:**
   Optional[int]
 
 #### env_vars
 
 Environment variables to be set for the job run.
 
-- **Type:**
+* **Type:**
   Optional[dict]
 
 #### catalog
 
 The catalog associated with the job, if applicable.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
-#### args _: dict | str | None_
+#### args *: dict | str | None*
 
-#### catalog _: str | None_
+#### catalog *: str | None*
 
-#### env*vars *: dict | None\_
+#### env_vars *: dict | None*
 
-#### exec*file *: str | None\_
+#### exec_file *: str | None*
 
-#### exec*text *: str | None\_
+#### exec_text *: str | None*
 
-#### retry*strategy *: [RetryStrategy](#bodosdk.models.job.RetryStrategy) | None\_
+#### retry_strategy *: [RetryStrategy](#bodosdk.models.job.RetryStrategy) | None*
 
-#### source _: [GitRepoSource](#bodosdk.models.job.GitRepoSource) | [WorkspaceSource](#bodosdk.models.job.WorkspaceSource) | [S3Source](#bodosdk.models.job.S3Source) | [TextSource](#bodosdk.models.job.TextSource) | None_
+#### source *: [GitRepoSource](#bodosdk.models.job.GitRepoSource) | [WorkspaceSource](#bodosdk.models.job.WorkspaceSource) | [S3Source](#bodosdk.models.job.S3Source) | [TextSource](#bodosdk.models.job.TextSource) | None*
 
-#### sql*query_parameters *: dict | None\_
+#### sql_query_parameters *: dict | None*
 
-#### timeout _: int | None_
+#### timeout *: int | None*
 
-#### type _: str | None_
+#### type *: str | None*
 
-### _class_ bodosdk.models.job.JobFilter(\*, ids: List[str | UUID] | None = None, template_ids: List[str | UUID] | None = None, cluster_ids: List[str | UUID] | None = None, types: List[str] | None = None, statuses: List[str] | None = None, started_at: datetime | None = None, finished_at: datetime | None = None)
+### *class* bodosdk.models.job.JobFilter(\*, ids: List[str | UUID] | None = None, template_ids: List[str | UUID] | None = None, cluster_ids: List[str | UUID] | None = None, types: List[str] | None = None, statuses: List[str] | None = None, started_at: datetime | None = None, finished_at: datetime | None = None)
 
 Bases: `SDKBaseModel`
 
 Provides filtering options for querying job-related data.
 
 #### ids
 
 A list of job IDs to filter by.
 
-- **Type:**
+* **Type:**
   Optional[List[Union[str, UUID]]]
 
 #### template_ids
 
 A list of job template IDs to filter by.
 
-- **Type:**
+* **Type:**
   Optional[List[Union[str, UUID]]]
 
 #### cluster_ids
 
 A list of cluster IDs to filter jobs by.
 
-- **Type:**
+* **Type:**
   Optional[List[Union[str, UUID]]]
 
 #### types
 
 A list of job types to filter by.
 
-- **Type:**
+* **Type:**
   Optional[List[str]]
 
 #### statuses
 
 A list of job statuses to filter by.
 
-- **Type:**
+* **Type:**
   Optional[List[str]]
 
 #### started_at
 
 A datetime value to filter jobs that started after it.
 
-- **Type:**
+* **Type:**
   Optional[datetime]
 
 #### finished_at
 
 A datetime value to filter jobs that finished before it.
 
-- **Type:**
+* **Type:**
   Optional[datetime]
 
-#### cluster*ids *: List[str | UUID] | None\_
+#### cluster_ids *: List[str | UUID] | None*
 
-#### finished*at *: datetime | None\_
+#### finished_at *: datetime | None*
 
-#### ids _: List[str | UUID] | None_
+#### ids *: List[str | UUID] | None*
 
-#### started*at *: datetime | None\_
+#### started_at *: datetime | None*
 
-#### statuses _: List[str] | None_
+#### statuses *: List[str] | None*
 
-#### template*ids *: List[str | UUID] | None\_
+#### template_ids *: List[str | UUID] | None*
 
-#### types _: List[str] | None_
+#### types *: List[str] | None*
 
-### _class_ bodosdk.models.job.JobRun(workspace_client: IBodoWorkspaceClient = None, \*, uuid: str | None = None, name: str | None = None, type: str | None = 'BATCH', submittedAt: datetime | None = None, finishedAt: datetime | None = None, lastHealthCheck: datetime | None = None, lastKnownActivity: datetime | None = None, status: str | None = None, reason: str | None = None, num_retries_used: int | None = (FieldInfo(default=0, alias='numRetriesUsed', alias_priority=2, extra={}),), tag: List | None = None, clusterUUID: str | None = None, cluster: 'Cluster' | None, clusterConfig: 'Cluster' | None = None, config: [JobConfig](#bodosdk.models.job.JobConfig) | None = None, jobTemplateUUID: str | None = None, submitter: str | None = None, stats: dict | None = None)
+### *class* bodosdk.models.job.JobRun(workspace_client: IBodoWorkspaceClient = None, \*, uuid: str | None = None, name: str | None = None, type: str | None = 'BATCH', submittedAt: datetime | None = None, finishedAt: datetime | None = None, lastHealthCheck: datetime | None = None, lastKnownActivity: datetime | None = None, status: str | None = None, reason: str | None = None, num_retries_used: int | None = (FieldInfo(default=0, alias='numRetriesUsed', alias_priority=2, extra={}),), tag: List | None = None, clusterUUID: str | None = None, cluster: 'Cluster' | None, clusterConfig: 'Cluster' | None = None, config: [JobConfig](#bodosdk.models.job.JobConfig) | None = None, jobTemplateUUID: str | None = None, submitter: str | None = None, stats: dict | None = None)
 
 Bases: `SDKBaseModel`, `IJobRun`
 
 Details a specific instance of a job run, including status and configuration details.
 
 #### uuid
 
 Unique identifier for the job run.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### name
 
 Name of the job run.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### type
 
 Type of job run, defaults to ‘BATCH’ if not specified.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### submitted_at
 
 Timestamp when the job was submitted.
 
-- **Type:**
+* **Type:**
   Optional[datetime]
 
 #### finished_at
 
 Timestamp when the job finished running.
 
-- **Type:**
+* **Type:**
   Optional[datetime]
 
 #### last_health_check
 
 Timestamp of the last health check performed.
 
-- **Type:**
+* **Type:**
   Optional[datetime]
 
 #### last_known_activity
 
 Timestamp of the last known activity of this job.
 
-- **Type:**
+* **Type:**
   Optional[datetime]
 
 #### status
 
 Current status of the job run.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### reason
 
 Reason for the job’s current status, particularly if there’s an error or failure.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### num_retries_used
 
 The number of retries that have been used for this job run. Defaults to 0.
 
-- **Type:**
+* **Type:**
   Optional[int]
 
 #### tags
 
 Tags associated with the job run. Default is an empty list.
 
-- **Type:**
+* **Type:**
   Optional[List]
 
 #### cluster_uuid
 
 UUID of the cluster on which the job is running.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### cluster
 
 The cluster object associated with the job run.
 
-- **Type:**
+* **Type:**
   Optional[[Cluster](#bodosdk.models.cluster.Cluster)]
 
 #### cluster_config
 
 Configuration of the cluster used for this job run.
 
-- **Type:**
+* **Type:**
   Optional[[Cluster](#bodosdk.models.cluster.Cluster)]
 
 #### config
 
 Job configuration details used for this run.
 
-- **Type:**
+* **Type:**
   Optional[[JobConfig](#bodosdk.models.job.JobConfig)]
 
 #### job_template_id
 
 UUID of the template from which this job was created.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### submitter
 
 The identifier of the user who submitted the job.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### stats
 
 Statistical data about the job run.
 
-- **Type:**
+* **Type:**
   Optional[dict]
 
 #### cancel()
 
 Cancels the job associated with this instance and updates its state based on the response from the job API.
 
 This method sends a cancellation request for the job identified by its UUID to the job API,
 handles the response to update the job’s attributes, and resets its modified state.
 
-- **Returns:**
+* **Returns:**
   The job instance, updated with the latest state after the cancellation attempt.
-- **Return type:**
+* **Return type:**
   [JobRun](#bodosdk.models.job.JobRun)
-- **Raises:**
+* **Raises:**
   **APIException** – If the cancellation request fails or returns an error response.
 
 Decorators:
 : @check_deprecation: Checks if the method or its parameters are deprecated.
 
-#### cluster _: 'Cluster' | None_
+#### cluster *: 'Cluster' | None*
 
-#### cluster*config *: 'Cluster' | None\_
+#### cluster_config *: 'Cluster' | None*
 
-#### cluster*id *: str | None\_
+#### cluster_id *: str | None*
 
-#### config _: [JobConfig](#bodosdk.models.job.JobConfig) | None_
+#### config *: [JobConfig](#bodosdk.models.job.JobConfig) | None*
 
-#### finished*at *: datetime | None\_
+#### finished_at *: datetime | None*
 
 #### get_logs_urls()
 
 #### get_stderr()
 
 #### get_stdout()
 
-#### _property_ id _: str_
+#### *property* id *: str*
 
-#### job*template_id *: str | None\_
+#### job_template_id *: str | None*
 
-#### last*health_check *: datetime | None\_
+#### last_health_check *: datetime | None*
 
-#### last*known_activity *: datetime | None\_
+#### last_known_activity *: datetime | None*
 
-#### name _: str | None_
+#### name *: str | None*
 
-#### num*retries_used *: int | None\_
+#### num_retries_used *: int | None*
 
-#### reason _: str | None_
+#### reason *: str | None*
 
-#### stats _: dict | None_
+#### stats *: dict | None*
 
-#### status _: str | None_
+#### status *: str | None*
 
-#### submitted*at *: datetime | None\_
+#### submitted_at *: datetime | None*
 
-#### submitter _: str | None_
+#### submitter *: str | None*
 
-#### tags _: List | None_
+#### tags *: List | None*
 
-#### type _: str | None_
+#### type *: str | None*
 
-#### uuid _: str | None_
+#### uuid *: str | None*
 
 #### wait_for_status(statuses: List[str], timeout: int = 3600, tick: int = 30)
 
 Waits for the job to reach one of the specified statuses, polling at regular intervals.
 
 This method checks the current status of the job at regular intervals defined by the tick parameter.
 If the job reaches one of the specified statuses before the timeout, it returns the job instance.
 If the timeout is exceeded, it raises a TimeoutException.
 
-- **Parameters:**
-  - **statuses** (_list_ _or_ _tuple_) – A list or tuple of statuses that the job is expected to reach.
-  - **timeout** (_int_ _,_ _optional_) – The maximum time in seconds to wait for the job to reach one of
-  - **seconds.** (_the specified statuses. Defaults to 600_) –
-  - **tick** (_int_ _,_ _optional_) – The time interval in seconds between status checks. Defaults to 30 seconds.
-- **Returns:**
+* **Parameters:**
+  * **statuses** (*list* *or* *tuple*) – A list or tuple of statuses that the job is expected to reach.
+  * **timeout** (*int* *,* *optional*) – The maximum time in seconds to wait for the job to reach one of
+  * **seconds.** (*the specified statuses. Defaults to 600*) –
+  * **tick** (*int* *,* *optional*) – The time interval in seconds between status checks. Defaults to 30 seconds.
+* **Returns:**
   The job instance if one of the specified statuses is reached within the timeout period.
-- **Return type:**
+* **Return type:**
   [JobRun](#bodosdk.models.job.JobRun)
-- **Raises:**
-  - **TimeoutException** – If the job does not reach one of the specified statuses within
-  - **the specified timeout period.** –
+* **Raises:**
+  * **TimeoutException** – If the job does not reach one of the specified statuses within
+  * **the specified timeout period.** –
 
 Decorators:
 : @check_deprecation: Checks if the method or its parameters are deprecated.
 
-### _class_ bodosdk.models.job.JobRunList(workspace_client: IBodoWorkspaceClient = None, \*, page: int | None = 0, pageSize: int | None = 10, total: int | None = None, order: Dict | None = None, filters: [JobFilter](#bodosdk.models.job.JobFilter) | None = None)
+### *class* bodosdk.models.job.JobRunList(workspace_client: IBodoWorkspaceClient = None, \*, page: int | None = 0, pageSize: int | None = 10, total: int | None = None, order: Dict | None = None, filters: [JobFilter](#bodosdk.models.job.JobFilter) | None = None)
 
 Bases: `IJobRunList`, `SDKBaseModel`
 
 Represents a paginated list of job runs, including metadata and filtering capabilities.
 
 #### page
 
 The current page number in the paginated list. Defaults to 0.
 
-- **Type:**
+* **Type:**
   Optional[int]
 
 #### page_size
 
 The number of job runs to display per page. Defaults to 10.
 
-- **Type:**
+* **Type:**
   Optional[int]
 
 #### total
 
 The total number of job runs available.
 
-- **Type:**
+* **Type:**
   Optional[int]
 
 #### order
 
 A dictionary specifying the order in which job runs are sorted.
 
-- **Type:**
+* **Type:**
   Optional[Dict]
 
 #### filters
 
 A JobFilter object used to apply filtering on the list of job runs.
 
-- **Type:**
+* **Type:**
   Optional[[JobFilter](#bodosdk.models.job.JobFilter)]
 
 #### cancel()
 
 Cancels all jobs in the list.
 
 This method iterates through each job in the current list (represented by instances of this class),
 and calls the cancel method on each job to attempt their cancellation.
 After attempting to cancel all jobs, it returns the updated list of jobs.
 
-- **Returns:**
+* **Returns:**
   The list instance, potentially with updated states of the individual jobs
   if the cancellation requests were successful.
-- **Return type:**
+* **Return type:**
   [JobRunList](#bodosdk.models.job.JobRunList)
 
 #### NOTE
-
 This method relies on the individual cancel() method of the job objects within the list.
 If any job cancellation fails, it could raise an exception depending on
 the implementation of the individual cancel() method.
 
-#### _property_ clusters
+#### *property* clusters
 
-#### filters _: [JobFilter](#bodosdk.models.job.JobFilter) | None_
+#### filters *: [JobFilter](#bodosdk.models.job.JobFilter) | None*
 
-#### order _: Dict | None_
+#### order *: Dict | None*
 
-#### page _: int | None_
+#### page *: int | None*
 
-#### page*size *: int | None\_
+#### page_size *: int | None*
 
 #### refresh()
 
 Refreshes the list of jobs by clearing the current elements and reloading the next page of job data.
 
 This method resets the internal state of the list, including the pagination index and the elements themselves.
 It then loads the next page of data from the underlying data source to repopulate the list.
 The list is temporarily set to mutable during this process to allow updates, and then set back to immutable
 once the refresh is complete.
 
-- **Returns:**
+* **Returns:**
   The refreshed job run list instance, with elements reloaded from the next available page.
-- **Return type:**
+* **Return type:**
   [JobRunList](#bodosdk.models.job.JobRunList)
 
 #### NOTE
-
 This method assumes that the list supports pagination and that the underlying data source provides
 the mechanism to load additional pages of data.
 
-#### total _: int | None_
+#### total *: int | None*
 
 #### wait_for_status(statuses: List[str], timeout: int = 3600, tick: int = 30)
 
 Waits for each job in the list to reach one of the specified statuses, polling each at regular intervals.
 
 This method iterates over each job within the list, checking at intervals (defined by tick) to see
 if the job has reached one of the desired statuses specified in statuses.
 If a job reaches the desired status within the timeout period, the method continues to the next job.
 If the timeout is reached without the job reaching the desired status, a TimeoutException is raised.
 
-- **Parameters:**
-  - **statuses** (_list_ _or_ _tuple_) – A list or tuple of statuses that each job is expected to reach.
-  - **timeout** (_int_ _,_ _optional_) – The maximum time in seconds to wait for each job to reach one of
-  - **seconds.** (_Defaults to 30_) –
-  - **tick** (_int_ _,_ _optional_) – The time interval in seconds between status checks for each job.
-  - **seconds.** –
-- **Returns:**
+* **Parameters:**
+  * **statuses** (*list* *or* *tuple*) – A list or tuple of statuses that each job is expected to reach.
+  * **timeout** (*int* *,* *optional*) – The maximum time in seconds to wait for each job to reach one of
+  * **seconds.** (*Defaults to 30*) –
+  * **tick** (*int* *,* *optional*) – The time interval in seconds between status checks for each job.
+  * **seconds.** –
+* **Returns:**
   The job run list instance, after attempting to wait for all jobs to reach the desired statuses.
-- **Return type:**
+* **Return type:**
   [JobRunList](#bodosdk.models.job.JobRunList)
-- **Raises:**
-  - **TimeoutException** – If any job does not reach one of the specified statuses within the specified
-  - **timeout period\*\***,\*\* **including details** **of** **the job's UUID and its current status.** –
+* **Raises:**
+  * **TimeoutException** – If any job does not reach one of the specified statuses within the specified
+  * **timeout period****,** **including details** **of** **the job's UUID and its current status.** –
 
 Decorators:
 : @check_deprecation: Checks if the method or its parameters are deprecated.
 
 #### NOTE
-
 This method individually tracks the timeout for each job, resetting the start time at the beginning
 of the wait for each job in the list.
 
-### _class_ bodosdk.models.job.JobRunLogsResponse(\*, stderrUrl: str = None, stdoutUrl: str = None, expirationDate: str = None)
+### *class* bodosdk.models.job.JobRunLogsResponse(\*, stderrUrl: str = None, stdoutUrl: str = None, expirationDate: str = None)
 
 Bases: `SDKBaseModel`, `IJobRunLogsResponse`
 
 Represents the response object containing URLs for accessing logs related to a job run.
 
 #### stderr_location_url
 
 The URL to access the standard error logs of the job run.
 
-- **Type:**
+* **Type:**
   str
 
 #### stdout_location_url
 
 The URL to access the standard output logs of the job run.
 
-- **Type:**
+* **Type:**
   str
 
 #### expiration_date
 
 The date when the log URLs will expire and no longer be accessible.
 
-- **Type:**
+* **Type:**
   str
 
-#### expiration*date *: str\_
+#### expiration_date *: str*
 
-#### stderr*location_url *: str\_
+#### stderr_location_url *: str*
 
-#### stdout*location_url *: str\_
+#### stdout_location_url *: str*
 
-### _class_ bodosdk.models.job.JobTemplate(workspace_client: IBodoWorkspaceClient = None, \*, uuid: str | None = None, name: str | None = None, jobRuns: List[[JobRun](#bodosdk.models.job.JobRun)] = None, description: str | None = None, createdBy: str | None = None, config: [JobConfig](#bodosdk.models.job.JobConfig) | None = None, clusterConfig: 'Cluster' | None = None)
+### *class* bodosdk.models.job.JobTemplate(workspace_client: IBodoWorkspaceClient = None, \*, uuid: str | None = None, name: str | None = None, jobRuns: List[[JobRun](#bodosdk.models.job.JobRun)] = None, description: str | None = None, createdBy: str | None = None, config: [JobConfig](#bodosdk.models.job.JobConfig) | None = None, clusterConfig: 'Cluster' | None = None)
 
 Bases: `SDKBaseModel`, `IJobTemplate`
 
 Represents a template for creating and managing jobs within an SDK environment, e
 ncapsulating common job configurations.
 
 #### uuid
 
 The unique identifier for the job template.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### name
 
 The name of the job template.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### job_runs
 
 A list of job runs associated with this template. Default is an empty list
 
-- **Type:**
+* **Type:**
   List[[JobRun](#bodosdk.models.job.JobRun)]
 
 ### if none are specified.
 
 #### description
 
 A brief description of the job template.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### created_by
 
 The identifier of the user who created the job template.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### config
 
 The job configuration specifics for this template.
 
-- **Type:**
+* **Type:**
   Optional[[JobConfig](#bodosdk.models.job.JobConfig)]
 
 #### cluster_config
 
 Configuration details of the cluster on which the jobs will run. D
 
-- **Type:**
+* **Type:**
   Optional[[Cluster](#bodosdk.models.cluster.Cluster)]
 
 ### efault is None.
 
-#### cluster*config *: [Cluster](#bodosdk.models.cluster.Cluster) | None\_
+#### cluster_config *: [Cluster](#bodosdk.models.cluster.Cluster) | None*
 
-#### config _: [JobConfig](#bodosdk.models.job.JobConfig) | None_
+#### config *: [JobConfig](#bodosdk.models.job.JobConfig) | None*
 
-#### created*by *: str | None\_
+#### created_by *: str | None*
 
 #### delete()
 
-#### description _: str | None_
+#### description *: str | None*
 
-#### _property_ id
+#### *property* id
 
-#### job*runs *: List[[JobRun](#bodosdk.models.job.JobRun)]\_
+#### job_runs *: List[[JobRun](#bodosdk.models.job.JobRun)]*
 
-#### name _: str | None_
+#### name *: str | None*
 
 #### run(name: str = None, cluster: dict | ICluster = None, code_type: str = None, source: dict | IS3Source | IGitRepoSource | IWorkspaceSource | ITextSource = None, exec_file: str = None, exec_text: str = None, args: dict | str = None, env_vars: dict = None, timeout: int = None, num_retries: int = None, delay_between_retries: int = None, retry_on_timeout: bool = None, catalog: str = None)
 
-#### uuid _: str | None_
+#### uuid *: str | None*
 
-### _class_ bodosdk.models.job.JobTemplateFilter(\*, ids: List[str] | None = None, names: List[str] | None = None, tags: dict | None = None)
+### *class* bodosdk.models.job.JobTemplateFilter(\*, ids: List[str] | None = None, names: List[str] | None = None, tags: dict | None = None)
 
 Bases: `SDKBaseModel`, `IJobTemplateFilter`
 
 Class representig filters for JobTemplateList
 
 #### ids
 
 returns list matching given ids
 
-- **Type:**
+* **Type:**
   List[str] | None
 
 #### names
 
 returns list matching given names
 
-- **Type:**
+* **Type:**
   List[str] | None
 
 #### tags
 
 returns list matching given tags
 
-- **Type:**
+* **Type:**
   dict | None
 
-#### ids _: List[str] | None_
+#### ids *: List[str] | None*
 
-#### names _: List[str] | None_
+#### names *: List[str] | None*
 
-#### tags _: dict | None_
+#### tags *: dict | None*
 
-### _class_ bodosdk.models.job.JobTemplateList(workspace_client: IBodoWorkspaceClient = None, \*, page: int | None = 0, pageSize: int | None = 10, total: int | None = None, order: Dict | None = None, filters: [JobTemplateFilter](#bodosdk.models.job.JobTemplateFilter) | None = None)
+### *class* bodosdk.models.job.JobTemplateList(workspace_client: IBodoWorkspaceClient = None, \*, page: int | None = 0, pageSize: int | None = 10, total: int | None = None, order: Dict | None = None, filters: [JobTemplateFilter](#bodosdk.models.job.JobTemplateFilter) | None = None)
 
 Bases: `IJobTemplateList`, `SDKBaseModel`
 
 Represents a list of JobTemplates, providing pagination and filtering capabilities.
 
 #### page
 
 The current page number in the list of Job Templates. Defaults to 0.
 
-- **Type:**
+* **Type:**
   Optional[int]
 
 #### page_size
 
 The number of Job Templates to display per page. Defaults to 10.
 
-- **Type:**
+* **Type:**
   Optional[int]
 
 #### total
 
 The total number of Job Templates available.
 
-- **Type:**
+* **Type:**
   Optional[int]
 
 #### order
 
 A dictionary specifying the order in which Job Templates are sorted.
 
-- **Type:**
+* **Type:**
   Optional[Dict]
 
 #### filters
 
 A filter object used to filter the Job Templates listed.
 
-- **Type:**
+* **Type:**
   Optional[[InstanceRoleFilter](#bodosdk.models.instance_role.InstanceRoleFilter)]
 
 #### delete()
 
 Deletes all job definitions in the list.
 
 This method iterates over each job definition contained within the list and calls its individual
 delete method. This action attempts to remove each job definition from the underlying storage
 or management system.
 
 #### NOTE
-
 The behavior and success of the deletion process depend on the implementation of the individual
 delete method of each job definition. This may include handling exceptions and ensuring that each
 job definition is properly removed. If an error occurs during the deletion of any job definition,
 it may raise an exception, which should be handled by the caller or within the individual delete methods.
 
-#### filters _: [JobTemplateFilter](#bodosdk.models.job.JobTemplateFilter) | None_
+#### filters *: [JobTemplateFilter](#bodosdk.models.job.JobTemplateFilter) | None*
 
-#### order _: Dict | None_
+#### order *: Dict | None*
 
-#### page _: int | None_
+#### page *: int | None*
 
-#### page*size *: int | None\_
+#### page_size *: int | None*
 
 #### refresh()
 
 Refreshes the list of job templates by clearing the current elements and reloading the next page of job data.
 
 This method resets the internal state of the list, including the pagination index and the elements themselves.
 It then loads the next page of data from the underlying data source to repopulate the list.
 The list is temporarily set to mutable during this process to allow updates, and then set back to
 immutable once the refresh is complete.
 
-- **Returns:**
+* **Returns:**
   The refreshed job template list instance, with elements reloaded from
   the next available page.
-- **Return type:**
+* **Return type:**
   [JobTemplateList](#bodosdk.models.job.JobTemplateList)
 
 #### NOTE
-
 This method assumes that the list supports pagination and that the underlying data source provides
 the mechanism to load additional pages of data.
 
 #### run(instance_type: str = None, workers_quantity: int = None, bodo_version: str = None)
 
 )
 Executes all job definitions in the list with specified configurations and aggregates their run IDs.
 
 This method iterates over each job definition in the list and invokes the run method on each, passing
 the specified configuration parameters such as instance type, the quantity of workers, and the Bodo version.
 It collects the IDs of the resulting job runs and returns a consolidated list of these job runs.
 
-- **Parameters:**
-  - **instance_type** (_str_ _,_ _optional_) – The type of instance to use for the jobs.
-  - **specifications.** (_This may specify the hardware_) –
-  - **workers_quantity** (_int_ _,_ _optional_) – The number of worker instances to deploy for the jobs.
-  - **bodo_version** (_str_ _,_ _optional_) – The specific version of Bodo to use for executing the jobs.
-- **Returns:**
+* **Parameters:**
+  * **instance_type** (*str* *,* *optional*) – The type of instance to use for the jobs.
+  * **specifications.** (*This may specify the hardware*) –
+  * **workers_quantity** (*int* *,* *optional*) – The number of worker instances to deploy for the jobs.
+  * **bodo_version** (*str* *,* *optional*) – The specific version of Bodo to use for executing the jobs.
+* **Returns:**
   An interface to the list of job runs created by executing the job definitions,
   allowing further operations like monitoring and management.
-- **Return type:**
+* **Return type:**
   IJobRunList
 
 #### NOTE
-
 The run method for each job definition must correctly handle the passed configurations.
 If any job execution fails, the behavior and handling of errors should be considered based
 on the implementation of each job definition’s run method.
 
-#### total _: int | None_
+#### total *: int | None*
 
-### _class_ bodosdk.models.job.RetryStrategy(\*, numRetries: int = 0, delayBetweenRetries: int = 1, retryOnTimeout: bool = False)
+### *class* bodosdk.models.job.RetryStrategy(\*, numRetries: int = 0, delayBetweenRetries: int = 1, retryOnTimeout: bool = False)
 
 Bases: `SDKBaseModel`
 
 A Pydantic model that defines the retry strategy for a job or a task. It specifies how many retries
 should be attempted,
 the delay between retries, and whether to retry on timeout.
 
 #### num_retries
 
 The number of times to retry the job after a failure. Defaults to 0, meaning no
 
-- **Type:**
+* **Type:**
   int
 
 ### retries by default.
 
 #### delay_between_retries
 
 The delay between consecutive retries, expressed in minutes. Defaults to 1 minute.
 
-- **Type:**
+* **Type:**
   int
 
 #### retry_on_timeout
 
 A flag to determine if the job should be retried upon timing out. Defaults to False,
 
-- **Type:**
+* **Type:**
   bool
 
 ### indicating no retry on timeout.
 
 Each field is represented with a default value and an alias that matches the corresponding key in JSON or
 other serialized forms.
 
-#### delay*between_retries *: int\_
+#### delay_between_retries *: int*
 
-#### num*retries *: int\_
+#### num_retries *: int*
 
-#### retry*on_timeout *: bool\_
+#### retry_on_timeout *: bool*
 
-### _class_ bodosdk.models.job.S3Source(\*, type: str = 'S3', bucketPath: str, bucketRegion: str)
+### *class* bodosdk.models.job.S3Source(\*, type: str = 'S3', bucketPath: str, bucketRegion: str)
 
 Bases: `SDKBaseModel`
 
 S3 source definition.
 
 …
 
 #### bucket_path
 
 S3 bucket path.
 
-- **Type:**
+* **Type:**
   str
 
 #### bucket_region
 
 S3 bucket region.
 
-- **Type:**
+* **Type:**
   str
 
-#### bucket*path *: str\_
+#### bucket_path *: str*
 
-#### bucket*region *: str\_
+#### bucket_region *: str*
 
-#### type _: str_
+#### type *: str*
 
-### _class_ bodosdk.models.job.TextSource(\*, type: str = 'SQL')
+### *class* bodosdk.models.job.TextSource(\*, type: str = 'SQL')
 
 Bases: `SDKBaseModel`
 
 Represents a specific type of source where the job configuration can originate from a text source.
 
 #### type
 
 Specifies the type of source
 
-- **Type:**
+* **Type:**
   str
 
-#### type _: str_
+#### type *: str*
 
-### _class_ bodosdk.models.job.WorkspaceSource(\*, type: str = 'WORKSPACE', path: str)
+### *class* bodosdk.models.job.WorkspaceSource(\*, type: str = 'WORKSPACE', path: str)
 
 Bases: `SDKBaseModel`
 
 Workspace source definition.
 
 …
 
 #### path
 
 Workspace path.
 
-- **Type:**
+* **Type:**
   str
 
-#### path _: str_
+#### path *: str*
 
-#### type _: str_
+#### type *: str*
 
 <a id="module-bodosdk.models.common"></a>
 
-### _class_ bodosdk.models.common.AWSNetworkData(\*, region: str | None = None, storageEndpoint: bool | None = None, vpcId: str | None = None, fetchedVpcId: str | None = None, publicSubnetsIds: List[str] | None = None, privateSubnetsIds: List[str] | None = None, policyArns: List[str] | None = None)
+### *class* bodosdk.models.common.AWSNetworkData(\*, region: str | None = None, storageEndpoint: bool | None = None, vpcId: str | None = None, fetchedVpcId: str | None = None, publicSubnetsIds: List[str] | None = None, privateSubnetsIds: List[str] | None = None, policyArns: List[str] | None = None)
 
 Bases: [`NetworkData`](#bodosdk.models.common.NetworkData)
 
 Extends the NetworkData class to include specific properties for AWS networking.
 
 #### vpc_id
 
 The ID of the AWS Virtual Private Cloud (VPC) where workspace should be created.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### fetched_vpc_id
 
 The ID of the fetched AWS VPC - if no vpc_id provided.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### public_subnets_ids
 
 List of IDs for the public subnets within the AWS VPC.
 
-- **Type:**
+* **Type:**
   Optional[List[str]]
 
 #### private_subnets_ids
 
 List of IDs for the private subnets within the AWS VPC.
 
-- **Type:**
+* **Type:**
   Optional[List[str]]
 
 #### policies_arn
 
 List of AWS Resource Names (ARNs) for the policies applied to the network.
 
-- **Type:**
+* **Type:**
   Optional[List[str]]
 
-#### fetched*vpc_id *: str | None\_
+#### fetched_vpc_id *: str | None*
 
-#### policies*arn *: List[str] | None\_
+#### policies_arn *: List[str] | None*
 
-#### private*subnets_ids *: List[str] | None\_
+#### private_subnets_ids *: List[str] | None*
 
-#### public*subnets_ids *: List[str] | None\_
+#### public_subnets_ids *: List[str] | None*
 
-#### vpc*id *: str | None\_
+#### vpc_id *: str | None*
 
-### _class_ bodosdk.models.common.NetworkData(\*, region: str | None = None, storageEndpoint: bool | None = None)
+### *class* bodosdk.models.common.NetworkData(\*, region: str | None = None, storageEndpoint: bool | None = None)
 
 Bases: `SDKBaseModel`
 
 A base model for network-related data within an SDK context.
 
 #### region
 
 The geographic region where the network is located.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### storage_endpoint
 
 Indicates whether a storage endpoint is enabled.
 
-- **Type:**
+* **Type:**
   Optional[bool]
 
-#### region _: str | None_
+#### region *: str | None*
 
-#### storage*endpoint *: bool | None\_
+#### storage_endpoint *: bool | None*
 
 <a id="module-bodosdk.models.instance_role"></a>
 
-### _class_ bodosdk.models.instance_role.InstanceRole(workspace_client: IBodoWorkspaceClient = None, \*, uuid: str | None = None, name: str | None = None, description: str | None = None, roleArn: str | None = None, status: str | None = None)
+### *class* bodosdk.models.instance_role.InstanceRole(workspace_client: IBodoWorkspaceClient = None, \*, uuid: str | None = None, name: str | None = None, description: str | None = None, roleArn: str | None = None, status: str | None = None)
 
 Bases: `SDKBaseModel`, `IInstanceRole`
 
 #### delete()
 
 Removes instance role from workspace
 
-- **Returns:**
+* **Returns:**
   None
 
-#### description _: str | None_
+#### description *: str | None*
 
-#### _property_ id
+#### *property* id
 
-#### name _: str | None_
+#### name *: str | None*
 
-#### role*arn *: str | None\_
+#### role_arn *: str | None*
 
-#### status _: str | None_
+#### status *: str | None*
 
-#### uuid _: str | None_
+#### uuid *: str | None*
 
-### _class_ bodosdk.models.instance_role.InstanceRoleFilter(\*, uuids: List[str] | None = None, names: List[str] | None = None, roleArns: List[str] | None = None)
+### *class* bodosdk.models.instance_role.InstanceRoleFilter(\*, uuids: List[str] | None = None, names: List[str] | None = None, roleArns: List[str] | None = None)
 
 Bases: `SDKBaseModel`, `IInstanceRoleFilter`
 
 Class representing filters for InstanceRoleList
 
 #### ids
 
 returns list matching given ids
 
-- **Type:**
+* **Type:**
   List[str] | None
 
 #### names
 
 returns list matching given names
 
-- **Type:**
+* **Type:**
   List[str] | None
 
 #### role_arns
 
 returns list matching giver arns
 
-- **Type:**
+* **Type:**
   List[str] | None
 
-#### _class_ Config
+#### *class* Config
 
 Bases: `object`
 
 Configuration for Pydantic models.
 [https://docs.pydantic.dev/latest/api/config/](https://docs.pydantic.dev/latest/api/config/)
 
-#### allow*population_by_field_name *= True\_
+#### allow_population_by_field_name *= True*
 
-#### extra _= 'forbid'_
+#### extra *= 'forbid'*
 
-#### ids _: List[str] | None_
+#### ids *: List[str] | None*
 
-#### names _: List[str] | None_
+#### names *: List[str] | None*
 
-#### role*arns *: List[str] | None\_
+#### role_arns *: List[str] | None*
 
-### _class_ bodosdk.models.instance_role.InstanceRoleList(workspace_client: IBodoWorkspaceClient = None, \*, page: int | None = 0, pageSize: int | None = 10, total: int | None = None, order: Dict | None = None, filters: [InstanceRoleFilter](#bodosdk.models.instance_role.InstanceRoleFilter) | None = None)
+### *class* bodosdk.models.instance_role.InstanceRoleList(workspace_client: IBodoWorkspaceClient = None, \*, page: int | None = 0, pageSize: int | None = 10, total: int | None = None, order: Dict | None = None, filters: [InstanceRoleFilter](#bodosdk.models.instance_role.InstanceRoleFilter) | None = None)
 
 Bases: `IInstanceRoleList`, `SDKBaseModel`
 
 Represents a list of instance roles within an SDK context, providing pagination and filtering capabilities.
 
 #### page
 
 The current page number in the list of instance roles. Defaults to 0.
 
-- **Type:**
+* **Type:**
   Optional[int]
 
 #### page_size
 
 The number of instance roles to display per page. Defaults to 10.
 
-- **Type:**
+* **Type:**
   Optional[int]
 
 #### total
 
 The total number of instance roles available.
 
-- **Type:**
+* **Type:**
   Optional[int]
 
 #### order
 
 A dictionary specifying the order in which instance roles are sorted.
 
-- **Type:**
+* **Type:**
   Optional[Dict]
 
 #### filters
 
 A filter object used to filter the instance roles listed.
 
-- **Type:**
+* **Type:**
   Optional[[InstanceRoleFilter](#bodosdk.models.instance_role.InstanceRoleFilter)]
 
-#### _class_ Config
+#### *class* Config
 
 Bases: `object`
 
 Configuration for Pydantic models.
 [https://docs.pydantic.dev/latest/api/config/](https://docs.pydantic.dev/latest/api/config/)
 
-#### allow*population_by_field_name *= True\_
+#### allow_population_by_field_name *= True*
 
-#### extra _= 'forbid'_
+#### extra *= 'forbid'*
 
 #### delete()
 
-#### filters _: [InstanceRoleFilter](#bodosdk.models.instance_role.InstanceRoleFilter) | None_
+#### filters *: [InstanceRoleFilter](#bodosdk.models.instance_role.InstanceRoleFilter) | None*
 
-#### order _: Dict | None_
+#### order *: Dict | None*
 
-#### page _: int | None_
+#### page *: int | None*
 
-#### page*size *: int | None\_
+#### page_size *: int | None*
 
-#### total _: int | None_
+#### total *: int | None*
 
 <a id="module-bodosdk.models.workspace"></a>
 
-### _class_ bodosdk.models.workspace.Workspace(org_client: IBodoOrganizationClient = None, \*, name: str | None = None, uuid: str | UUID | None = None, status: str | None = None, organizationUUID: str | UUID | None = None, networkData: [NetworkData](#bodosdk.models.common.NetworkData) | [AWSNetworkData](#bodosdk.models.common.AWSNetworkData) | None = None, createdBy: str | None = None, notebookAutoDeployEnabled: bool | None = None, assignedAt: datetime | None = None, customTags: Dict[str, Any] | None = None, jupyterLastActivity: datetime | None = None, jupyterIsActive: bool | None = False, cloudConfig: [AwsCloudConfig](#bodosdk.models.cloud_config.AwsCloudConfig) | [AzureCloudConfig](#bodosdk.models.cloud_config.AzureCloudConfig) | None = None)
+### *class* bodosdk.models.workspace.Workspace(org_client: IBodoOrganizationClient = None, \*, name: str | None = None, uuid: str | UUID | None = None, status: str | None = None, organizationUUID: str | UUID | None = None, networkData: [NetworkData](#bodosdk.models.common.NetworkData) | [AWSNetworkData](#bodosdk.models.common.AWSNetworkData) | None = None, createdBy: str | None = None, notebookAutoDeployEnabled: bool | None = None, assignedAt: datetime | None = None, customTags: Dict[str, Any] | None = None, jupyterLastActivity: datetime | None = None, jupyterIsActive: bool | None = False, cloudConfig: [AwsCloudConfig](#bodosdk.models.cloud_config.AwsCloudConfig) | [AzureCloudConfig](#bodosdk.models.cloud_config.AzureCloudConfig) | None = None)
 
 Bases: `SDKBaseModel`, `IWorkspace`
 
-#### assigned*at *: datetime | None\_
+#### assigned_at *: datetime | None*
 
-#### cloud*config *: [AwsCloudConfig](#bodosdk.models.cloud_config.AwsCloudConfig) | [AzureCloudConfig](#bodosdk.models.cloud_config.AzureCloudConfig) | None\_
+#### cloud_config *: [AwsCloudConfig](#bodosdk.models.cloud_config.AwsCloudConfig) | [AzureCloudConfig](#bodosdk.models.cloud_config.AzureCloudConfig) | None*
 
-#### created*by *: str | None\_
+#### created_by *: str | None*
 
-#### custom*tags *: Dict[str, Any] | None\_
+#### custom_tags *: Dict[str, Any] | None*
 
 #### delete()
 
 Deletes the workspace from the API based on its UUID and updates the instance’s properties
 with the response from the deletion API call.
 
-- **Returns:**
+* **Returns:**
   The Workspace instance after deletion, updated with the API’s response data.
 
-#### _property_ id
+#### *property* id
 
-#### jupyter*is_active *: bool | None\_
+#### jupyter_is_active *: bool | None*
 
-#### jupyter*last_activity *: datetime | None\_
+#### jupyter_last_activity *: datetime | None*
 
-#### name _: str | None_
+#### name *: str | None*
 
-#### network*data *: [NetworkData](#bodosdk.models.common.NetworkData) | [AWSNetworkData](#bodosdk.models.common.AWSNetworkData) | None\_
+#### network_data *: [NetworkData](#bodosdk.models.common.NetworkData) | [AWSNetworkData](#bodosdk.models.common.AWSNetworkData) | None*
 
-#### notebook*auto_deploy_enabled *: bool | None\_
+#### notebook_auto_deploy_enabled *: bool | None*
 
-#### organization*uuid *: str | UUID | None\_
+#### organization_uuid *: str | UUID | None*
 
-#### status _: str | None_
+#### status *: str | None*
 
 #### update_infra()
 
-#### uuid _: str | UUID | None_
+#### uuid *: str | UUID | None*
 
 #### wait_for_status(statuses, timeout=600, tick=30)
 
 Waits for the workspace to reach one of the specified states within a given timeout.
 
-- **Parameters:**
-  - **statuses** – A list of states to wait for.
-  - **timeout** – The maximum time to wait before raising a TimeoutException.
-  - **tick** – The interval between checks.
-- **Returns:**
+* **Parameters:**
+  * **statuses** – A list of states to wait for.
+  * **timeout** – The maximum time to wait before raising a TimeoutException.
+  * **tick** – The interval between checks.
+* **Returns:**
   The workspace instance, once it has reached one of the desired states.
-- **Raises:**
+* **Raises:**
   **TimeoutException** – If the workspace does not reach a desired state within the timeout.
 
-### _class_ bodosdk.models.workspace.WorkspaceFilter(\*, uuids: List[str] | None = None, names: List[str] | None = None, statuses: List[str] | None = None, organizationUUIDs: List[str] | None = None)
+### *class* bodosdk.models.workspace.WorkspaceFilter(\*, uuids: List[str] | None = None, names: List[str] | None = None, statuses: List[str] | None = None, organizationUUIDs: List[str] | None = None)
 
 Bases: `SDKBaseModel`, `IWorkspaceFilter`
 
-#### _class_ Config
+#### *class* Config
 
 Bases: `object`
 
-#### allow*population_by_field_name *= True\_
+#### allow_population_by_field_name *= True*
 
-#### extra _= 'forbid'_
+#### extra *= 'forbid'*
 
-#### ids _: List[str] | None_
+#### ids *: List[str] | None*
 
-#### names _: List[str] | None_
+#### names *: List[str] | None*
 
-#### organization*uuids *: List[str] | None\_
+#### organization_uuids *: List[str] | None*
 
-#### statuses _: List[str] | None_
+#### statuses *: List[str] | None*
 
-### _class_ bodosdk.models.workspace.WorkspaceList(org_client: IBodoOrganizationClient = None, \*, page: int | None = 0, pageSize: int | None = 10, total: int | None = None, order: Dict | None = None, filters: [WorkspaceFilter](#bodosdk.models.workspace.WorkspaceFilter) | None = None)
+### *class* bodosdk.models.workspace.WorkspaceList(org_client: IBodoOrganizationClient = None, \*, page: int | None = 0, pageSize: int | None = 10, total: int | None = None, order: Dict | None = None, filters: [WorkspaceFilter](#bodosdk.models.workspace.WorkspaceFilter) | None = None)
 
 Bases: `IWorkspaceList`, `SDKBaseModel`
 
-#### _class_ Config
+#### *class* Config
 
 Bases: `object`
 
-#### allow*population_by_field_name *= True\_
+#### allow_population_by_field_name *= True*
 
-#### extra _= 'forbid'_
+#### extra *= 'forbid'*
 
 #### delete()
 
 Deletes the workspaces present on the list
 
-- **Returns:**
+* **Returns:**
   WorkspaceListAPIModel
 
-#### filters _: [WorkspaceFilter](#bodosdk.models.workspace.WorkspaceFilter) | None_
+#### filters *: [WorkspaceFilter](#bodosdk.models.workspace.WorkspaceFilter) | None*
 
-#### order _: Dict | None_
+#### order *: Dict | None*
 
-#### page _: int | None_
+#### page *: int | None*
 
-#### page*size *: int | None\_
+#### page_size *: int | None*
 
-#### total _: int | None_
+#### total *: int | None*
 
 #### update_infra()
```

### Comparing `bodosdk-2.0.0rc1/README.md` & `bodosdk-2.0.0rc2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
 my_workspace = BodoWorkspaceClient()
 my_cluster = my_workspace.ClusterClient.get("cluster_id")
 if my_cluster.status != 'STOPPED':
     my_cluster.stop(wait=True)
 my_cluster.update(instance_type='c5.2xlarge', workers_quantity=2)
 ```
 
-### Create Fisrst Job
+### Create First Job
 
 On running cluster you can schedule a job in very simple way:
 First on `https://platform.bodo.ai` navigate to notebook in your workspace and
 create following `test.py` file in your main directory:
 
 ```python
 import pandas as pd
```

### Comparing `bodosdk-2.0.0rc1/bodosdk/api/auth.py` & `bodosdk-2.0.0rc2/bodosdk/api/auth.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc1/bodosdk/api/base.py` & `bodosdk-2.0.0rc2/bodosdk/api/base.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc1/bodosdk/api/billing.py` & `bodosdk-2.0.0rc2/bodosdk/api/billing.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc1/bodosdk/api/catalog.py` & `bodosdk-2.0.0rc2/bodosdk/api/catalog.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc1/bodosdk/api/cloud_config.py` & `bodosdk-2.0.0rc2/bodosdk/api/cloud_config.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc1/bodosdk/api/cluster.py` & `bodosdk-2.0.0rc2/bodosdk/api/cluster.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc1/bodosdk/api/instance_role.py` & `bodosdk-2.0.0rc2/bodosdk/api/instance_role.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc1/bodosdk/api/job.py` & `bodosdk-2.0.0rc2/bodosdk/api/job.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc1/bodosdk/api/job_tpl.py` & `bodosdk-2.0.0rc2/bodosdk/api/job_tpl.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc1/bodosdk/api/models/__init__.py` & `bodosdk-2.0.0rc2/bodosdk/api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc1/bodosdk/api/models/catalog.py` & `bodosdk-2.0.0rc2/bodosdk/api/models/catalog.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc1/bodosdk/api/models/cloud_config.py` & `bodosdk-2.0.0rc2/bodosdk/api/models/cloud_config.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc1/bodosdk/api/models/cluster.py` & `bodosdk-2.0.0rc2/bodosdk/api/models/cluster.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc1/bodosdk/api/models/instance_role.py` & `bodosdk-2.0.0rc2/bodosdk/api/models/instance_role.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc1/bodosdk/api/models/job.py` & `bodosdk-2.0.0rc2/bodosdk/api/models/job.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc1/bodosdk/api/models/workspace.py` & `bodosdk-2.0.0rc2/bodosdk/api/models/workspace.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc1/bodosdk/api/request_wrapper.py` & `bodosdk-2.0.0rc2/bodosdk/api/request_wrapper.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc1/bodosdk/api/secret_group.py` & `bodosdk-2.0.0rc2/bodosdk/api/secret_group.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc1/bodosdk/api/secrets.py` & `bodosdk-2.0.0rc2/bodosdk/api/secrets.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc1/bodosdk/api/workspace.py` & `bodosdk-2.0.0rc2/bodosdk/api/workspace.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc1/bodosdk/base.py` & `bodosdk-2.0.0rc2/bodosdk/base.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc1/bodosdk/clients/catalog.py` & `bodosdk-2.0.0rc2/bodosdk/clients/catalog.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc1/bodosdk/clients/cluster.py` & `bodosdk-2.0.0rc2/bodosdk/clients/cluster.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc1/bodosdk/clients/instance_role.py` & `bodosdk-2.0.0rc2/bodosdk/clients/instance_role.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc1/bodosdk/clients/job.py` & `bodosdk-2.0.0rc2/bodosdk/clients/job.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc1/bodosdk/clients/job_tpl.py` & `bodosdk-2.0.0rc2/bodosdk/clients/job_tpl.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc1/bodosdk/clients/organization.py` & `bodosdk-2.0.0rc2/bodosdk/clients/organization.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc1/bodosdk/clients/secret.py` & `bodosdk-2.0.0rc2/bodosdk/clients/secret.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc1/bodosdk/clients/workspace.py` & `bodosdk-2.0.0rc2/bodosdk/clients/workspace.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc1/bodosdk/db/connection.py` & `bodosdk-2.0.0rc2/bodosdk/db/connection.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc1/bodosdk/deprecation_decorator.py` & `bodosdk-2.0.0rc2/bodosdk/deprecation_decorator.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc1/bodosdk/interfaces.py` & `bodosdk-2.0.0rc2/bodosdk/interfaces.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc1/bodosdk/models/__init__.py` & `bodosdk-2.0.0rc2/bodosdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc1/bodosdk/models/catalog.py` & `bodosdk-2.0.0rc2/bodosdk/models/catalog.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc1/bodosdk/models/cloud_config.py` & `bodosdk-2.0.0rc2/bodosdk/models/cloud_config.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc1/bodosdk/models/cluster.py` & `bodosdk-2.0.0rc2/bodosdk/models/cluster.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc1/bodosdk/models/common.py` & `bodosdk-2.0.0rc2/bodosdk/models/common.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc1/bodosdk/models/instance_role.py` & `bodosdk-2.0.0rc2/bodosdk/models/instance_role.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc1/bodosdk/models/job.py` & `bodosdk-2.0.0rc2/bodosdk/models/job.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc1/bodosdk/models/secret.py` & `bodosdk-2.0.0rc2/bodosdk/models/secret.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc1/bodosdk/models/workspace.py` & `bodosdk-2.0.0rc2/bodosdk/models/workspace.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc1/bodosdk.egg-info/PKG-INFO` & `bodosdk-2.0.0rc2/bodosdk.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: bodosdk
-Version: 2.0.0rc1
-Summary: Bodo Platform SDK 2.0.0RC1
+Version: 2.0.0rc2
+Summary: Bodo Platform SDK 2.0.0RC2
 Home-page: https://github.com/Bodo-inc/bodo-sdk
 Author: Bodo, Inc.
 Author-email: noreply@bodo.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -150,15 +150,15 @@
 my_workspace = BodoWorkspaceClient()
 my_cluster = my_workspace.ClusterClient.get("cluster_id")
 if my_cluster.status != 'STOPPED':
     my_cluster.stop(wait=True)
 my_cluster.update(instance_type='c5.2xlarge', workers_quantity=2)
 ```
 
-### Create Fisrst Job
+### Create First Job
 
 On running cluster you can schedule a job in very simple way:
 First on `https://platform.bodo.ai` navigate to notebook in your workspace and
 create following `test.py` file in your main directory:
 
 ```python
 import pandas as pd
@@ -597,267 +597,267 @@
 
  #INDEX 
 
 # bodosdk package contents
 
 <a id="module-bodosdk.clients.cluster"></a>
 
-### _class_ bodosdk.clients.cluster.ClusterClient(workspace_client: IBodoWorkspaceClient)
+### *class* bodosdk.clients.cluster.ClusterClient(workspace_client: IBodoWorkspaceClient)
 
 Bases: `IClusterClient`
 
 A client for managing cluster operations in a Bodo workspace.
 
 #### \_deprecated_methods
 
 A dictionary of deprecated methods.
 
-- **Type:**
+* **Type:**
   Dict
 
 #### \_images
 
 A list of available Bodo images.
 
-- **Type:**
+* **Type:**
   List[IBodoImage]
 
-- **Parameters:**
-  **workspace_client** (_IBodoWorkspaceClient_) – The workspace client used for operations.
+* **Parameters:**
+  **workspace_client** (*IBodoWorkspaceClient*) – The workspace client used for operations.
 
-#### _property_ Cluster _: [Cluster](#bodosdk.models.cluster.Cluster)_
+#### *property* Cluster *: [Cluster](#bodosdk.models.cluster.Cluster)*
 
 Provides access to cluster operations.
 
-- **Returns:**
+* **Returns:**
   An instance of Cluster for cluster operations.
-- **Return type:**
+* **Return type:**
   [Cluster](#bodosdk.models.cluster.Cluster)
 
-#### _property_ ClusterList _: [ClusterList](#bodosdk.models.cluster.ClusterList)_
+#### *property* ClusterList *: [ClusterList](#bodosdk.models.cluster.ClusterList)*
 
 Provides access to listing clusters.
 
-- **Returns:**
+* **Returns:**
   An instance of ClusterListAPIModel for listing clusters.
-- **Return type:**
+* **Return type:**
   [ClusterList](#bodosdk.models.cluster.ClusterList)
 
 #### connect(catalog: str, cluster_id: str)
 
 #### create(name: str, instance_type: str = None, workers_quantity: int = None, description: str | None = None, bodo_version: str = None, auto_stop: int | None = None, auto_pause: int | None = None, image_id: str | None = None, accelerated_networking: bool | None = None, auto_az: bool | None = None, use_spot_instance: bool | None = None, aws_deployment_subnet_id: str | None = None, availability_zone: str | None = None, instance_role: [InstanceRole](#bodosdk.models.instance_role.InstanceRole) | Dict | None = None, custom_tags: Dict | None = None)
 
 Creates a new cluster with the specified configuration.
 
-- **Parameters:**
-  - **name** (_str_) – The name of the cluster.
-  - **instance_type** (_str_ _,_ _optional_) – The type of instance to use for the cluster nodes.
-  - **workers_quantity** (_int_ _,_ _optional_) – The number of worker nodes in the cluster.
-  - **description** (_str_ _,_ _optional_) – A description of the cluster.
-  - **bodo_version** (_str_ _,_ _optional_) – The Bodo version to use for the cluster.
-  - **auto_stop** (_int_ _,_ _optional_) – The auto-stop time in minutes for the cluster.
-  - **auto_pause** (_int_ _,_ _optional_) – The auto-pause time in minutes for the cluster.
-  - **image_id** (_str_ _,_ _optional_) – The ID of the image to use for the cluster.
-  - **accelerated_networking** (_bool_ _,_ _optional_) – Whether to use accelerated networking.
-  - **auto_az** (_bool_ _,_ _optional_) – Whether to automatically select the availability zone.
-  - **use_spot_instance** (_bool_ _,_ _optional_) – Whether to use spot instances for the cluster.
-  - **aws_deployment_subnet_id** (_str_ _,_ _optional_) – The AWS deployment subnet ID.
-  - **availability_zone** (_str_ _,_ _optional_) – The availability zone for the cluster.
-  - **instance_role** ([_InstanceRole_](#bodosdk.models.instance_role.InstanceRole) _|_ _Dict_ _,_ _optional_) – The instance role or a custom role configuration.
-  - **custom_tags** (_Dict_ _,_ _optional_) – Custom tags to assign to the cluster resources.
-- **Returns:**
+* **Parameters:**
+  * **name** (*str*) – The name of the cluster.
+  * **instance_type** (*str* *,* *optional*) – The type of instance to use for the cluster nodes.
+  * **workers_quantity** (*int* *,* *optional*) – The number of worker nodes in the cluster.
+  * **description** (*str* *,* *optional*) – A description of the cluster.
+  * **bodo_version** (*str* *,* *optional*) – The Bodo version to use for the cluster.
+  * **auto_stop** (*int* *,* *optional*) – The auto-stop time in minutes for the cluster.
+  * **auto_pause** (*int* *,* *optional*) – The auto-pause time in minutes for the cluster.
+  * **image_id** (*str* *,* *optional*) – The ID of the image to use for the cluster.
+  * **accelerated_networking** (*bool* *,* *optional*) – Whether to use accelerated networking.
+  * **auto_az** (*bool* *,* *optional*) – Whether to automatically select the availability zone.
+  * **use_spot_instance** (*bool* *,* *optional*) – Whether to use spot instances for the cluster.
+  * **aws_deployment_subnet_id** (*str* *,* *optional*) – The AWS deployment subnet ID.
+  * **availability_zone** (*str* *,* *optional*) – The availability zone for the cluster.
+  * **instance_role** ([*InstanceRole*](#bodosdk.models.instance_role.InstanceRole) *|* *Dict* *,* *optional*) – The instance role or a custom role configuration.
+  * **custom_tags** (*Dict* *,* *optional*) – Custom tags to assign to the cluster resources.
+* **Returns:**
   The created Cluster object.
-- **Return type:**
+* **Return type:**
   [Cluster](#bodosdk.models.cluster.Cluster)
 
 #### get(id: str)
 
 Retrieves a cluster by its ID.
 
-- **Parameters:**
-  **id** (_str_) – The ID of the cluster to retrieve.
-- **Returns:**
+* **Parameters:**
+  **id** (*str*) – The ID of the cluster to retrieve.
+* **Returns:**
   The retrieved Cluster object.
-- **Return type:**
+* **Return type:**
   [Cluster](#bodosdk.models.cluster.Cluster)
 
 #### get_bodo_versions()
 
 Retrieves a list of available Bodo versions.
 
-- **Returns:**
+* **Returns:**
   A list of available Bodo versions.
-- **Return type:**
+* **Return type:**
   List[str]
 
 #### get_images()
 
 Retrieves a list of available images.
 
-- **Returns:**
+* **Returns:**
   A list of image IDs available for clusters.
-- **Return type:**
+* **Return type:**
   List[str]
 
 #### get_instance_types()
 
 Retrieves list of all supported instance types
 
-- **Returns:**
+* **Returns:**
   List[InstanceType]
 
-#### _property_ latest*bodo_version *: str\_
+#### *property* latest_bodo_version *: str*
 
 Retrieves the latest Bodo version available.
 
-- **Returns:**
+* **Returns:**
   The latest Bodo version.
-- **Return type:**
+* **Return type:**
   str
 
 #### list(filters: Dict | [ClusterFilter](#bodosdk.models.cluster.ClusterFilter) | None = None, order: Dict | None = None)
 
 Lists clusters based on the provided filters and order.
 
-- **Parameters:**
-  - **filters** (_Dict_ _|_ [_ClusterFilter_](#bodosdk.models.cluster.ClusterFilter) _,_ _optional_) – The filters to apply to the cluster listing.
-  - **order** (_Dict_ _,_ _optional_) – The order in which to list the clusters.
-- **Returns:**
+* **Parameters:**
+  * **filters** (*Dict* *|* [*ClusterFilter*](#bodosdk.models.cluster.ClusterFilter) *,* *optional*) – The filters to apply to the cluster listing.
+  * **order** (*Dict* *,* *optional*) – The order in which to list the clusters.
+* **Returns:**
   A list of clusters matching the criteria.
-- **Return type:**
+* **Return type:**
   [ClusterList](#bodosdk.models.cluster.ClusterList)
 
 #### pause(id: str, wait=False)
 
 Pauses the specified cluster.
 
-- **Parameters:**
-  **id** (_str_) – The ID of the cluster to pause.
-- **Returns:**
+* **Parameters:**
+  **id** (*str*) – The ID of the cluster to pause.
+* **Returns:**
   The paused Cluster object.
-- **Return type:**
+* **Return type:**
   [Cluster](#bodosdk.models.cluster.Cluster)
 
 #### remove(id: str, wait=False)
 
 Removes the specified cluster.
 
-- **Parameters:**
-  **id** (_str_) – The ID of the cluster to remove.
-- **Returns:**
+* **Parameters:**
+  **id** (*str*) – The ID of the cluster to remove.
+* **Returns:**
   None
 
 #### resume(id: str, wait=False)
 
 Resumes the specified paused cluster.
 
-- **Parameters:**
-  **id** (_str_) – The ID of the cluster to resume.
-- **Returns:**
+* **Parameters:**
+  **id** (*str*) – The ID of the cluster to resume.
+* **Returns:**
   The resumed Cluster object.
-- **Return type:**
+* **Return type:**
   [Cluster](#bodosdk.models.cluster.Cluster)
 
 #### scale(id: str, new_size: int)
 
 Scales the specified cluster to the new size.
 
-- **Parameters:**
-  - **id** (_str_) – The ID of the cluster to scale.
-  - **new_size** (_int_) – The new size for the cluster in terms of the number of worker nodes.
-- **Returns:**
+* **Parameters:**
+  * **id** (*str*) – The ID of the cluster to scale.
+  * **new_size** (*int*) – The new size for the cluster in terms of the number of worker nodes.
+* **Returns:**
   The scaled Cluster object.
-- **Return type:**
+* **Return type:**
   [Cluster](#bodosdk.models.cluster.Cluster)
 
 #### start(id: str, wait=False)
 
 Starts the specified stopped cluster.
 
-- **Parameters:**
-  **id** (_str_) – The ID of the cluster to start.
-- **Returns:**
+* **Parameters:**
+  **id** (*str*) – The ID of the cluster to start.
+* **Returns:**
   The started Cluster object.
-- **Return type:**
+* **Return type:**
   [Cluster](#bodosdk.models.cluster.Cluster)
 
 #### stop(id: str, wait=False)
 
 Stops the specified cluster.
 
-- **Parameters:**
-  **id** (_str_) – The ID of the cluster to stop.
-- **Returns:**
+* **Parameters:**
+  **id** (*str*) – The ID of the cluster to stop.
+* **Returns:**
   The stopped Cluster object.
-- **Return type:**
+* **Return type:**
   [Cluster](#bodosdk.models.cluster.Cluster)
 
 #### update(id: str, name: str | None = None, description: str | None = None, auto_stop: int | None = None, auto_pause: int | None = None, workers_quantity: int | None = None, instance_role: [InstanceRole](#bodosdk.models.instance_role.InstanceRole) | Dict | None = None, instance_type: str | None = None, bodo_version: str | None = None, auto_az: bool | None = None, availability_zone: str | None = None, custom_tags: Dict | None = None)
 
 Updates the specified cluster with the given configuration.
 
-- **Parameters:**
-  - **id** (_str_) – The ID of the cluster to update.
-  - **name** (_str_ _,_ _optional_) – The new name for the cluster.
-  - **description** (_str_ _,_ _optional_) – A new description for the cluster.
-  - **auto_stop** (_int_ _,_ _optional_) – The new auto-stop time in minutes.
-  - **auto_pause** (_int_ _,_ _optional_) – The new auto-pause time in minutes.
-  - **workers_quantity** (_int_ _,_ _optional_) – The new number of worker nodes.
-  - **instance_role** ([_InstanceRole_](#bodosdk.models.instance_role.InstanceRole) _|_ _Dict_ _,_ _optional_) – The new instance role or custom role configuration.
-  - **instance_type** (_str_ _,_ _optional_) – The new instance type for the cluster nodes.
-  - **bodo_version** (_str_ _,_ _optional_) – The new Bodo version for the cluster.
-  - **auto_az** (_bool_ _,_ _optional_) – Whether to automatically select the availability zone.
-  - **availability_zone** (_str_ _,_ _optional_) – The new availability zone for the cluster.
-  - **custom_tags** (_Dict_ _,_ _optional_) – New custom tags for the cluster resources.
-- **Returns:**
+* **Parameters:**
+  * **id** (*str*) – The ID of the cluster to update.
+  * **name** (*str* *,* *optional*) – The new name for the cluster.
+  * **description** (*str* *,* *optional*) – A new description for the cluster.
+  * **auto_stop** (*int* *,* *optional*) – The new auto-stop time in minutes.
+  * **auto_pause** (*int* *,* *optional*) – The new auto-pause time in minutes.
+  * **workers_quantity** (*int* *,* *optional*) – The new number of worker nodes.
+  * **instance_role** ([*InstanceRole*](#bodosdk.models.instance_role.InstanceRole) *|* *Dict* *,* *optional*) – The new instance role or custom role configuration.
+  * **instance_type** (*str* *,* *optional*) – The new instance type for the cluster nodes.
+  * **bodo_version** (*str* *,* *optional*) – The new Bodo version for the cluster.
+  * **auto_az** (*bool* *,* *optional*) – Whether to automatically select the availability zone.
+  * **availability_zone** (*str* *,* *optional*) – The new availability zone for the cluster.
+  * **custom_tags** (*Dict* *,* *optional*) – New custom tags for the cluster resources.
+* **Returns:**
   The updated Cluster object.
-- **Return type:**
+* **Return type:**
   [Cluster](#bodosdk.models.cluster.Cluster)
 
 #### wait_for_status(id: str, statuses: List, timeout: int | None = 300, tick: int | None = 30)
 
 Waits for the specified cluster to reach any of the given statuses within the timeout period.
 
-- **Parameters:**
-  - **id** (_str_) – The ID of the cluster to monitor.
-  - **statuses** (_List_) – The list of statuses to wait for.
-  - **timeout** (_int_ _,_ _optional_) – The timeout period in seconds.
-  - **tick** (_int_ _,_ _optional_) – The interval in seconds between status checks.
-- **Returns:**
+* **Parameters:**
+  * **id** (*str*) – The ID of the cluster to monitor.
+  * **statuses** (*List*) – The list of statuses to wait for.
+  * **timeout** (*int* *,* *optional*) – The timeout period in seconds.
+  * **tick** (*int* *,* *optional*) – The interval in seconds between status checks.
+* **Returns:**
   The Cluster object if it reaches the desired status within the timeout period.
-- **Return type:**
+* **Return type:**
   [Cluster](#bodosdk.models.cluster.Cluster)
 
 <a id="module-bodosdk.clients.instance_role"></a>
 
-### _class_ bodosdk.clients.instance_role.InstanceRoleClient(workspace_client: IBodoWorkspaceClient)
+### *class* bodosdk.clients.instance_role.InstanceRoleClient(workspace_client: IBodoWorkspaceClient)
 
 Bases: `IInstanceRoleClient`
 
-#### _property_ InstanceRole _: [InstanceRole](#bodosdk.models.instance_role.InstanceRole)_
+#### *property* InstanceRole *: [InstanceRole](#bodosdk.models.instance_role.InstanceRole)*
 
-#### _property_ InstanceRoleList _: [InstanceRoleList](#bodosdk.models.instance_role.InstanceRoleList)_
+#### *property* InstanceRoleList *: [InstanceRoleList](#bodosdk.models.instance_role.InstanceRoleList)*
 
 #### create(role_arn: str, description: str, name: str = None)
 
 #### delete(id: str)
 
 #### get(id: str)
 
 #### list(filters: Dict | [InstanceRoleFilter](#bodosdk.models.instance_role.InstanceRoleFilter) | None = None, order: Dict | None = None)
 
 <a id="module-bodosdk.clients.job"></a>
 
-### _class_ bodosdk.clients.job.JobClient(workspace_client: IBodoWorkspaceClient)
+### *class* bodosdk.clients.job.JobClient(workspace_client: IBodoWorkspaceClient)
 
 Bases: `IJobClient`
 
-#### _property_ JobRun _: [JobRun](#bodosdk.models.job.JobRun)_
+#### *property* JobRun *: [JobRun](#bodosdk.models.job.JobRun)*
 
-#### _property_ JobRunList _: [JobRunList](#bodosdk.models.job.JobRunList)_
+#### *property* JobRunList *: [JobRunList](#bodosdk.models.job.JobRunList)*
 
 #### cancel_job(id: str)
 
 #### cancel_jobs(filters: Dict | [JobFilter](#bodosdk.models.job.JobFilter) | None = None)
 
 #### get(id: str)
 
@@ -867,47 +867,47 @@
 
 #### run_sql_query(template_id: str = None, catalog: str = None, sql_query: str = None, cluster: dict | ICluster = None, name: str = None, args: dict = None, timeout: int = None, num_retries: int = None, delay_between_retries: int = None, retry_on_timeout: bool = None)
 
 #### wait_for_status(id: str, statuses: List[str], timeout: int = 3600, tick: int = 30)
 
 <a id="module-bodosdk.clients.job_tpl"></a>
 
-### _class_ bodosdk.clients.job_tpl.JobTemplateClient(workspace_client: IBodoWorkspaceClient)
+### *class* bodosdk.clients.job_tpl.JobTemplateClient(workspace_client: IBodoWorkspaceClient)
 
 Bases: `IJobTemplateClient`
 
-#### _property_ JobTemplate _: [JobTemplate](#bodosdk.models.job.JobTemplate)_
+#### *property* JobTemplate *: [JobTemplate](#bodosdk.models.job.JobTemplate)*
 
-#### _property_ JobTemplateList _: [JobTemplateList](#bodosdk.models.job.JobTemplateList)_
+#### *property* JobTemplateList *: [JobTemplateList](#bodosdk.models.job.JobTemplateList)*
 
 #### create(name: str = None, description: str = None, cluster: dict | ICluster = None, code_type: str = None, source: dict | IS3Source | IGitRepoSource | IWorkspaceSource | ITextSource = None, exec_file: str = None, exec_text: str = None, args: dict | str = None, env_vars: dict = None, timeout: int = None, num_retries: int = None, delay_between_retries: int = None, retry_on_timeout: bool = None, catalog: str = None)
 
 #### get(id: str)
 
 #### list(filters: Dict = None)
 
 #### remove(id: str)
 
 <a id="module-bodosdk.clients.organization"></a>
 
-### _class_ bodosdk.clients.organization.BodoOrganizationClient(client_id=None, secret_key=None, api_url='https://api.bodo.ai/api', auth_url='https://auth.bodo.ai', print_logs=False)
+### *class* bodosdk.clients.organization.BodoOrganizationClient(client_id=None, secret_key=None, api_url='https://api.bodo.ai/api', auth_url='https://auth.bodo.ai', print_logs=False)
 
 Bases: `IBodoOrganizationClient`
 
-#### _property_ AwsCloudConfig _: [AwsCloudConfig](#bodosdk.models.cloud_config.AwsCloudConfig)_
+#### *property* AwsCloudConfig *: [AwsCloudConfig](#bodosdk.models.cloud_config.AwsCloudConfig)*
 
-#### _property_ AzureCloudConfig _: [AzureCloudConfig](#bodosdk.models.cloud_config.AzureCloudConfig)_
+#### *property* AzureCloudConfig *: [AzureCloudConfig](#bodosdk.models.cloud_config.AzureCloudConfig)*
 
-#### _property_ CloudConfig _: [CloudConfigBase](#bodosdk.models.cloud_config.CloudConfigBase)_
+#### *property* CloudConfig *: [CloudConfigBase](#bodosdk.models.cloud_config.CloudConfigBase)*
 
-#### _property_ CloudConfigList _: [CloudConfigList](#bodosdk.models.cloud_config.CloudConfigList)_
+#### *property* CloudConfigList *: [CloudConfigList](#bodosdk.models.cloud_config.CloudConfigList)*
 
-#### _property_ Workspace _: [Workspace](#bodosdk.models.workspace.Workspace)_
+#### *property* Workspace *: [Workspace](#bodosdk.models.workspace.Workspace)*
 
-#### _property_ WorkspaceList _: [WorkspaceList](#bodosdk.models.workspace.WorkspaceList)_
+#### *property* WorkspaceList *: [WorkspaceList](#bodosdk.models.workspace.WorkspaceList)*
 
 #### create_workspace(name: str, region: str, storage_endpoint_enabled: bool, cloud_config_id: str = None, vpc_id: str | None = None, public_subnets_ids: List[str] | None = None, private_subnets_ids: List[str] | None = None, custom_tags: dict | None = None)
 
 #### delete_workspace(id)
 
 #### get_cloud_config(id)
 
@@ -915,2277 +915,2271 @@
 
 #### list_cloud_configs(filters: dict | None = None)
 
 #### list_workspaces(filters: [WorkspaceFilter](#bodosdk.models.workspace.WorkspaceFilter) | dict | None = None)
 
 <a id="module-bodosdk.clients.workspace"></a>
 
-### _class_ bodosdk.clients.workspace.BodoWorkspaceClient(client_id=None, secret_key=None, api_url='https://api.bodo.ai/api', auth_url='https://auth.bodo.ai', print_logs=False)
+### *class* bodosdk.clients.workspace.BodoWorkspaceClient(client_id=None, secret_key=None, api_url='https://api.bodo.ai/api', auth_url='https://auth.bodo.ai', print_logs=False)
 
 Bases: `IBodoWorkspaceClient`
 
-#### ClusterClient _: IClusterClient_
+#### ClusterClient *: IClusterClient*
 
-#### JobClient _: IJobClient_
+#### JobClient *: IJobClient*
 
-#### JobTemplateClient _: IJobTemplateClient_
+#### JobTemplateClient *: IJobTemplateClient*
 
-#### _property_ workspace*data *: IWorkspace\_
+#### *property* workspace_data *: IWorkspace*
 
-#### _property_ workspace*id *: str\_
+#### *property* workspace_id *: str*
 
 <a id="module-bodosdk.models.catalog"></a>
 
-### _class_ bodosdk.models.catalog.Catalog(workspace_client: IBodoWorkspaceClient = None, \*, uuid: str | None = None, name: str | None = None, description: str | None = None, catalogType: str | None = None, details: [SnowflakeDetails](#bodosdk.models.catalog.SnowflakeDetails) | dict | None = None)
+### *class* bodosdk.models.catalog.Catalog(workspace_client: IBodoWorkspaceClient = None, \*, uuid: str | None = None, name: str | None = None, description: str | None = None, catalogType: str | None = None, details: [SnowflakeDetails](#bodosdk.models.catalog.SnowflakeDetails) | dict | None = None)
 
 Bases: `SDKBaseModel`, `ICatalog`
 
 #### delete()
 
-### _class_ bodosdk.models.catalog.CatalogFilter(\*, names: List[str] | None = None, ids: List[str] | None = None)
+### *class* bodosdk.models.catalog.CatalogFilter(\*, names: List[str] | None = None, ids: List[str] | None = None)
 
 Bases: `SDKBaseModel`, `ICatalogFilter`
 
-#### ids _: List[str] | None_
+#### ids *: List[str] | None*
 
-#### names _: List[str] | None_
+#### names *: List[str] | None*
 
-### _class_ bodosdk.models.catalog.CatalogList(workspace_client: IBodoWorkspaceClient = None, \*, page: int | None = 0, pageSize: int | None = 10, total: int | None = None, order: dict | None = None, filters: dict | [CatalogFilter](#bodosdk.models.catalog.CatalogFilter) | None = None)
+### *class* bodosdk.models.catalog.CatalogList(workspace_client: IBodoWorkspaceClient = None, \*, page: int | None = 0, pageSize: int | None = 10, total: int | None = None, order: dict | None = None, filters: dict | [CatalogFilter](#bodosdk.models.catalog.CatalogFilter) | None = None)
 
 Bases: `ICatalogList`, `SDKBaseModel`
 
-#### _class_ Config
+#### *class* Config
 
 Bases: `object`
 
 Configuration for Pydantic models.
 [https://docs.pydantic.dev/latest/api/config/](https://docs.pydantic.dev/latest/api/config/)
 
-#### allow*population_by_field_name *= True\_
+#### allow_population_by_field_name *= True*
 
-#### extra _= 'forbid'_
+#### extra *= 'forbid'*
 
 #### delete()
 
-#### filters _: dict | [CatalogFilter](#bodosdk.models.catalog.CatalogFilter) | None_
+#### filters *: dict | [CatalogFilter](#bodosdk.models.catalog.CatalogFilter) | None*
 
-#### order _: dict | None_
+#### order *: dict | None*
 
-#### page _: int | None_
+#### page *: int | None*
 
-#### page*size *: int | None\_
+#### page_size *: int | None*
 
-#### total _: int | None_
+#### total *: int | None*
 
-### _class_ bodosdk.models.catalog.SnowflakeDetails(\*, port: int | None = None, db_schema: str | None = None, database: str | None = None, userRole: str | None = None, username: str | None = None, warehouse: str | None = None, accountName: str | None = None, password: str | None = None)
+### *class* bodosdk.models.catalog.SnowflakeDetails(\*, port: int | None = None, db_schema: str | None = None, database: str | None = None, userRole: str | None = None, username: str | None = None, warehouse: str | None = None, accountName: str | None = None, password: str | None = None)
 
 Bases: `SDKBaseModel`
 
-#### account*name *: str | None\_
+#### account_name *: str | None*
 
-#### database _: str | None_
+#### database *: str | None*
 
-#### db*schema *: str | None\_
+#### db_schema *: str | None*
 
-#### password _: str | None_
+#### password *: str | None*
 
-#### port _: int | None_
+#### port *: int | None*
 
-#### user*role *: str | None\_
+#### user_role *: str | None*
 
-#### username _: str | None_
+#### username *: str | None*
 
-#### warehouse _: str | None_
+#### warehouse *: str | None*
 
 <a id="module-bodosdk.models.cloud_config"></a>
 
-### _class_ bodosdk.models.cloud_config.AwsCloudConfig(org_client: IBodoOrganizationClient = None, \*, cloudProvider: str | None = None, name: str | None = None, status: str | None = None, organizationUUID: str | None = None, customTags: dict | None = None, uuid: str | UUID | None = None, awsProviderData: [AwsProviderData](#bodosdk.models.cloud_config.AwsProviderData) | None = None)
+### *class* bodosdk.models.cloud_config.AwsCloudConfig(org_client: IBodoOrganizationClient = None, \*, cloudProvider: str | None = None, name: str | None = None, status: str | None = None, organizationUUID: str | None = None, customTags: dict | None = None, uuid: str | UUID | None = None, awsProviderData: [AwsProviderData](#bodosdk.models.cloud_config.AwsProviderData) | None = None)
 
 Bases: [`CloudConfigBase`](#bodosdk.models.cloud_config.CloudConfigBase), `IAwsCloudConfig`
 
-#### data _: [AwsProviderData](#bodosdk.models.cloud_config.AwsProviderData) | None_
+#### data *: [AwsProviderData](#bodosdk.models.cloud_config.AwsProviderData) | None*
 
-### _class_ bodosdk.models.cloud_config.AwsProviderData(\*, roleArn: str | None = None, tfBucketName: str | None = None, tfDynamoDbTableName: str | None = None, tfBackendRegion: str | None = None, externalId: str | None = None, accountId: str | None = None)
+### *class* bodosdk.models.cloud_config.AwsProviderData(\*, roleArn: str | None = None, tfBucketName: str | None = None, tfDynamoDbTableName: str | None = None, tfBackendRegion: str | None = None, externalId: str | None = None, accountId: str | None = None)
 
 Bases: `SDKBaseModel`, `IAwsProviderData`
 
-#### account*id *: str | None\_
+#### account_id *: str | None*
 
-#### external*id *: str | None\_
+#### external_id *: str | None*
 
-#### role*arn *: str | None\_
+#### role_arn *: str | None*
 
-#### tf*backend_region *: str | None\_
+#### tf_backend_region *: str | None*
 
-#### tf*bucket_name *: str | None\_
+#### tf_bucket_name *: str | None*
 
-#### tf*dynamo_db_table_name *: str | None\_
+#### tf_dynamo_db_table_name *: str | None*
 
-### _class_ bodosdk.models.cloud_config.AzureCloudConfig(org_client: IBodoOrganizationClient = None, \*, cloudProvider: str | None = None, name: str | None = None, status: str | None = None, organizationUUID: str | None = None, customTags: dict | None = None, uuid: str | UUID | None = None, azureProviderData: [AzureProviderData](#bodosdk.models.cloud_config.AzureProviderData) | None = None)
+### *class* bodosdk.models.cloud_config.AzureCloudConfig(org_client: IBodoOrganizationClient = None, \*, cloudProvider: str | None = None, name: str | None = None, status: str | None = None, organizationUUID: str | None = None, customTags: dict | None = None, uuid: str | UUID | None = None, azureProviderData: [AzureProviderData](#bodosdk.models.cloud_config.AzureProviderData) | None = None)
 
 Bases: [`CloudConfigBase`](#bodosdk.models.cloud_config.CloudConfigBase), `IAzureCloudConfig`
 
-#### data _: [AzureProviderData](#bodosdk.models.cloud_config.AzureProviderData) | None_
+#### data *: [AzureProviderData](#bodosdk.models.cloud_config.AzureProviderData) | None*
 
-### _class_ bodosdk.models.cloud_config.AzureProviderData(\*, tfBackendRegion: str | None = None, resourceGroup: str | None = None, subscriptionId: str | None = None, tenantId: str | None = None, tfStorageAccountName: str | None = None, applicationId: str | None = None)
+### *class* bodosdk.models.cloud_config.AzureProviderData(\*, tfBackendRegion: str | None = None, resourceGroup: str | None = None, subscriptionId: str | None = None, tenantId: str | None = None, tfStorageAccountName: str | None = None, applicationId: str | None = None)
 
 Bases: `SDKBaseModel`, `IAzureProviderData`
 
-#### application*id *: str | None\_
+#### application_id *: str | None*
 
-#### resource*group *: str | None\_
+#### resource_group *: str | None*
 
-#### subscription*id *: str | None\_
+#### subscription_id *: str | None*
 
-#### tenant*id *: str | None\_
+#### tenant_id *: str | None*
 
-#### tf*backend_region *: str | None\_
+#### tf_backend_region *: str | None*
 
-#### tf*storage_account_name *: str | None\_
+#### tf_storage_account_name *: str | None*
 
-### _class_ bodosdk.models.cloud_config.CloudConfigBase(org_client: IBodoOrganizationClient = None, \*, cloudProvider: str | None = None, name: str | None = None, status: str | None = None, organizationUUID: str | None = None, customTags: dict | None = None, uuid: str | UUID | None = None, data: [AwsProviderData](#bodosdk.models.cloud_config.AwsProviderData) | [AzureProviderData](#bodosdk.models.cloud_config.AzureProviderData) | None = None)
+### *class* bodosdk.models.cloud_config.CloudConfigBase(org_client: IBodoOrganizationClient = None, \*, cloudProvider: str | None = None, name: str | None = None, status: str | None = None, organizationUUID: str | None = None, customTags: dict | None = None, uuid: str | UUID | None = None, data: [AwsProviderData](#bodosdk.models.cloud_config.AwsProviderData) | [AzureProviderData](#bodosdk.models.cloud_config.AzureProviderData) | None = None)
 
 Bases: `SDKBaseModel`, `ICloudConfig`
 
-#### cloud*provider *: str | None\_
+#### cloud_provider *: str | None*
 
-#### custom*tags *: dict | None\_
+#### custom_tags *: dict | None*
 
-#### data _: [AwsProviderData](#bodosdk.models.cloud_config.AwsProviderData) | [AzureProviderData](#bodosdk.models.cloud_config.AzureProviderData) | None_
+#### data *: [AwsProviderData](#bodosdk.models.cloud_config.AwsProviderData) | [AzureProviderData](#bodosdk.models.cloud_config.AzureProviderData) | None*
 
 #### delete()
 
-#### _property_ id
+#### *property* id
 
-#### name _: str | None_
+#### name *: str | None*
 
-#### organization*uuid *: str | None\_
+#### organization_uuid *: str | None*
 
-#### status _: str | None_
+#### status *: str | None*
 
-#### uuid _: str | UUID | None_
+#### uuid *: str | UUID | None*
 
-### _class_ bodosdk.models.cloud_config.CloudConfigList(org_client: IBodoOrganizationClient = None, \*, page: int | None = 0, pageSize: int | None = 10, total: int | None = None, order: dict | None = None, filters: dict | None = None)
+### *class* bodosdk.models.cloud_config.CloudConfigList(org_client: IBodoOrganizationClient = None, \*, page: int | None = 0, pageSize: int | None = 10, total: int | None = None, order: dict | None = None, filters: dict | None = None)
 
 Bases: `ICloudConfigList`, `SDKBaseModel`
 
-#### _class_ Config
+#### *class* Config
 
 Bases: `object`
 
 Configuration for Pydantic models.
 [https://docs.pydantic.dev/latest/api/config/](https://docs.pydantic.dev/latest/api/config/)
 
-#### allow*population_by_field_name *= True\_
+#### allow_population_by_field_name *= True*
 
-#### extra _= 'forbid'_
+#### extra *= 'forbid'*
 
 #### delete()
 
-#### filters _: dict | None_
+#### filters *: dict | None*
 
-#### order _: dict | None_
+#### order *: dict | None*
 
-#### page _: int | None_
+#### page *: int | None*
 
-#### page*size *: int | None\_
+#### page_size *: int | None*
 
-#### total _: int | None_
+#### total *: int | None*
 
 <a id="module-bodosdk.models.cluster"></a>
 
-### _class_ bodosdk.models.cluster.BodoImage(\*, image_id: str, bodo_version: str)
+### *class* bodosdk.models.cluster.BodoImage(\*, image_id: str, bodo_version: str)
 
 Bases: `SDKBaseModel`
 
 Represents an image configuration for Bodo, encapsulating the image ID and the specific Bodo version.
 
 This class is a data model that holds information about a Bodo environment image.
 
 #### image_id
 
 The unique identifier for the Bodo image.
 
-- **Type:**
+* **Type:**
   str
 
 #### bodo_version
 
 The version of Bodo used in the image.
 
-- **Type:**
+* **Type:**
   str
 
-#### bodo*version *: str\_
+#### bodo_version *: str*
 
-#### image*id *: str\_
+#### image_id *: str*
 
-### _class_ bodosdk.models.cluster.Cluster(workspace_client: IBodoWorkspaceClient = None, \*, name: str | None = None, uuid: str | None = None, status: str | None = None, description: str | None = None, instanceType: str | None = None, workersQuantity: int | None = None, autoStop: int | None = None, autoPause: int | None = None, bodoVersion: str | None = None, imageId: str | None = None, coresPerWorker: int | None = None, acceleratedNetworking: bool | None = None, createdAt: datetime | None = None, updatedAt: datetime | None = None, isJobDedicated: bool | None = None, autoAZ: bool | None = None, useSpotInstance: bool | None = None, lastKnownActivity: datetime | None = None, inStateSince: datetime | None = None, clusterAgentVersion: str | None = None, clusterInitStatus: str | None = None, clusterHealthStatus: str | None = None, primaryAgentIP: str | None = None, awsDeploymentSubnetId: str | None = None, nodeMetadata: List[[NodeMetadata](#bodosdk.models.cluster.NodeMetadata)] | None = None, availabilityZone: str | None = None, instanceRole: [InstanceRole](#bodosdk.models.instance_role.InstanceRole) | None = None, workspace: dict | None = None, autoscalingIdentifier: str | None = None, lastAsgActivityId: str | None = None, nodesIp: List[str] | None = None, customTags: Dict | None = None)
+### *class* bodosdk.models.cluster.Cluster(workspace_client: IBodoWorkspaceClient = None, \*, name: str | None = None, uuid: str | None = None, status: str | None = None, description: str | None = None, instanceType: str | None = None, workersQuantity: int | None = None, autoStop: int | None = None, autoPause: int | None = None, bodoVersion: str | None = None, imageId: str | None = None, coresPerWorker: int | None = None, acceleratedNetworking: bool | None = None, createdAt: datetime | None = None, updatedAt: datetime | None = None, isJobDedicated: bool | None = None, autoAZ: bool | None = None, useSpotInstance: bool | None = None, lastKnownActivity: datetime | None = None, inStateSince: datetime | None = None, clusterAgentVersion: str | None = None, clusterInitStatus: str | None = None, clusterHealthStatus: str | None = None, primaryAgentIP: str | None = None, awsDeploymentSubnetId: str | None = None, nodeMetadata: List[[NodeMetadata](#bodosdk.models.cluster.NodeMetadata)] | None = None, availabilityZone: str | None = None, instanceRole: [InstanceRole](#bodosdk.models.instance_role.InstanceRole) | None = None, workspace: dict | None = None, autoscalingIdentifier: str | None = None, lastAsgActivityId: str | None = None, nodesIp: List[str] | None = None, customTags: Dict | None = None)
 
 Bases: `SDKBaseModel`, `ICluster`
 
 Represents a cluster in the SDK model, encapsulating various properties and operations
 related to a compute cluster.
 
 #### name
 
 The name of the cluster.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### uuid
 
 The unique identifier of the cluster.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### status
 
 The current status of the cluster (e.g., ‘RUNNING’, ‘STOPPED’).
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### description
 
 A description of the cluster.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### instance_type
 
 The type of instances used in the cluster (e.g., ‘c5.large’).
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### workers_quantity
 
 The number of worker nodes in the cluster.
 
-- **Type:**
+* **Type:**
   Optional[int]
 
 #### auto_stop
 
 The auto-stop configuration in minutes.
 The cluster automatically stops when idle for this duration.
 
-- **Type:**
+* **Type:**
   Optional[int]
 
 #### auto_pause
 
 The auto-pause configuration in minutes.
 The cluster automatically pauses when idle for this duration.
 
-- **Type:**
+* **Type:**
   Optional[int]
 
 #### bodo_version
 
 The version of Bodo being used in the cluster.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### image_id
 
 The ID of the image used for the cluster’s instances.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### cores_per_worker
 
 The number of CPU cores per worker node.
 
-- **Type:**
+* **Type:**
   Optional[int]
 
 #### accelerated_networking
 
 Whether accelerated networking is enabled.
 
-- **Type:**
+* **Type:**
   Optional[bool]
 
 #### created_at
 
 The creation timestamp of the cluster.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### updated_at
 
 The last update timestamp of the cluster.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### is_job_dedicated
 
 Whether the cluster is dedicated to a specific job.
 
-- **Type:**
+* **Type:**
   Optional[bool]
 
 #### auto_az
 
 Whether automatic availability zone selection is enabled.
 
-- **Type:**
+* **Type:**
   Optional[bool]
 
 #### use_spot_instance
 
 Whether spot instances are used for the cluster.
 
-- **Type:**
+* **Type:**
   Optional[bool]
 
 #### last_known_activity
 
 The last known activity timestamp of the cluster.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### in_state_since
 
 The timestamp since the cluster has been in its current state.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### cluster_agent_version
 
 The version of the cluster agent.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### cluster_init_status
 
 The initialization status of the cluster.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### cluster_health_status
 
 The health status of the cluster.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### primary_agent_ip
 
 The IP address of the primary agent in the cluster.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### aws_deployment_subnet_id
 
 The subnet ID used for deploying AWS resources.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### node_metadata
 
 Metadata information for each node in the cluster.
 
-- **Type:**
+* **Type:**
   Optional[List[[NodeMetadata](#bodosdk.models.cluster.NodeMetadata)]]
 
 #### availability_zone
 
 The AWS availability zone in which the cluster is located.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### instance_role
 
 The IAM role used by instances in the cluster.
 
-- **Type:**
+* **Type:**
   Optional[[InstanceRole](#bodosdk.models.instance_role.InstanceRole)]
 
 #### workspace
 
 A dictionary containing workspace-related information for the cluster.
 
-- **Type:**
+* **Type:**
   Optional[dict]
 
 #### autoscaling_identifier
 
 The identifier for autoscaling configuration.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### last_asg_activity_id
 
 The identifier of the last activity in the autoscaling group.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### nodes_ip
 
 A list of IP addresses for the nodes in the cluster.
 
-- **Type:**
+* **Type:**
   Optional[List[str]]
 
-#### accelerated*networking *: bool | None\_
+#### accelerated_networking *: bool | None*
 
-#### auto*az *: bool | None\_
+#### auto_az *: bool | None*
 
-#### auto*pause *: int | None\_
+#### auto_pause *: int | None*
 
-#### auto*stop *: int | None\_
+#### auto_stop *: int | None*
 
-#### autoscaling*identifier *: str | None\_
+#### autoscaling_identifier *: str | None*
 
-#### availability*zone *: str | None\_
+#### availability_zone *: str | None*
 
-#### aws*deployment_subnet_id *: str | None\_
+#### aws_deployment_subnet_id *: str | None*
 
-#### bodo*version *: str | None\_
+#### bodo_version *: str | None*
 
 #### cancel_jobs()
 
 Cancels all jobs associated with the cluster.
 
-- **Returns:**
+* **Returns:**
   The Cluster instance.
 
-#### cluster*agent_version *: str | None\_
+#### cluster_agent_version *: str | None*
 
-#### cluster*health_status *: str | None\_
+#### cluster_health_status *: str | None*
 
-#### cluster*init_status *: str | None\_
+#### cluster_init_status *: str | None*
 
 #### connect(catalog: str)
 
 Establishes a connection to the specified catalog from Cluster.
 
 This method is responsible for creating and returning a new Connection instance based on the provided catalog.
 
 Parameters:
 catalog (str): The name of the catalog to which the connection should be established.
 
 Returns:
 Connection: An instance of Connection initialized with the specified catalog and the current class instance.
 
-#### cores*per_worker *: int | None\_
+#### cores_per_worker *: int | None*
 
-#### created*at *: datetime | None\_
+#### created_at *: datetime | None*
 
-#### custom*tags *: Dict | None\_
+#### custom_tags *: Dict | None*
 
 #### delete(force: bool = False, mark_as_terminated: bool = False, wait: bool = False)
 
 Deletes the cluster, optionally forcing removal or marking as terminated.
 
-- **Parameters:**
-  - **force** – If True, forces the deletion of the cluster.
-  - **mark_as_terminated** – If True, marks the cluster as terminated instead of deleting.
-  - **wait** – If True, waits till cluster will be TERMINATED.
-- **Returns:**
+* **Parameters:**
+  * **force** – If True, forces the deletion of the cluster.
+  * **mark_as_terminated** – If True, marks the cluster as terminated instead of deleting.
+  * **wait** – If True, waits till cluster will be TERMINATED.
+* **Returns:**
   The Cluster instance, potentially updated to reflect its new state.
 
 Handles:
 : ResourceNotFound: Silently if the cluster is already deleted or not found.
 
-#### description _: str | None_
+#### description *: str | None*
 
-#### _property_ id _: str_
+#### *property* id *: str*
 
 The UUID of the cluster.
 
-- **Returns:**
+* **Returns:**
   The UUID string of the cluster.
 
-#### image*id *: str | None\_
+#### image_id *: str | None*
 
-#### in*state_since *: datetime | None\_
+#### in_state_since *: datetime | None*
 
-#### instance*role *: [InstanceRole](#bodosdk.models.instance_role.InstanceRole) | None\_
+#### instance_role *: [InstanceRole](#bodosdk.models.instance_role.InstanceRole) | None*
 
-#### instance*type *: str | None\_
+#### instance_type *: str | None*
 
-#### is*job_dedicated *: bool | None\_
+#### is_job_dedicated *: bool | None*
 
-#### last*asg_activity_id *: str | None\_
+#### last_asg_activity_id *: str | None*
 
-#### last*known_activity *: datetime | None\_
+#### last_known_activity *: datetime | None*
 
-#### name _: str | None_
+#### name *: str | None*
 
-#### node*metadata *: List[[NodeMetadata](#bodosdk.models.cluster.NodeMetadata)] | None\_
+#### node_metadata *: List[[NodeMetadata](#bodosdk.models.cluster.NodeMetadata)] | None*
 
-#### nodes*ip *: List[str] | None\_
+#### nodes_ip *: List[str] | None*
 
 #### pause(wait: bool = False)
 
 Pauses the cluster if it is running.
 
-- **Parameters:**
+* **Parameters:**
   **wait** – If True, waits till cluster will be PAUSED.
-- **Returns:**
+* **Returns:**
   The Cluster instance with updated status.
-- **Raises:**
+* **Raises:**
   **ConflictException** – If the cluster cannot be paused due to its current status.
 
-#### primary*agent_ip *: str | None\_
+#### primary_agent_ip *: str | None*
 
 #### resume(wait: bool = False)
 
 Resumes the cluster if it was paused or stopped.
 
-- **Parameters:**
+* **Parameters:**
   **wait** – If True, waits till cluster will be RUNNING.
-- **Returns:**
+* **Returns:**
   The Cluster instance with updated status.
-- **Raises:**
+* **Raises:**
   **ConflictException** – If the cluster cannot be resumed due to its current status.
 
 #### run_job(template_id: str = None, code_type: str = None, source: dict | IS3Source | IGitRepoSource | IWorkspaceSource | ITextSource = None, exec_file: str = None, args: dict | str = None, env_vars: dict = None, timeout: int = None, num_retries: int = None, delay_between_retries: int = None, retry_on_timeout: bool = None, name: str = None, catalog: str = None)
 
 Submits a batch job for execution using specified configurations and resources.
 
 This method creates and dispatches a job within a computing cluster, allowing for extensive customization of
 execution parameters including source data, runtime environment, and failure handling strategies.
 
-- **Parameters:**
-  - **template_id** (_str_ _,_ _optional_) – Identifier for the job template to use.
-  - **code_type** (_str_ _,_ _optional_) – Type of code to execute (e.g., Python, Java).
-  - **source** (_Union_ _[\*\*dict_ _,_ _IS3Source_ _,_ _IGitRepoSource_ _,_ _IWorkspaceSource_ _,_ _ITextSource_ _]_ _,_ _optional_) – Source of the code to be executed. Can be specified as a dictionary
+* **Parameters:**
+  * **template_id** (*str* *,* *optional*) – Identifier for the job template to use.
+  * **code_type** (*str* *,* *optional*) – Type of code to execute (e.g., Python, Java).
+  * **source** (*Union* *[**dict* *,* *IS3Source* *,* *IGitRepoSource* *,* *IWorkspaceSource* *,* *ITextSource* *]* *,* *optional*) – Source of the code to be executed. Can be specified as a dictionary
     or an instance of one of the predefined source interfaces.
-  - **exec_file** (_str_ _,_ _optional_) – Path to the executable file within the source.
-  - **args** (_Union_ _[\*\*dict_ _,_ _str_ _]_ _,_ _optional_) – Arguments to pass to the executable.
-  - **parameters.** (_Can be a string_ _or_ _a dictionary of_) –
-  - **env_vars** (_dict_ _,_ _optional_) – Environment variables to set for the job.
-  - **timeout** (_int_ _,_ _optional_) – Maximum runtime (in seconds) before the job is terminated.
-  - **num_retries** (_int_ _,_ _optional_) – Number of times to retry the job on failure.
-  - **delay_between_retries** (_int_ _,_ _optional_) – Time to wait between retries.
-  - **retry_on_timeout** (_bool_ _,_ _optional_) – Whether to retry the job if it times out.
-  - **name** (_str_ _,_ _optional_) – Name of the job.
-  - **catalog** (_str_ _,_ _optional_) – Catalog to log the job under.
-- **Returns:**
+  * **exec_file** (*str* *,* *optional*) – Path to the executable file within the source.
+  * **args** (*Union* *[**dict* *,* *str* *]* *,* *optional*) – Arguments to pass to the executable.
+  * **parameters.** (*Can be a string* *or* *a dictionary of*) –
+  * **env_vars** (*dict* *,* *optional*) – Environment variables to set for the job.
+  * **timeout** (*int* *,* *optional*) – Maximum runtime (in seconds) before the job is terminated.
+  * **num_retries** (*int* *,* *optional*) – Number of times to retry the job on failure.
+  * **delay_between_retries** (*int* *,* *optional*) – Time to wait between retries.
+  * **retry_on_timeout** (*bool* *,* *optional*) – Whether to retry the job if it times out.
+  * **name** (*str* *,* *optional*) – Name of the job.
+  * **catalog** (*str* *,* *optional*) – Catalog to log the job under.
+* **Returns:**
   An object representing the submitted job, capable of providing status and results.
-- **Return type:**
+* **Return type:**
   IJobRun
 
 #### run_sql_query(template_id: str = None, catalog: str = None, sql_query: str = None, name: str = None, args: dict = None, timeout: int = None, num_retries: int = None, delay_between_retries: int = None, retry_on_timeout: bool = None)
 
 > Submits an SQL query for execution on the cluster, returning a job run object.
 
 > This method handles the execution of an SQL query within a defined cluster environment.
 > It supports customization of execution parameters such as query arguments,
 > job name, execution timeouts, and retry strategies.
 
 > Parameters:
 > : template_id (str, optional): Identifier for the job template to use.
-> catalog (str, optional): Catalog under which to log the SQL job.
-> sql_query (str, optional): The SQL query string to be executed.
-> name (str, optional): Descriptive name for the SQL job.
-> args (dict, optional): Dictionary of arguments that are passed to the SQL query.
-> timeout (int, optional): Maximum allowable runtime in seconds before the job is terminated.
-> num_retries (int, optional): Number of times the job will be retried on failure.
-> delay_between_retries (int, optional): Interval in seconds between job retries.
-> retry_on_timeout (bool, optional): Whether to retry the job if it times out.
+>   catalog (str, optional): Catalog under which to log the SQL job.
+>   sql_query (str, optional): The SQL query string to be executed.
+>   name (str, optional): Descriptive name for the SQL job.
+>   args (dict, optional): Dictionary of arguments that are passed to the SQL query.
+>   timeout (int, optional): Maximum allowable runtime in seconds before the job is terminated.
+>   num_retries (int, optional): Number of times the job will be retried on failure.
+>   delay_between_retries (int, optional): Interval in seconds between job retries.
+>   retry_on_timeout (bool, optional): Whether to retry the job if it times out.
 
 > Returns:
 > : IJobRun: An object representing the status and result of the executed SQL job.
 
 ```
 `
 ```
 
 #### start(wait: bool = False)
 
 Starts the cluster.
 
-- **Parameters:**
+* **Parameters:**
   **wait** – If True, waits till cluster will be RUNNING.
-- **Returns:**
+* **Returns:**
   The Cluster instance with updated status.
 
-#### status _: str | None_
+#### status *: str | None*
 
 #### stop(wait: bool = False)
 
 Stops the cluster.
 
-- **Parameters:**
+* **Parameters:**
   **wait** – If True, waits till cluster will be STOPPED.
-- **Returns:**
+* **Returns:**
   The Cluster instance with updated status.
 
 #### update(auto_stop: int | None = None, auto_pause: int | None = None, description: str | None = None, name: str | None = None, workers_quantity: int | None = None, instance_role: [InstanceRole](#bodosdk.models.instance_role.InstanceRole) | None = None, instance_type: str | None = None, bodo_version: str | None = None, auto_az: bool | None = None, availability_zone: str | None = None, custom_tags: Dict | None = None)
 
 Updates the cluster’s configuration with the provided values.
 
-- **Parameters:**
-  - **auto_stop** – Optional; configures auto-stop feature.
-  - **auto_pause** – Optional; configures auto-pause feature.
-  - **description** – Optional; updates the cluster’s description.
-  - **name** – Optional; updates the cluster’s name.
-  - **workers_quantity** – Optional; updates the number of workers.
-  - **instance_role** – Optional; updates the instance role.
-  - **instance_type** – Optional; updates the instance type.
-  - **bodo_version** – Optional; updates the Bodo version.
-  - **auto_az** – Optional; enables/disables automatic availability zone selection.
-  - **availability_zone** – Optional; sets a specific availability zone.
-- **Returns:**
+* **Parameters:**
+  * **auto_stop** – Optional; configures auto-stop feature.
+  * **auto_pause** – Optional; configures auto-pause feature.
+  * **description** – Optional; updates the cluster’s description.
+  * **name** – Optional; updates the cluster’s name.
+  * **workers_quantity** – Optional; updates the number of workers.
+  * **instance_role** – Optional; updates the instance role.
+  * **instance_type** – Optional; updates the instance type.
+  * **bodo_version** – Optional; updates the Bodo version.
+  * **auto_az** – Optional; enables/disables automatic availability zone selection.
+  * **availability_zone** – Optional; sets a specific availability zone.
+* **Returns:**
   The updated Cluster instance.
 
-#### updated*at *: datetime | None\_
+#### updated_at *: datetime | None*
 
-#### use*spot_instance *: bool | None\_
+#### use_spot_instance *: bool | None*
 
-#### uuid _: str | None_
+#### uuid *: str | None*
 
 #### wait_for_status(statuses: List[str], timeout: int = 600, tick: int = 30)
 
 Waits for the cluster to reach one of the specified states within a given timeout.
 
-- **Parameters:**
-  - **statuses** – A list of states to wait for.
-  - **timeout** – The maximum time to wait before raising a TimeoutException.
-  - **tick** – The interval between checks.
-- **Returns:**
+* **Parameters:**
+  * **statuses** – A list of states to wait for.
+  * **timeout** – The maximum time to wait before raising a TimeoutException.
+  * **tick** – The interval between checks.
+* **Returns:**
   The Cluster instance, once it has reached one of the desired states.
-- **Raises:**
+* **Raises:**
   **TimeoutException** – If the cluster does not reach a desired state within the timeout.
 
-#### workers*quantity *: int | None\_
+#### workers_quantity *: int | None*
 
-#### workspace _: dict | None_
+#### workspace *: dict | None*
 
-### _class_ bodosdk.models.cluster.ClusterFilter(\*, uuids: List[str] | None = None, clusterNames: List[str] | None = None, statues: List[str] | None = None, tags: Dict | None = None)
+### *class* bodosdk.models.cluster.ClusterFilter(\*, uuids: List[str] | None = None, clusterNames: List[str] | None = None, statues: List[str] | None = None, tags: Dict | None = None)
 
 Bases: `SDKBaseModel`, `IClusterFilter`
 
 Represents a filter used to select clusters based on specific criteria.
 
 This class is used to construct filter criteria for querying clusters by their identifiers,
 names, statuses, or tags. It inherits from SDKBaseModel and implements the IClusterFilter interface.
 
 #### ids
 
 Optional list of cluster UUIDs. Default is an empty list.
 
-- **Type:**
+* **Type:**
   Optional[List[str]]
 
 #### cluster_names
 
 Optional list of cluster names to filter by. Default is an empty list.
 
-- **Type:**
+* **Type:**
   Optional[List[str]]
 
 #### statuses
 
 Optional list of cluster statuses to filter by. Default is an empty list.
 
-- **Type:**
+* **Type:**
   Optional[List[str]]
 
 #### tags
 
 Optional dictionary of tags for more fine-grained filtering.
 
-- **Type:**
+* **Type:**
   Optional[Dict]
 
 ### Default is an empty dictionary.
 
 Each attribute supports being set via their field name or by the specified alias in the Field definition.
 
-#### _class_ Config
+#### *class* Config
 
 Bases: `object`
 
 Configuration for Pydantic models.
 [https://docs.pydantic.dev/latest/api/config/](https://docs.pydantic.dev/latest/api/config/)
 
-#### allow*population_by_field_name *= True\_
+#### allow_population_by_field_name *= True*
 
-#### extra _= 'forbid'_
+#### extra *= 'forbid'*
 
-#### cluster*names *: List[str] | None\_
+#### cluster_names *: List[str] | None*
 
-#### ids _: List[str] | None_
+#### ids *: List[str] | None*
 
-#### statuses _: List[str] | None_
+#### statuses *: List[str] | None*
 
-#### tags _: Dict | None_
+#### tags *: Dict | None*
 
-### _class_ bodosdk.models.cluster.ClusterList(workspace_client: IBodoWorkspaceClient = None, \*, page: int | None = 0, pageSize: int | None = 10, total: int | None = None, order: Dict | None = None, filters: [ClusterFilter](#bodosdk.models.cluster.ClusterFilter) | dict | None = None)
+### *class* bodosdk.models.cluster.ClusterList(workspace_client: IBodoWorkspaceClient = None, \*, page: int | None = 0, pageSize: int | None = 10, total: int | None = None, order: Dict | None = None, filters: [ClusterFilter](#bodosdk.models.cluster.ClusterFilter) | dict | None = None)
 
 Bases: `IClusterList`, `SDKBaseModel`
 
 A model representing a list of clusters, providing pagination, filtering, and
 operations on clusters such as start, stop, delete, resume, and pause.
 
 #### page
 
 The current page number for pagination, starting from 0.
 
-- **Type:**
+* **Type:**
   Optional[int]
 
 #### page_size
 
 The number of items to be displayed per page.
 
-- **Type:**
+* **Type:**
   Optional[int]
 
 #### total
 
 The total number of items available across all pages.
 
-- **Type:**
+* **Type:**
   Optional[int]
 
 #### order
 
 Ordering information for listing clusters. Defaults to an empty dict.
 
-- **Type:**
+* **Type:**
   Optional[Dict]
 
 #### filters
 
 Filtering criteria to apply when fetching the cluster list.
 
-- **Type:**
+* **Type:**
   Optional[[ClusterFilter](#bodosdk.models.cluster.ClusterFilter)]
 
 #### \_clusters
 
 Internal list of cluster objects.
 
-- **Type:**
+* **Type:**
   List[ICluster]
 
 #### \_index
 
 Internal index to track the current position when iterating through clusters.
 
-- **Type:**
+* **Type:**
   int
 
-#### _class_ Config
+#### *class* Config
 
 Bases: `object`
 
 Configuration for Pydantic models.
 [https://docs.pydantic.dev/latest/api/config/](https://docs.pydantic.dev/latest/api/config/)
 
-#### allow*population_by_field_name *= True\_
+#### allow_population_by_field_name *= True*
 
-#### extra _= 'forbid'_
+#### extra *= 'forbid'*
 
 #### cancel_jobs()
 
 Cancels all jobs associated with the clusters.
 
-- **Returns:**
+* **Returns:**
   The ClusterList instance.
 
 #### delete(wait=False)
 
 Deletes each cluster in the list, updating the internal list with the result
 of each delete operation. This method effectively attempts to delete all clusters
 and returns the updated list.
 
-- **Returns:**
+* **Returns:**
   The current instance of ClusterList after attempting to delete
   : all clusters.
-- **Return type:**
+* **Return type:**
   [ClusterList](#bodosdk.models.cluster.ClusterList)
 
-#### filters _: [ClusterFilter](#bodosdk.models.cluster.ClusterFilter) | dict | None_
+#### filters *: [ClusterFilter](#bodosdk.models.cluster.ClusterFilter) | dict | None*
 
-#### order _: Dict | None_
+#### order *: Dict | None*
 
-#### page _: int | None_
+#### page *: int | None*
 
-#### page*size *: int | None\_
+#### page_size *: int | None*
 
 #### pause(wait=False)
 
 Attempts to pause each running cluster in the list. It handles exceptions gracefully,
 updating the list with the status of each cluster following the operation.
 
-- **Returns:**
+* **Returns:**
   The current instance of ClusterList after attempting to pause
   : all clusters.
-- **Return type:**
+* **Return type:**
   [ClusterList](#bodosdk.models.cluster.ClusterList)
 
 #### refresh()
 
 Refreshes the list of clusters by resetting the pagination and filter settings,
 then reloading the first page of clusters. This method effectively resets the
 ClusterList instance to its initial state, based on current filters and ordering.
 
-- **Returns:**
+* **Returns:**
   The current instance of ClusterList after reloading the first page
   : of clusters.
-- **Return type:**
+* **Return type:**
   [ClusterList](#bodosdk.models.cluster.ClusterList)
 
 #### resume(wait=False)
 
 Attempts to resume each paused or stopped cluster in the list. It handles exceptions
 gracefully, ensuring the list is updated with the status of each cluster after
 the operation.
 
-- **Returns:**
+* **Returns:**
   The current instance of ClusterList after attempting to resume
   : all clusters.
-- **Return type:**
+* **Return type:**
   [ClusterList](#bodosdk.models.cluster.ClusterList)
 
 #### run_job(template_id: str = None, code_type: str = None, source: dict | IS3Source | IGitRepoSource | IWorkspaceSource | ITextSource = None, exec_file: str = None, args: dict | str = None, env_vars: dict = None, timeout: int = None, num_retries: int = None, delay_between_retries: int = None, retry_on_timeout: bool = None, name: str = None, catalog: str = None)
 
 Executes a job across all clusters managed by the instance.
 
 This method supports multiple source types and configurations for executing jobs,
 including retries and custom environment variables.
 
-- **Parameters:**
-  - **template_id** (_str_ _,_ _optional_) – Identifier for the job template to be used.
-  - **code_type** (_str_ _,_ _optional_) – The type of code to execute (e.g., Python, Java).
-  - **source** (_Union_ _[\*\*dict_ _,_ _IS3Source_ _,_ _IGitRepoSource_ _,_ _IWorkspaceSource_ _,_ _ITextSource_ _]_ _,_ _optional_) –
-  - **retrieved.** (_The source from where the job's code will be_) –
-  - **exec_file** (_str_ _,_ _optional_) – Path to the main executable file within the source.
-  - **args** (_Union_ _[\*\*dict_ _,_ _str_ _]_ _,_ _optional_) – Arguments to pass to the job. Can be a dictionary or a
-  - **job.** (_string formatted as required by the_) –
-  - **env_vars** (_dict_ _,_ _optional_) – Environment variables to set for the job execution.
-  - **timeout** (_int_ _,_ _optional_) – Maximum time in seconds for the job to run before it is terminated.
-  - **num_retries** (_int_ _,_ _optional_) – Number of times to retry the job on failure.
-  - **delay_between_retries** (_int_ _,_ _optional_) – Time in seconds to wait between retries.
-  - **retry_on_timeout** (_bool_ _,_ _optional_) – Whether to retry the job if it times out.
-  - **name** (_str_ _,_ _optional_) – A name for the job run.
-  - **catalog** (_str_ _,_ _optional_) – Catalog identifier to specify a data catalog for the job.
-- **Returns:**
+* **Parameters:**
+  * **template_id** (*str* *,* *optional*) – Identifier for the job template to be used.
+  * **code_type** (*str* *,* *optional*) – The type of code to execute (e.g., Python, Java).
+  * **source** (*Union* *[**dict* *,* *IS3Source* *,* *IGitRepoSource* *,* *IWorkspaceSource* *,* *ITextSource* *]* *,* *optional*) –
+  * **retrieved.** (*The source from where the job's code will be*) –
+  * **exec_file** (*str* *,* *optional*) – Path to the main executable file within the source.
+  * **args** (*Union* *[**dict* *,* *str* *]* *,* *optional*) – Arguments to pass to the job. Can be a dictionary or a
+  * **job.** (*string formatted as required by the*) –
+  * **env_vars** (*dict* *,* *optional*) – Environment variables to set for the job execution.
+  * **timeout** (*int* *,* *optional*) – Maximum time in seconds for the job to run before it is terminated.
+  * **num_retries** (*int* *,* *optional*) – Number of times to retry the job on failure.
+  * **delay_between_retries** (*int* *,* *optional*) – Time in seconds to wait between retries.
+  * **retry_on_timeout** (*bool* *,* *optional*) – Whether to retry the job if it times out.
+  * **name** (*str* *,* *optional*) – A name for the job run.
+  * **catalog** (*str* *,* *optional*) – Catalog identifier to specify a data catalog for the job.
+* **Returns:**
   An object listing the UUIDs of jobs that were successfully initiated.
-- **Return type:**
+* **Return type:**
   IJobRunList
 
 Decorators:
 : @check_deprecation: Checks if the method or its parameters are deprecated.
 
 #### run_sql_query(template_id: str = None, catalog: str = None, sql_query: str = None, name: str = None, args: dict = None, timeout: int = None, num_retries: int = None, delay_between_retries: int = None, retry_on_timeout: bool = None)
 
 Executes an SQL job across all clusters managed by the instance.
 
 This method submits an SQL query for execution, allowing for additional configurations such as retries
 and setting execution timeouts.
 
-- **Parameters:**
-  - **template_id** (_str_ _,_ _optional_) – Identifier for the job template to be used.
-  - **catalog** (_str_ _,_ _optional_) – Catalog identifier to specify a data catalog for the SQL job.
-  - **sql_query** (_str_ _,_ _optional_) – The SQL query to execute.
-  - **name** (_str_ _,_ _optional_) – A name for the job run.
-  - **args** (_dict_ _,_ _optional_) – Additional arguments specific to the SQL job.
-  - **timeout** (_int_ _,_ _optional_) – Maximum time in seconds for the job to run before it is terminated.
-  - **num_retries** (_int_ _,_ _optional_) – Number of times to retry the job on failure.
-  - **delay_between_retries** (_int_ _,_ _optional_) – Time in seconds to wait between retries.
-  - **retry_on_timeout** (_bool_ _,_ _optional_) – Whether to retry the job if it times out.
-- **Returns:**
+* **Parameters:**
+  * **template_id** (*str* *,* *optional*) – Identifier for the job template to be used.
+  * **catalog** (*str* *,* *optional*) – Catalog identifier to specify a data catalog for the SQL job.
+  * **sql_query** (*str* *,* *optional*) – The SQL query to execute.
+  * **name** (*str* *,* *optional*) – A name for the job run.
+  * **args** (*dict* *,* *optional*) – Additional arguments specific to the SQL job.
+  * **timeout** (*int* *,* *optional*) – Maximum time in seconds for the job to run before it is terminated.
+  * **num_retries** (*int* *,* *optional*) – Number of times to retry the job on failure.
+  * **delay_between_retries** (*int* *,* *optional*) – Time in seconds to wait between retries.
+  * **retry_on_timeout** (*bool* *,* *optional*) – Whether to retry the job if it times out.
+* **Returns:**
   An object listing the UUIDs of SQL jobs that were successfully initiated.
-- **Return type:**
+* **Return type:**
   IJobRunList
 
 Decorators:
 : @check_deprecation: Checks if the method or its parameters are deprecated.
 
 #### start(wait=False)
 
 Attempts to start each stopped or paused cluster in the list. It handles exceptions
 gracefully, ensuring the list reflects the status of each cluster after the operation.
 
-- **Returns:**
+* **Returns:**
   The current instance of ClusterList after attempting to start
   : all clusters.
-- **Return type:**
+* **Return type:**
   [ClusterList](#bodosdk.models.cluster.ClusterList)
 
 #### stop(wait=False)
 
 Attempts to stop each running or starting cluster in the list. It handles exceptions
 gracefully, updating the list with the status of each cluster after the operation.
 
-- **Returns:**
+* **Returns:**
   The current instance of ClusterList after attempting to stop
   : all clusters.
-- **Return type:**
+* **Return type:**
   [ClusterList](#bodosdk.models.cluster.ClusterList)
 
-#### total _: int | None_
+#### total *: int | None*
 
 #### wait_for_status(statuses: List[str] = None, timeout: int = 600, tick: int = 60)
 
 Waits for each cluster in the list to reach one of the specified statuses, updating
 the list with the results. This method polls each cluster’s status until it matches
 one of the desired statuses or until the timeout is reached.
 
-- **Parameters:**
-  - **statuses** (_List_ _[\*\*str_ _]_ _,_ _optional_) – A list of status strings to wait for.
-  - **timeout** (_int_ _,_ _optional_) – The maximum time to wait for each cluster to reach the
+* **Parameters:**
+  * **statuses** (*List* *[**str* *]* *,* *optional*) – A list of status strings to wait for.
+  * **timeout** (*int* *,* *optional*) – The maximum time to wait for each cluster to reach the
     desired status, in seconds.
-  - **tick** (_int_ _,_ _optional_) – The interval between status checks, in seconds.
-- **Returns:**
+  * **tick** (*int* *,* *optional*) – The interval between status checks, in seconds.
+* **Returns:**
   The current instance of ClusterList after waiting for all clusters
   : to reach one of the specified statuses.
-- **Return type:**
+* **Return type:**
   [ClusterList](#bodosdk.models.cluster.ClusterList)
 
-### _class_ bodosdk.models.cluster.InstanceType(\*, name: str, vcpus: int, cores: int, memory: int, efa: bool | None = None, acceleratedNetworking: bool | None = None)
+### *class* bodosdk.models.cluster.InstanceType(\*, name: str, vcpus: int, cores: int, memory: int, efa: bool | None = None, acceleratedNetworking: bool | None = None)
 
 Bases: `SDKBaseModel`, `IInstanceType`
 
 Represents the specifications for a type of computing instance.
 
 This class defines a specific configuration of a computing instance,
 including its processing power and memory capabilities, as well as optional features related to networking.
 
 #### name
 
 The name or identifier of the instance type.
 
-- **Type:**
+* **Type:**
   str
 
 #### vcpus
 
 The number of virtual CPUs available in this instance type.
 
-- **Type:**
+* **Type:**
   int
 
 #### cores
 
 The number of physical cores available in this instance type.
 
-- **Type:**
+* **Type:**
   int
 
 #### memory
 
 The amount of RAM (in megabytes) available in this instance type.
 
-- **Type:**
+* **Type:**
   int
 
 #### efa
 
 Indicates whether Elastic Fabric Adapter (EFA) is supported. Defaults to None.
 
-- **Type:**
+* **Type:**
   Optional[bool]
 
 #### accelerated_networking
 
 Specifies if accelerated networking is enabled.
 
-- **Type:**
+* **Type:**
   Optional[bool]
 
 ### This is mapped to the JSON key 'acceleratedNetworking'. Defaults to None.
 
-#### accelerated*networking *: bool | None\_
+#### accelerated_networking *: bool | None*
 
-#### cores _: int_
+#### cores *: int*
 
-#### efa _: bool | None_
+#### efa *: bool | None*
 
-#### memory _: int_
+#### memory *: int*
 
-#### name _: str_
+#### name *: str*
 
-#### vcpus _: int_
+#### vcpus *: int*
 
-### _class_ bodosdk.models.cluster.NodeMetadata(\*, privateIP: str | None = None, instanceId: str | None = None)
+### *class* bodosdk.models.cluster.NodeMetadata(\*, privateIP: str | None = None, instanceId: str | None = None)
 
 Bases: `SDKBaseModel`
 
-#### instance*id *: str | None\_
+#### instance_id *: str | None*
 
-#### private*ip *: str | None\_
+#### private_ip *: str | None*
 
 <a id="module-bodosdk.db.connection"></a>
 
-### _class_ bodosdk.db.connection.Connection(catalog: str, cluster: ICluster, timeout=3600)
+### *class* bodosdk.db.connection.Connection(catalog: str, cluster: ICluster, timeout=3600)
 
 Bases: `object`
 
 #### cursor()
 
-### _class_ bodosdk.db.connection.Cursor(catalog: str, cluster: ICluster, timeout: int)
+### *class* bodosdk.db.connection.Cursor(catalog: str, cluster: ICluster, timeout: int)
 
 Bases: `object`
 
 #### execute(query: str, \*\*kwargs)
 
 #### execute_async(query: str, \*\*kwargs)
 
 #### fetchall()
 
 #### fetchmany(size)
 
 #### fetchone()
 
-### _exception_ bodosdk.db.connection.QueryError
+### *exception* bodosdk.db.connection.QueryError
 
 Bases: `Exception`
 
 <a id="module-bodosdk.models.job"></a>
 
-### _class_ bodosdk.models.job.GitRepoSource(\*, type: str = 'GIT', repoUrl: str, reference: str | None = '', username: str, token: str)
+### *class* bodosdk.models.job.GitRepoSource(\*, type: str = 'GIT', repoUrl: str, reference: str | None = '', username: str, token: str)
 
 Bases: `SDKBaseModel`
 
 Git repository source definition.
 
 …
 
 #### repo_url
 
 Git repository URL.
 
-- **Type:**
+* **Type:**
   str
 
 #### reference
 
 Git reference (branch, tag, commit hash). (Default: “”)
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### username
 
 Git username.
 
-- **Type:**
+* **Type:**
   str
 
 #### token
 
 Git token.
 
-- **Type:**
+* **Type:**
   str
 
-#### reference _: str | None_
+#### reference *: str | None*
 
-#### repo*url *: str\_
+#### repo_url *: str*
 
-#### token _: str_
+#### token *: str*
 
-#### type _: str_
+#### type *: str*
 
-#### username _: str_
+#### username *: str*
 
-### _class_ bodosdk.models.job.JobConfig(\*, type: str | None = None, source: [GitRepoSource](#bodosdk.models.job.GitRepoSource) | [WorkspaceSource](#bodosdk.models.job.WorkspaceSource) | [S3Source](#bodosdk.models.job.S3Source) | [TextSource](#bodosdk.models.job.TextSource) | None = None, sourceLocation: str | None = None, sqlQueryText: str | None = None, sqlQueryParameters: dict | None = None, args: dict | str | None = None, retryStrategy: [RetryStrategy](#bodosdk.models.job.RetryStrategy) | None = None, timeout: int | None = None, envVars: dict | None = None, catalog: str | None = None)
+### *class* bodosdk.models.job.JobConfig(\*, type: str | None = None, source: [GitRepoSource](#bodosdk.models.job.GitRepoSource) | [WorkspaceSource](#bodosdk.models.job.WorkspaceSource) | [S3Source](#bodosdk.models.job.S3Source) | [TextSource](#bodosdk.models.job.TextSource) | None = None, sourceLocation: str | None = None, sqlQueryText: str | None = None, sqlQueryParameters: dict | None = None, args: dict | str | None = None, retryStrategy: [RetryStrategy](#bodosdk.models.job.RetryStrategy) | None = None, timeout: int | None = None, envVars: dict | None = None, catalog: str | None = None)
 
 Bases: `SDKBaseModel`, `IJobConfig`
 
 Configures details for executing a job, including the execution source, file location, and execution parameters.
 
 #### type
 
 The type of job: PYTHON, SQL, IPYNB
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### source
 
-- **Type:**
+* **Type:**
   Optional[Union[[GitRepoSource](#bodosdk.models.job.GitRepoSource), [WorkspaceSource](#bodosdk.models.job.WorkspaceSource), [S3Source](#bodosdk.models.job.S3Source), [TextSource](#bodosdk.models.job.TextSource)]]
 
 ### The source from which the job is configured or executed.
 
 #### exec_file
 
 The location of the file to execute.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### exec_text
 
 The text containing script/code/sql to execute, valid for TextSource
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### sql_query_parameters
 
 Parameters to substitute within an SQL query.
 
-- **Type:**
+* **Type:**
   Optional[dict]
 
 #### args
 
 Additional arguments required for job execution.
 
-- **Type:**
+* **Type:**
   Optional[Union[dict, str]]
 
 ### Can be a dictionary or string.
 
 #### retry_strategy
 
-- **Type:**
+* **Type:**
   Optional[[RetryStrategy](#bodosdk.models.job.RetryStrategy)]
 
 ### Configuration for the job retry strategy.
 
 #### timeout
 
 The maximum time (in seconds) allowed for the job to run before it times out.
 
-- **Type:**
+* **Type:**
   Optional[int]
 
 #### env_vars
 
 Environment variables to be set for the job run.
 
-- **Type:**
+* **Type:**
   Optional[dict]
 
 #### catalog
 
 The catalog associated with the job, if applicable.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
-#### args _: dict | str | None_
+#### args *: dict | str | None*
 
-#### catalog _: str | None_
+#### catalog *: str | None*
 
-#### env*vars *: dict | None\_
+#### env_vars *: dict | None*
 
-#### exec*file *: str | None\_
+#### exec_file *: str | None*
 
-#### exec*text *: str | None\_
+#### exec_text *: str | None*
 
-#### retry*strategy *: [RetryStrategy](#bodosdk.models.job.RetryStrategy) | None\_
+#### retry_strategy *: [RetryStrategy](#bodosdk.models.job.RetryStrategy) | None*
 
-#### source _: [GitRepoSource](#bodosdk.models.job.GitRepoSource) | [WorkspaceSource](#bodosdk.models.job.WorkspaceSource) | [S3Source](#bodosdk.models.job.S3Source) | [TextSource](#bodosdk.models.job.TextSource) | None_
+#### source *: [GitRepoSource](#bodosdk.models.job.GitRepoSource) | [WorkspaceSource](#bodosdk.models.job.WorkspaceSource) | [S3Source](#bodosdk.models.job.S3Source) | [TextSource](#bodosdk.models.job.TextSource) | None*
 
-#### sql*query_parameters *: dict | None\_
+#### sql_query_parameters *: dict | None*
 
-#### timeout _: int | None_
+#### timeout *: int | None*
 
-#### type _: str | None_
+#### type *: str | None*
 
-### _class_ bodosdk.models.job.JobFilter(\*, ids: List[str | UUID] | None = None, template_ids: List[str | UUID] | None = None, cluster_ids: List[str | UUID] | None = None, types: List[str] | None = None, statuses: List[str] | None = None, started_at: datetime | None = None, finished_at: datetime | None = None)
+### *class* bodosdk.models.job.JobFilter(\*, ids: List[str | UUID] | None = None, template_ids: List[str | UUID] | None = None, cluster_ids: List[str | UUID] | None = None, types: List[str] | None = None, statuses: List[str] | None = None, started_at: datetime | None = None, finished_at: datetime | None = None)
 
 Bases: `SDKBaseModel`
 
 Provides filtering options for querying job-related data.
 
 #### ids
 
 A list of job IDs to filter by.
 
-- **Type:**
+* **Type:**
   Optional[List[Union[str, UUID]]]
 
 #### template_ids
 
 A list of job template IDs to filter by.
 
-- **Type:**
+* **Type:**
   Optional[List[Union[str, UUID]]]
 
 #### cluster_ids
 
 A list of cluster IDs to filter jobs by.
 
-- **Type:**
+* **Type:**
   Optional[List[Union[str, UUID]]]
 
 #### types
 
 A list of job types to filter by.
 
-- **Type:**
+* **Type:**
   Optional[List[str]]
 
 #### statuses
 
 A list of job statuses to filter by.
 
-- **Type:**
+* **Type:**
   Optional[List[str]]
 
 #### started_at
 
 A datetime value to filter jobs that started after it.
 
-- **Type:**
+* **Type:**
   Optional[datetime]
 
 #### finished_at
 
 A datetime value to filter jobs that finished before it.
 
-- **Type:**
+* **Type:**
   Optional[datetime]
 
-#### cluster*ids *: List[str | UUID] | None\_
+#### cluster_ids *: List[str | UUID] | None*
 
-#### finished*at *: datetime | None\_
+#### finished_at *: datetime | None*
 
-#### ids _: List[str | UUID] | None_
+#### ids *: List[str | UUID] | None*
 
-#### started*at *: datetime | None\_
+#### started_at *: datetime | None*
 
-#### statuses _: List[str] | None_
+#### statuses *: List[str] | None*
 
-#### template*ids *: List[str | UUID] | None\_
+#### template_ids *: List[str | UUID] | None*
 
-#### types _: List[str] | None_
+#### types *: List[str] | None*
 
-### _class_ bodosdk.models.job.JobRun(workspace_client: IBodoWorkspaceClient = None, \*, uuid: str | None = None, name: str | None = None, type: str | None = 'BATCH', submittedAt: datetime | None = None, finishedAt: datetime | None = None, lastHealthCheck: datetime | None = None, lastKnownActivity: datetime | None = None, status: str | None = None, reason: str | None = None, num_retries_used: int | None = (FieldInfo(default=0, alias='numRetriesUsed', alias_priority=2, extra={}),), tag: List | None = None, clusterUUID: str | None = None, cluster: 'Cluster' | None, clusterConfig: 'Cluster' | None = None, config: [JobConfig](#bodosdk.models.job.JobConfig) | None = None, jobTemplateUUID: str | None = None, submitter: str | None = None, stats: dict | None = None)
+### *class* bodosdk.models.job.JobRun(workspace_client: IBodoWorkspaceClient = None, \*, uuid: str | None = None, name: str | None = None, type: str | None = 'BATCH', submittedAt: datetime | None = None, finishedAt: datetime | None = None, lastHealthCheck: datetime | None = None, lastKnownActivity: datetime | None = None, status: str | None = None, reason: str | None = None, num_retries_used: int | None = (FieldInfo(default=0, alias='numRetriesUsed', alias_priority=2, extra={}),), tag: List | None = None, clusterUUID: str | None = None, cluster: 'Cluster' | None, clusterConfig: 'Cluster' | None = None, config: [JobConfig](#bodosdk.models.job.JobConfig) | None = None, jobTemplateUUID: str | None = None, submitter: str | None = None, stats: dict | None = None)
 
 Bases: `SDKBaseModel`, `IJobRun`
 
 Details a specific instance of a job run, including status and configuration details.
 
 #### uuid
 
 Unique identifier for the job run.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### name
 
 Name of the job run.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### type
 
 Type of job run, defaults to ‘BATCH’ if not specified.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### submitted_at
 
 Timestamp when the job was submitted.
 
-- **Type:**
+* **Type:**
   Optional[datetime]
 
 #### finished_at
 
 Timestamp when the job finished running.
 
-- **Type:**
+* **Type:**
   Optional[datetime]
 
 #### last_health_check
 
 Timestamp of the last health check performed.
 
-- **Type:**
+* **Type:**
   Optional[datetime]
 
 #### last_known_activity
 
 Timestamp of the last known activity of this job.
 
-- **Type:**
+* **Type:**
   Optional[datetime]
 
 #### status
 
 Current status of the job run.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### reason
 
 Reason for the job’s current status, particularly if there’s an error or failure.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### num_retries_used
 
 The number of retries that have been used for this job run. Defaults to 0.
 
-- **Type:**
+* **Type:**
   Optional[int]
 
 #### tags
 
 Tags associated with the job run. Default is an empty list.
 
-- **Type:**
+* **Type:**
   Optional[List]
 
 #### cluster_uuid
 
 UUID of the cluster on which the job is running.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### cluster
 
 The cluster object associated with the job run.
 
-- **Type:**
+* **Type:**
   Optional[[Cluster](#bodosdk.models.cluster.Cluster)]
 
 #### cluster_config
 
 Configuration of the cluster used for this job run.
 
-- **Type:**
+* **Type:**
   Optional[[Cluster](#bodosdk.models.cluster.Cluster)]
 
 #### config
 
 Job configuration details used for this run.
 
-- **Type:**
+* **Type:**
   Optional[[JobConfig](#bodosdk.models.job.JobConfig)]
 
 #### job_template_id
 
 UUID of the template from which this job was created.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### submitter
 
 The identifier of the user who submitted the job.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### stats
 
 Statistical data about the job run.
 
-- **Type:**
+* **Type:**
   Optional[dict]
 
 #### cancel()
 
 Cancels the job associated with this instance and updates its state based on the response from the job API.
 
 This method sends a cancellation request for the job identified by its UUID to the job API,
 handles the response to update the job’s attributes, and resets its modified state.
 
-- **Returns:**
+* **Returns:**
   The job instance, updated with the latest state after the cancellation attempt.
-- **Return type:**
+* **Return type:**
   [JobRun](#bodosdk.models.job.JobRun)
-- **Raises:**
+* **Raises:**
   **APIException** – If the cancellation request fails or returns an error response.
 
 Decorators:
 : @check_deprecation: Checks if the method or its parameters are deprecated.
 
-#### cluster _: 'Cluster' | None_
+#### cluster *: 'Cluster' | None*
 
-#### cluster*config *: 'Cluster' | None\_
+#### cluster_config *: 'Cluster' | None*
 
-#### cluster*id *: str | None\_
+#### cluster_id *: str | None*
 
-#### config _: [JobConfig](#bodosdk.models.job.JobConfig) | None_
+#### config *: [JobConfig](#bodosdk.models.job.JobConfig) | None*
 
-#### finished*at *: datetime | None\_
+#### finished_at *: datetime | None*
 
 #### get_logs_urls()
 
 #### get_stderr()
 
 #### get_stdout()
 
-#### _property_ id _: str_
+#### *property* id *: str*
 
-#### job*template_id *: str | None\_
+#### job_template_id *: str | None*
 
-#### last*health_check *: datetime | None\_
+#### last_health_check *: datetime | None*
 
-#### last*known_activity *: datetime | None\_
+#### last_known_activity *: datetime | None*
 
-#### name _: str | None_
+#### name *: str | None*
 
-#### num*retries_used *: int | None\_
+#### num_retries_used *: int | None*
 
-#### reason _: str | None_
+#### reason *: str | None*
 
-#### stats _: dict | None_
+#### stats *: dict | None*
 
-#### status _: str | None_
+#### status *: str | None*
 
-#### submitted*at *: datetime | None\_
+#### submitted_at *: datetime | None*
 
-#### submitter _: str | None_
+#### submitter *: str | None*
 
-#### tags _: List | None_
+#### tags *: List | None*
 
-#### type _: str | None_
+#### type *: str | None*
 
-#### uuid _: str | None_
+#### uuid *: str | None*
 
 #### wait_for_status(statuses: List[str], timeout: int = 3600, tick: int = 30)
 
 Waits for the job to reach one of the specified statuses, polling at regular intervals.
 
 This method checks the current status of the job at regular intervals defined by the tick parameter.
 If the job reaches one of the specified statuses before the timeout, it returns the job instance.
 If the timeout is exceeded, it raises a TimeoutException.
 
-- **Parameters:**
-  - **statuses** (_list_ _or_ _tuple_) – A list or tuple of statuses that the job is expected to reach.
-  - **timeout** (_int_ _,_ _optional_) – The maximum time in seconds to wait for the job to reach one of
-  - **seconds.** (_the specified statuses. Defaults to 600_) –
-  - **tick** (_int_ _,_ _optional_) – The time interval in seconds between status checks. Defaults to 30 seconds.
-- **Returns:**
+* **Parameters:**
+  * **statuses** (*list* *or* *tuple*) – A list or tuple of statuses that the job is expected to reach.
+  * **timeout** (*int* *,* *optional*) – The maximum time in seconds to wait for the job to reach one of
+  * **seconds.** (*the specified statuses. Defaults to 600*) –
+  * **tick** (*int* *,* *optional*) – The time interval in seconds between status checks. Defaults to 30 seconds.
+* **Returns:**
   The job instance if one of the specified statuses is reached within the timeout period.
-- **Return type:**
+* **Return type:**
   [JobRun](#bodosdk.models.job.JobRun)
-- **Raises:**
-  - **TimeoutException** – If the job does not reach one of the specified statuses within
-  - **the specified timeout period.** –
+* **Raises:**
+  * **TimeoutException** – If the job does not reach one of the specified statuses within
+  * **the specified timeout period.** –
 
 Decorators:
 : @check_deprecation: Checks if the method or its parameters are deprecated.
 
-### _class_ bodosdk.models.job.JobRunList(workspace_client: IBodoWorkspaceClient = None, \*, page: int | None = 0, pageSize: int | None = 10, total: int | None = None, order: Dict | None = None, filters: [JobFilter](#bodosdk.models.job.JobFilter) | None = None)
+### *class* bodosdk.models.job.JobRunList(workspace_client: IBodoWorkspaceClient = None, \*, page: int | None = 0, pageSize: int | None = 10, total: int | None = None, order: Dict | None = None, filters: [JobFilter](#bodosdk.models.job.JobFilter) | None = None)
 
 Bases: `IJobRunList`, `SDKBaseModel`
 
 Represents a paginated list of job runs, including metadata and filtering capabilities.
 
 #### page
 
 The current page number in the paginated list. Defaults to 0.
 
-- **Type:**
+* **Type:**
   Optional[int]
 
 #### page_size
 
 The number of job runs to display per page. Defaults to 10.
 
-- **Type:**
+* **Type:**
   Optional[int]
 
 #### total
 
 The total number of job runs available.
 
-- **Type:**
+* **Type:**
   Optional[int]
 
 #### order
 
 A dictionary specifying the order in which job runs are sorted.
 
-- **Type:**
+* **Type:**
   Optional[Dict]
 
 #### filters
 
 A JobFilter object used to apply filtering on the list of job runs.
 
-- **Type:**
+* **Type:**
   Optional[[JobFilter](#bodosdk.models.job.JobFilter)]
 
 #### cancel()
 
 Cancels all jobs in the list.
 
 This method iterates through each job in the current list (represented by instances of this class),
 and calls the cancel method on each job to attempt their cancellation.
 After attempting to cancel all jobs, it returns the updated list of jobs.
 
-- **Returns:**
+* **Returns:**
   The list instance, potentially with updated states of the individual jobs
   if the cancellation requests were successful.
-- **Return type:**
+* **Return type:**
   [JobRunList](#bodosdk.models.job.JobRunList)
 
 #### NOTE
-
 This method relies on the individual cancel() method of the job objects within the list.
 If any job cancellation fails, it could raise an exception depending on
 the implementation of the individual cancel() method.
 
-#### _property_ clusters
+#### *property* clusters
 
-#### filters _: [JobFilter](#bodosdk.models.job.JobFilter) | None_
+#### filters *: [JobFilter](#bodosdk.models.job.JobFilter) | None*
 
-#### order _: Dict | None_
+#### order *: Dict | None*
 
-#### page _: int | None_
+#### page *: int | None*
 
-#### page*size *: int | None\_
+#### page_size *: int | None*
 
 #### refresh()
 
 Refreshes the list of jobs by clearing the current elements and reloading the next page of job data.
 
 This method resets the internal state of the list, including the pagination index and the elements themselves.
 It then loads the next page of data from the underlying data source to repopulate the list.
 The list is temporarily set to mutable during this process to allow updates, and then set back to immutable
 once the refresh is complete.
 
-- **Returns:**
+* **Returns:**
   The refreshed job run list instance, with elements reloaded from the next available page.
-- **Return type:**
+* **Return type:**
   [JobRunList](#bodosdk.models.job.JobRunList)
 
 #### NOTE
-
 This method assumes that the list supports pagination and that the underlying data source provides
 the mechanism to load additional pages of data.
 
-#### total _: int | None_
+#### total *: int | None*
 
 #### wait_for_status(statuses: List[str], timeout: int = 3600, tick: int = 30)
 
 Waits for each job in the list to reach one of the specified statuses, polling each at regular intervals.
 
 This method iterates over each job within the list, checking at intervals (defined by tick) to see
 if the job has reached one of the desired statuses specified in statuses.
 If a job reaches the desired status within the timeout period, the method continues to the next job.
 If the timeout is reached without the job reaching the desired status, a TimeoutException is raised.
 
-- **Parameters:**
-  - **statuses** (_list_ _or_ _tuple_) – A list or tuple of statuses that each job is expected to reach.
-  - **timeout** (_int_ _,_ _optional_) – The maximum time in seconds to wait for each job to reach one of
-  - **seconds.** (_Defaults to 30_) –
-  - **tick** (_int_ _,_ _optional_) – The time interval in seconds between status checks for each job.
-  - **seconds.** –
-- **Returns:**
+* **Parameters:**
+  * **statuses** (*list* *or* *tuple*) – A list or tuple of statuses that each job is expected to reach.
+  * **timeout** (*int* *,* *optional*) – The maximum time in seconds to wait for each job to reach one of
+  * **seconds.** (*Defaults to 30*) –
+  * **tick** (*int* *,* *optional*) – The time interval in seconds between status checks for each job.
+  * **seconds.** –
+* **Returns:**
   The job run list instance, after attempting to wait for all jobs to reach the desired statuses.
-- **Return type:**
+* **Return type:**
   [JobRunList](#bodosdk.models.job.JobRunList)
-- **Raises:**
-  - **TimeoutException** – If any job does not reach one of the specified statuses within the specified
-  - **timeout period\*\***,\*\* **including details** **of** **the job's UUID and its current status.** –
+* **Raises:**
+  * **TimeoutException** – If any job does not reach one of the specified statuses within the specified
+  * **timeout period****,** **including details** **of** **the job's UUID and its current status.** –
 
 Decorators:
 : @check_deprecation: Checks if the method or its parameters are deprecated.
 
 #### NOTE
-
 This method individually tracks the timeout for each job, resetting the start time at the beginning
 of the wait for each job in the list.
 
-### _class_ bodosdk.models.job.JobRunLogsResponse(\*, stderrUrl: str = None, stdoutUrl: str = None, expirationDate: str = None)
+### *class* bodosdk.models.job.JobRunLogsResponse(\*, stderrUrl: str = None, stdoutUrl: str = None, expirationDate: str = None)
 
 Bases: `SDKBaseModel`, `IJobRunLogsResponse`
 
 Represents the response object containing URLs for accessing logs related to a job run.
 
 #### stderr_location_url
 
 The URL to access the standard error logs of the job run.
 
-- **Type:**
+* **Type:**
   str
 
 #### stdout_location_url
 
 The URL to access the standard output logs of the job run.
 
-- **Type:**
+* **Type:**
   str
 
 #### expiration_date
 
 The date when the log URLs will expire and no longer be accessible.
 
-- **Type:**
+* **Type:**
   str
 
-#### expiration*date *: str\_
+#### expiration_date *: str*
 
-#### stderr*location_url *: str\_
+#### stderr_location_url *: str*
 
-#### stdout*location_url *: str\_
+#### stdout_location_url *: str*
 
-### _class_ bodosdk.models.job.JobTemplate(workspace_client: IBodoWorkspaceClient = None, \*, uuid: str | None = None, name: str | None = None, jobRuns: List[[JobRun](#bodosdk.models.job.JobRun)] = None, description: str | None = None, createdBy: str | None = None, config: [JobConfig](#bodosdk.models.job.JobConfig) | None = None, clusterConfig: 'Cluster' | None = None)
+### *class* bodosdk.models.job.JobTemplate(workspace_client: IBodoWorkspaceClient = None, \*, uuid: str | None = None, name: str | None = None, jobRuns: List[[JobRun](#bodosdk.models.job.JobRun)] = None, description: str | None = None, createdBy: str | None = None, config: [JobConfig](#bodosdk.models.job.JobConfig) | None = None, clusterConfig: 'Cluster' | None = None)
 
 Bases: `SDKBaseModel`, `IJobTemplate`
 
 Represents a template for creating and managing jobs within an SDK environment, e
 ncapsulating common job configurations.
 
 #### uuid
 
 The unique identifier for the job template.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### name
 
 The name of the job template.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### job_runs
 
 A list of job runs associated with this template. Default is an empty list
 
-- **Type:**
+* **Type:**
   List[[JobRun](#bodosdk.models.job.JobRun)]
 
 ### if none are specified.
 
 #### description
 
 A brief description of the job template.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### created_by
 
 The identifier of the user who created the job template.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### config
 
 The job configuration specifics for this template.
 
-- **Type:**
+* **Type:**
   Optional[[JobConfig](#bodosdk.models.job.JobConfig)]
 
 #### cluster_config
 
 Configuration details of the cluster on which the jobs will run. D
 
-- **Type:**
+* **Type:**
   Optional[[Cluster](#bodosdk.models.cluster.Cluster)]
 
 ### efault is None.
 
-#### cluster*config *: [Cluster](#bodosdk.models.cluster.Cluster) | None\_
+#### cluster_config *: [Cluster](#bodosdk.models.cluster.Cluster) | None*
 
-#### config _: [JobConfig](#bodosdk.models.job.JobConfig) | None_
+#### config *: [JobConfig](#bodosdk.models.job.JobConfig) | None*
 
-#### created*by *: str | None\_
+#### created_by *: str | None*
 
 #### delete()
 
-#### description _: str | None_
+#### description *: str | None*
 
-#### _property_ id
+#### *property* id
 
-#### job*runs *: List[[JobRun](#bodosdk.models.job.JobRun)]\_
+#### job_runs *: List[[JobRun](#bodosdk.models.job.JobRun)]*
 
-#### name _: str | None_
+#### name *: str | None*
 
 #### run(name: str = None, cluster: dict | ICluster = None, code_type: str = None, source: dict | IS3Source | IGitRepoSource | IWorkspaceSource | ITextSource = None, exec_file: str = None, exec_text: str = None, args: dict | str = None, env_vars: dict = None, timeout: int = None, num_retries: int = None, delay_between_retries: int = None, retry_on_timeout: bool = None, catalog: str = None)
 
-#### uuid _: str | None_
+#### uuid *: str | None*
 
-### _class_ bodosdk.models.job.JobTemplateFilter(\*, ids: List[str] | None = None, names: List[str] | None = None, tags: dict | None = None)
+### *class* bodosdk.models.job.JobTemplateFilter(\*, ids: List[str] | None = None, names: List[str] | None = None, tags: dict | None = None)
 
 Bases: `SDKBaseModel`, `IJobTemplateFilter`
 
 Class representig filters for JobTemplateList
 
 #### ids
 
 returns list matching given ids
 
-- **Type:**
+* **Type:**
   List[str] | None
 
 #### names
 
 returns list matching given names
 
-- **Type:**
+* **Type:**
   List[str] | None
 
 #### tags
 
 returns list matching given tags
 
-- **Type:**
+* **Type:**
   dict | None
 
-#### ids _: List[str] | None_
+#### ids *: List[str] | None*
 
-#### names _: List[str] | None_
+#### names *: List[str] | None*
 
-#### tags _: dict | None_
+#### tags *: dict | None*
 
-### _class_ bodosdk.models.job.JobTemplateList(workspace_client: IBodoWorkspaceClient = None, \*, page: int | None = 0, pageSize: int | None = 10, total: int | None = None, order: Dict | None = None, filters: [JobTemplateFilter](#bodosdk.models.job.JobTemplateFilter) | None = None)
+### *class* bodosdk.models.job.JobTemplateList(workspace_client: IBodoWorkspaceClient = None, \*, page: int | None = 0, pageSize: int | None = 10, total: int | None = None, order: Dict | None = None, filters: [JobTemplateFilter](#bodosdk.models.job.JobTemplateFilter) | None = None)
 
 Bases: `IJobTemplateList`, `SDKBaseModel`
 
 Represents a list of JobTemplates, providing pagination and filtering capabilities.
 
 #### page
 
 The current page number in the list of Job Templates. Defaults to 0.
 
-- **Type:**
+* **Type:**
   Optional[int]
 
 #### page_size
 
 The number of Job Templates to display per page. Defaults to 10.
 
-- **Type:**
+* **Type:**
   Optional[int]
 
 #### total
 
 The total number of Job Templates available.
 
-- **Type:**
+* **Type:**
   Optional[int]
 
 #### order
 
 A dictionary specifying the order in which Job Templates are sorted.
 
-- **Type:**
+* **Type:**
   Optional[Dict]
 
 #### filters
 
 A filter object used to filter the Job Templates listed.
 
-- **Type:**
+* **Type:**
   Optional[[InstanceRoleFilter](#bodosdk.models.instance_role.InstanceRoleFilter)]
 
 #### delete()
 
 Deletes all job definitions in the list.
 
 This method iterates over each job definition contained within the list and calls its individual
 delete method. This action attempts to remove each job definition from the underlying storage
 or management system.
 
 #### NOTE
-
 The behavior and success of the deletion process depend on the implementation of the individual
 delete method of each job definition. This may include handling exceptions and ensuring that each
 job definition is properly removed. If an error occurs during the deletion of any job definition,
 it may raise an exception, which should be handled by the caller or within the individual delete methods.
 
-#### filters _: [JobTemplateFilter](#bodosdk.models.job.JobTemplateFilter) | None_
+#### filters *: [JobTemplateFilter](#bodosdk.models.job.JobTemplateFilter) | None*
 
-#### order _: Dict | None_
+#### order *: Dict | None*
 
-#### page _: int | None_
+#### page *: int | None*
 
-#### page*size *: int | None\_
+#### page_size *: int | None*
 
 #### refresh()
 
 Refreshes the list of job templates by clearing the current elements and reloading the next page of job data.
 
 This method resets the internal state of the list, including the pagination index and the elements themselves.
 It then loads the next page of data from the underlying data source to repopulate the list.
 The list is temporarily set to mutable during this process to allow updates, and then set back to
 immutable once the refresh is complete.
 
-- **Returns:**
+* **Returns:**
   The refreshed job template list instance, with elements reloaded from
   the next available page.
-- **Return type:**
+* **Return type:**
   [JobTemplateList](#bodosdk.models.job.JobTemplateList)
 
 #### NOTE
-
 This method assumes that the list supports pagination and that the underlying data source provides
 the mechanism to load additional pages of data.
 
 #### run(instance_type: str = None, workers_quantity: int = None, bodo_version: str = None)
 
 )
 Executes all job definitions in the list with specified configurations and aggregates their run IDs.
 
 This method iterates over each job definition in the list and invokes the run method on each, passing
 the specified configuration parameters such as instance type, the quantity of workers, and the Bodo version.
 It collects the IDs of the resulting job runs and returns a consolidated list of these job runs.
 
-- **Parameters:**
-  - **instance_type** (_str_ _,_ _optional_) – The type of instance to use for the jobs.
-  - **specifications.** (_This may specify the hardware_) –
-  - **workers_quantity** (_int_ _,_ _optional_) – The number of worker instances to deploy for the jobs.
-  - **bodo_version** (_str_ _,_ _optional_) – The specific version of Bodo to use for executing the jobs.
-- **Returns:**
+* **Parameters:**
+  * **instance_type** (*str* *,* *optional*) – The type of instance to use for the jobs.
+  * **specifications.** (*This may specify the hardware*) –
+  * **workers_quantity** (*int* *,* *optional*) – The number of worker instances to deploy for the jobs.
+  * **bodo_version** (*str* *,* *optional*) – The specific version of Bodo to use for executing the jobs.
+* **Returns:**
   An interface to the list of job runs created by executing the job definitions,
   allowing further operations like monitoring and management.
-- **Return type:**
+* **Return type:**
   IJobRunList
 
 #### NOTE
-
 The run method for each job definition must correctly handle the passed configurations.
 If any job execution fails, the behavior and handling of errors should be considered based
 on the implementation of each job definition’s run method.
 
-#### total _: int | None_
+#### total *: int | None*
 
-### _class_ bodosdk.models.job.RetryStrategy(\*, numRetries: int = 0, delayBetweenRetries: int = 1, retryOnTimeout: bool = False)
+### *class* bodosdk.models.job.RetryStrategy(\*, numRetries: int = 0, delayBetweenRetries: int = 1, retryOnTimeout: bool = False)
 
 Bases: `SDKBaseModel`
 
 A Pydantic model that defines the retry strategy for a job or a task. It specifies how many retries
 should be attempted,
 the delay between retries, and whether to retry on timeout.
 
 #### num_retries
 
 The number of times to retry the job after a failure. Defaults to 0, meaning no
 
-- **Type:**
+* **Type:**
   int
 
 ### retries by default.
 
 #### delay_between_retries
 
 The delay between consecutive retries, expressed in minutes. Defaults to 1 minute.
 
-- **Type:**
+* **Type:**
   int
 
 #### retry_on_timeout
 
 A flag to determine if the job should be retried upon timing out. Defaults to False,
 
-- **Type:**
+* **Type:**
   bool
 
 ### indicating no retry on timeout.
 
 Each field is represented with a default value and an alias that matches the corresponding key in JSON or
 other serialized forms.
 
-#### delay*between_retries *: int\_
+#### delay_between_retries *: int*
 
-#### num*retries *: int\_
+#### num_retries *: int*
 
-#### retry*on_timeout *: bool\_
+#### retry_on_timeout *: bool*
 
-### _class_ bodosdk.models.job.S3Source(\*, type: str = 'S3', bucketPath: str, bucketRegion: str)
+### *class* bodosdk.models.job.S3Source(\*, type: str = 'S3', bucketPath: str, bucketRegion: str)
 
 Bases: `SDKBaseModel`
 
 S3 source definition.
 
 …
 
 #### bucket_path
 
 S3 bucket path.
 
-- **Type:**
+* **Type:**
   str
 
 #### bucket_region
 
 S3 bucket region.
 
-- **Type:**
+* **Type:**
   str
 
-#### bucket*path *: str\_
+#### bucket_path *: str*
 
-#### bucket*region *: str\_
+#### bucket_region *: str*
 
-#### type _: str_
+#### type *: str*
 
-### _class_ bodosdk.models.job.TextSource(\*, type: str = 'SQL')
+### *class* bodosdk.models.job.TextSource(\*, type: str = 'SQL')
 
 Bases: `SDKBaseModel`
 
 Represents a specific type of source where the job configuration can originate from a text source.
 
 #### type
 
 Specifies the type of source
 
-- **Type:**
+* **Type:**
   str
 
-#### type _: str_
+#### type *: str*
 
-### _class_ bodosdk.models.job.WorkspaceSource(\*, type: str = 'WORKSPACE', path: str)
+### *class* bodosdk.models.job.WorkspaceSource(\*, type: str = 'WORKSPACE', path: str)
 
 Bases: `SDKBaseModel`
 
 Workspace source definition.
 
 …
 
 #### path
 
 Workspace path.
 
-- **Type:**
+* **Type:**
   str
 
-#### path _: str_
+#### path *: str*
 
-#### type _: str_
+#### type *: str*
 
 <a id="module-bodosdk.models.common"></a>
 
-### _class_ bodosdk.models.common.AWSNetworkData(\*, region: str | None = None, storageEndpoint: bool | None = None, vpcId: str | None = None, fetchedVpcId: str | None = None, publicSubnetsIds: List[str] | None = None, privateSubnetsIds: List[str] | None = None, policyArns: List[str] | None = None)
+### *class* bodosdk.models.common.AWSNetworkData(\*, region: str | None = None, storageEndpoint: bool | None = None, vpcId: str | None = None, fetchedVpcId: str | None = None, publicSubnetsIds: List[str] | None = None, privateSubnetsIds: List[str] | None = None, policyArns: List[str] | None = None)
 
 Bases: [`NetworkData`](#bodosdk.models.common.NetworkData)
 
 Extends the NetworkData class to include specific properties for AWS networking.
 
 #### vpc_id
 
 The ID of the AWS Virtual Private Cloud (VPC) where workspace should be created.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### fetched_vpc_id
 
 The ID of the fetched AWS VPC - if no vpc_id provided.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### public_subnets_ids
 
 List of IDs for the public subnets within the AWS VPC.
 
-- **Type:**
+* **Type:**
   Optional[List[str]]
 
 #### private_subnets_ids
 
 List of IDs for the private subnets within the AWS VPC.
 
-- **Type:**
+* **Type:**
   Optional[List[str]]
 
 #### policies_arn
 
 List of AWS Resource Names (ARNs) for the policies applied to the network.
 
-- **Type:**
+* **Type:**
   Optional[List[str]]
 
-#### fetched*vpc_id *: str | None\_
+#### fetched_vpc_id *: str | None*
 
-#### policies*arn *: List[str] | None\_
+#### policies_arn *: List[str] | None*
 
-#### private*subnets_ids *: List[str] | None\_
+#### private_subnets_ids *: List[str] | None*
 
-#### public*subnets_ids *: List[str] | None\_
+#### public_subnets_ids *: List[str] | None*
 
-#### vpc*id *: str | None\_
+#### vpc_id *: str | None*
 
-### _class_ bodosdk.models.common.NetworkData(\*, region: str | None = None, storageEndpoint: bool | None = None)
+### *class* bodosdk.models.common.NetworkData(\*, region: str | None = None, storageEndpoint: bool | None = None)
 
 Bases: `SDKBaseModel`
 
 A base model for network-related data within an SDK context.
 
 #### region
 
 The geographic region where the network is located.
 
-- **Type:**
+* **Type:**
   Optional[str]
 
 #### storage_endpoint
 
 Indicates whether a storage endpoint is enabled.
 
-- **Type:**
+* **Type:**
   Optional[bool]
 
-#### region _: str | None_
+#### region *: str | None*
 
-#### storage*endpoint *: bool | None\_
+#### storage_endpoint *: bool | None*
 
 <a id="module-bodosdk.models.instance_role"></a>
 
-### _class_ bodosdk.models.instance_role.InstanceRole(workspace_client: IBodoWorkspaceClient = None, \*, uuid: str | None = None, name: str | None = None, description: str | None = None, roleArn: str | None = None, status: str | None = None)
+### *class* bodosdk.models.instance_role.InstanceRole(workspace_client: IBodoWorkspaceClient = None, \*, uuid: str | None = None, name: str | None = None, description: str | None = None, roleArn: str | None = None, status: str | None = None)
 
 Bases: `SDKBaseModel`, `IInstanceRole`
 
 #### delete()
 
 Removes instance role from workspace
 
-- **Returns:**
+* **Returns:**
   None
 
-#### description _: str | None_
+#### description *: str | None*
 
-#### _property_ id
+#### *property* id
 
-#### name _: str | None_
+#### name *: str | None*
 
-#### role*arn *: str | None\_
+#### role_arn *: str | None*
 
-#### status _: str | None_
+#### status *: str | None*
 
-#### uuid _: str | None_
+#### uuid *: str | None*
 
-### _class_ bodosdk.models.instance_role.InstanceRoleFilter(\*, uuids: List[str] | None = None, names: List[str] | None = None, roleArns: List[str] | None = None)
+### *class* bodosdk.models.instance_role.InstanceRoleFilter(\*, uuids: List[str] | None = None, names: List[str] | None = None, roleArns: List[str] | None = None)
 
 Bases: `SDKBaseModel`, `IInstanceRoleFilter`
 
 Class representing filters for InstanceRoleList
 
 #### ids
 
 returns list matching given ids
 
-- **Type:**
+* **Type:**
   List[str] | None
 
 #### names
 
 returns list matching given names
 
-- **Type:**
+* **Type:**
   List[str] | None
 
 #### role_arns
 
 returns list matching giver arns
 
-- **Type:**
+* **Type:**
   List[str] | None
 
-#### _class_ Config
+#### *class* Config
 
 Bases: `object`
 
 Configuration for Pydantic models.
 [https://docs.pydantic.dev/latest/api/config/](https://docs.pydantic.dev/latest/api/config/)
 
-#### allow*population_by_field_name *= True\_
+#### allow_population_by_field_name *= True*
 
-#### extra _= 'forbid'_
+#### extra *= 'forbid'*
 
-#### ids _: List[str] | None_
+#### ids *: List[str] | None*
 
-#### names _: List[str] | None_
+#### names *: List[str] | None*
 
-#### role*arns *: List[str] | None\_
+#### role_arns *: List[str] | None*
 
-### _class_ bodosdk.models.instance_role.InstanceRoleList(workspace_client: IBodoWorkspaceClient = None, \*, page: int | None = 0, pageSize: int | None = 10, total: int | None = None, order: Dict | None = None, filters: [InstanceRoleFilter](#bodosdk.models.instance_role.InstanceRoleFilter) | None = None)
+### *class* bodosdk.models.instance_role.InstanceRoleList(workspace_client: IBodoWorkspaceClient = None, \*, page: int | None = 0, pageSize: int | None = 10, total: int | None = None, order: Dict | None = None, filters: [InstanceRoleFilter](#bodosdk.models.instance_role.InstanceRoleFilter) | None = None)
 
 Bases: `IInstanceRoleList`, `SDKBaseModel`
 
 Represents a list of instance roles within an SDK context, providing pagination and filtering capabilities.
 
 #### page
 
 The current page number in the list of instance roles. Defaults to 0.
 
-- **Type:**
+* **Type:**
   Optional[int]
 
 #### page_size
 
 The number of instance roles to display per page. Defaults to 10.
 
-- **Type:**
+* **Type:**
   Optional[int]
 
 #### total
 
 The total number of instance roles available.
 
-- **Type:**
+* **Type:**
   Optional[int]
 
 #### order
 
 A dictionary specifying the order in which instance roles are sorted.
 
-- **Type:**
+* **Type:**
   Optional[Dict]
 
 #### filters
 
 A filter object used to filter the instance roles listed.
 
-- **Type:**
+* **Type:**
   Optional[[InstanceRoleFilter](#bodosdk.models.instance_role.InstanceRoleFilter)]
 
-#### _class_ Config
+#### *class* Config
 
 Bases: `object`
 
 Configuration for Pydantic models.
 [https://docs.pydantic.dev/latest/api/config/](https://docs.pydantic.dev/latest/api/config/)
 
-#### allow*population_by_field_name *= True\_
+#### allow_population_by_field_name *= True*
 
-#### extra _= 'forbid'_
+#### extra *= 'forbid'*
 
 #### delete()
 
-#### filters _: [InstanceRoleFilter](#bodosdk.models.instance_role.InstanceRoleFilter) | None_
+#### filters *: [InstanceRoleFilter](#bodosdk.models.instance_role.InstanceRoleFilter) | None*
 
-#### order _: Dict | None_
+#### order *: Dict | None*
 
-#### page _: int | None_
+#### page *: int | None*
 
-#### page*size *: int | None\_
+#### page_size *: int | None*
 
-#### total _: int | None_
+#### total *: int | None*
 
 <a id="module-bodosdk.models.workspace"></a>
 
-### _class_ bodosdk.models.workspace.Workspace(org_client: IBodoOrganizationClient = None, \*, name: str | None = None, uuid: str | UUID | None = None, status: str | None = None, organizationUUID: str | UUID | None = None, networkData: [NetworkData](#bodosdk.models.common.NetworkData) | [AWSNetworkData](#bodosdk.models.common.AWSNetworkData) | None = None, createdBy: str | None = None, notebookAutoDeployEnabled: bool | None = None, assignedAt: datetime | None = None, customTags: Dict[str, Any] | None = None, jupyterLastActivity: datetime | None = None, jupyterIsActive: bool | None = False, cloudConfig: [AwsCloudConfig](#bodosdk.models.cloud_config.AwsCloudConfig) | [AzureCloudConfig](#bodosdk.models.cloud_config.AzureCloudConfig) | None = None)
+### *class* bodosdk.models.workspace.Workspace(org_client: IBodoOrganizationClient = None, \*, name: str | None = None, uuid: str | UUID | None = None, status: str | None = None, organizationUUID: str | UUID | None = None, networkData: [NetworkData](#bodosdk.models.common.NetworkData) | [AWSNetworkData](#bodosdk.models.common.AWSNetworkData) | None = None, createdBy: str | None = None, notebookAutoDeployEnabled: bool | None = None, assignedAt: datetime | None = None, customTags: Dict[str, Any] | None = None, jupyterLastActivity: datetime | None = None, jupyterIsActive: bool | None = False, cloudConfig: [AwsCloudConfig](#bodosdk.models.cloud_config.AwsCloudConfig) | [AzureCloudConfig](#bodosdk.models.cloud_config.AzureCloudConfig) | None = None)
 
 Bases: `SDKBaseModel`, `IWorkspace`
 
-#### assigned*at *: datetime | None\_
+#### assigned_at *: datetime | None*
 
-#### cloud*config *: [AwsCloudConfig](#bodosdk.models.cloud_config.AwsCloudConfig) | [AzureCloudConfig](#bodosdk.models.cloud_config.AzureCloudConfig) | None\_
+#### cloud_config *: [AwsCloudConfig](#bodosdk.models.cloud_config.AwsCloudConfig) | [AzureCloudConfig](#bodosdk.models.cloud_config.AzureCloudConfig) | None*
 
-#### created*by *: str | None\_
+#### created_by *: str | None*
 
-#### custom*tags *: Dict[str, Any] | None\_
+#### custom_tags *: Dict[str, Any] | None*
 
 #### delete()
 
 Deletes the workspace from the API based on its UUID and updates the instance’s properties
 with the response from the deletion API call.
 
-- **Returns:**
+* **Returns:**
   The Workspace instance after deletion, updated with the API’s response data.
 
-#### _property_ id
+#### *property* id
 
-#### jupyter*is_active *: bool | None\_
+#### jupyter_is_active *: bool | None*
 
-#### jupyter*last_activity *: datetime | None\_
+#### jupyter_last_activity *: datetime | None*
 
-#### name _: str | None_
+#### name *: str | None*
 
-#### network*data *: [NetworkData](#bodosdk.models.common.NetworkData) | [AWSNetworkData](#bodosdk.models.common.AWSNetworkData) | None\_
+#### network_data *: [NetworkData](#bodosdk.models.common.NetworkData) | [AWSNetworkData](#bodosdk.models.common.AWSNetworkData) | None*
 
-#### notebook*auto_deploy_enabled *: bool | None\_
+#### notebook_auto_deploy_enabled *: bool | None*
 
-#### organization*uuid *: str | UUID | None\_
+#### organization_uuid *: str | UUID | None*
 
-#### status _: str | None_
+#### status *: str | None*
 
 #### update_infra()
 
-#### uuid _: str | UUID | None_
+#### uuid *: str | UUID | None*
 
 #### wait_for_status(statuses, timeout=600, tick=30)
 
 Waits for the workspace to reach one of the specified states within a given timeout.
 
-- **Parameters:**
-  - **statuses** – A list of states to wait for.
-  - **timeout** – The maximum time to wait before raising a TimeoutException.
-  - **tick** – The interval between checks.
-- **Returns:**
+* **Parameters:**
+  * **statuses** – A list of states to wait for.
+  * **timeout** – The maximum time to wait before raising a TimeoutException.
+  * **tick** – The interval between checks.
+* **Returns:**
   The workspace instance, once it has reached one of the desired states.
-- **Raises:**
+* **Raises:**
   **TimeoutException** – If the workspace does not reach a desired state within the timeout.
 
-### _class_ bodosdk.models.workspace.WorkspaceFilter(\*, uuids: List[str] | None = None, names: List[str] | None = None, statuses: List[str] | None = None, organizationUUIDs: List[str] | None = None)
+### *class* bodosdk.models.workspace.WorkspaceFilter(\*, uuids: List[str] | None = None, names: List[str] | None = None, statuses: List[str] | None = None, organizationUUIDs: List[str] | None = None)
 
 Bases: `SDKBaseModel`, `IWorkspaceFilter`
 
-#### _class_ Config
+#### *class* Config
 
 Bases: `object`
 
-#### allow*population_by_field_name *= True\_
+#### allow_population_by_field_name *= True*
 
-#### extra _= 'forbid'_
+#### extra *= 'forbid'*
 
-#### ids _: List[str] | None_
+#### ids *: List[str] | None*
 
-#### names _: List[str] | None_
+#### names *: List[str] | None*
 
-#### organization*uuids *: List[str] | None\_
+#### organization_uuids *: List[str] | None*
 
-#### statuses _: List[str] | None_
+#### statuses *: List[str] | None*
 
-### _class_ bodosdk.models.workspace.WorkspaceList(org_client: IBodoOrganizationClient = None, \*, page: int | None = 0, pageSize: int | None = 10, total: int | None = None, order: Dict | None = None, filters: [WorkspaceFilter](#bodosdk.models.workspace.WorkspaceFilter) | None = None)
+### *class* bodosdk.models.workspace.WorkspaceList(org_client: IBodoOrganizationClient = None, \*, page: int | None = 0, pageSize: int | None = 10, total: int | None = None, order: Dict | None = None, filters: [WorkspaceFilter](#bodosdk.models.workspace.WorkspaceFilter) | None = None)
 
 Bases: `IWorkspaceList`, `SDKBaseModel`
 
-#### _class_ Config
+#### *class* Config
 
 Bases: `object`
 
-#### allow*population_by_field_name *= True\_
+#### allow_population_by_field_name *= True*
 
-#### extra _= 'forbid'_
+#### extra *= 'forbid'*
 
 #### delete()
 
 Deletes the workspaces present on the list
 
-- **Returns:**
+* **Returns:**
   WorkspaceListAPIModel
 
-#### filters _: [WorkspaceFilter](#bodosdk.models.workspace.WorkspaceFilter) | None_
+#### filters *: [WorkspaceFilter](#bodosdk.models.workspace.WorkspaceFilter) | None*
 
-#### order _: Dict | None_
+#### order *: Dict | None*
 
-#### page _: int | None_
+#### page *: int | None*
 
-#### page*size *: int | None\_
+#### page_size *: int | None*
 
-#### total _: int | None_
+#### total *: int | None*
 
 #### update_infra()
```

### Comparing `bodosdk-2.0.0rc1/bodosdk.egg-info/SOURCES.txt` & `bodosdk-2.0.0rc2/bodosdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc1/setup.py` & `bodosdk-2.0.0rc2/setup.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc1/tests/test_base.py` & `bodosdk-2.0.0rc2/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc1/versioneer.py` & `bodosdk-2.0.0rc2/versioneer.py`

 * *Files identical despite different names*

