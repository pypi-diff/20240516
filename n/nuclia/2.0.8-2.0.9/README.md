# Comparing `tmp/nuclia-2.0.8.tar.gz` & `tmp/nuclia-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuclia-2.0.8.tar", last modified: Mon Mar 18 16:03:49 2024, max compression
+gzip compressed data, was "nuclia-2.0.9.tar", last modified: Wed Mar 20 07:37:03 2024, max compression
```

## Comparing `nuclia-2.0.8.tar` & `nuclia-2.0.9.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-03-18 16:03:49.625145 nuclia-2.0.8/
--rw-r--r--   0 ebr        (501) staff       (20)       59 2024-03-18 16:03:48.000000 nuclia-2.0.8/.gitignore
--rw-r--r--   0 ebr        (501) staff       (20)        7 2024-03-18 16:03:48.000000 nuclia-2.0.8/.python-version
--rw-r--r--   0 ebr        (501) staff       (20)     3597 2024-03-18 16:03:48.000000 nuclia-2.0.8/CHANGELOG.md
--rw-r--r--   0 ebr        (501) staff       (20)     1063 2024-03-18 16:03:48.000000 nuclia-2.0.8/LICENSE
--rw-r--r--   0 ebr        (501) staff       (20)       83 2024-03-18 16:03:48.000000 nuclia-2.0.8/MANIFEST.in
--rw-r--r--   0 ebr        (501) staff       (20)      270 2024-03-18 16:03:48.000000 nuclia-2.0.8/Makefile
--rw-r--r--   0 ebr        (501) staff       (20)     2053 2024-03-18 16:03:49.625302 nuclia-2.0.8/PKG-INFO
--rw-r--r--   0 ebr        (501) staff       (20)      967 2024-03-18 16:03:48.000000 nuclia-2.0.8/README.md
--rw-r--r--   0 ebr        (501) staff       (20)        6 2024-03-18 16:03:48.000000 nuclia-2.0.8/VERSION
--rw-r--r--   0 ebr        (501) staff       (20)       24 2024-03-18 16:03:48.000000 nuclia-2.0.8/code-requirements.txt
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-03-18 16:03:49.608210 nuclia-2.0.8/docs/
--rw-r--r--   0 ebr        (501) staff       (20)      871 2024-03-18 16:03:48.000000 nuclia-2.0.8/docs/01-README.md
--rw-r--r--   0 ebr        (501) staff       (20)     1894 2024-03-18 16:03:48.000000 nuclia-2.0.8/docs/02-auth.md
--rw-r--r--   0 ebr        (501) staff       (20)     5530 2024-03-18 16:03:48.000000 nuclia-2.0.8/docs/03-kb.md
--rw-r--r--   0 ebr        (501) staff       (20)     3285 2024-03-18 16:03:48.000000 nuclia-2.0.8/docs/04-upload.md
--rw-r--r--   0 ebr        (501) staff       (20)     2357 2024-03-18 16:03:48.000000 nuclia-2.0.8/docs/05-search.md
--rw-r--r--   0 ebr        (501) staff       (20)     1234 2024-03-18 16:03:48.000000 nuclia-2.0.8/docs/06-read.md
--rw-r--r--   0 ebr        (501) staff       (20)     3247 2024-03-18 16:03:48.000000 nuclia-2.0.8/docs/07-nua.md
--rw-r--r--   0 ebr        (501) staff       (20)     1987 2024-03-18 16:03:48.000000 nuclia-2.0.8/docs/08-import-export.md
--rw-r--r--   0 ebr        (501) staff       (20)     2072 2024-03-18 16:03:48.000000 nuclia-2.0.8/docs/09-manage.md
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-03-18 16:03:49.610176 nuclia-2.0.8/nuclia/
--rw-r--r--   0 ebr        (501) staff       (20)      645 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/__init__.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-03-18 16:03:49.613046 nuclia-2.0.8/nuclia/cli/
--rw-r--r--   0 ebr        (501) staff       (20)        0 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/cli/__init__.py
--rw-r--r--   0 ebr        (501) staff       (20)     1522 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/cli/run.py
--rw-r--r--   0 ebr        (501) staff       (20)     1223 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/cli/utils.py
--rw-r--r--   0 ebr        (501) staff       (20)     8077 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/config.py
--rw-r--r--   0 ebr        (501) staff       (20)     1021 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/data.py
--rw-r--r--   0 ebr        (501) staff       (20)     8242 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/decorators.py
--rw-r--r--   0 ebr        (501) staff       (20)      521 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/exceptions.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-03-18 16:03:49.614819 nuclia-2.0.8/nuclia/lib/
--rw-r--r--   0 ebr        (501) staff       (20)        0 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/lib/__init__.py
--rw-r--r--   0 ebr        (501) staff       (20)      153 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/lib/conversations.py
--rw-r--r--   0 ebr        (501) staff       (20)    14145 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/lib/kb.py
--rw-r--r--   0 ebr        (501) staff       (20)    16530 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/lib/nua.py
--rw-r--r--   0 ebr        (501) staff       (20)    10085 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/lib/nua_responses.py
--rw-r--r--   0 ebr        (501) staff       (20)      472 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/lib/utils.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-03-18 16:03:49.619990 nuclia-2.0.8/nuclia/sdk/
--rw-r--r--   0 ebr        (501) staff       (20)      822 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/sdk/__init__.py
--rw-r--r--   0 ebr        (501) staff       (20)      647 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/sdk/accounts.py
--rw-r--r--   0 ebr        (501) staff       (20)     1966 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/sdk/agent.py
--rw-r--r--   0 ebr        (501) staff       (20)    20954 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/sdk/auth.py
--rw-r--r--   0 ebr        (501) staff       (20)     9654 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/sdk/export_import.py
--rw-r--r--   0 ebr        (501) staff       (20)     6035 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/sdk/kb.py
--rw-r--r--   0 ebr        (501) staff       (20)     4648 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/sdk/kbs.py
--rw-r--r--   0 ebr        (501) staff       (20)       57 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/sdk/logger.py
--rw-r--r--   0 ebr        (501) staff       (20)      462 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/sdk/logs.py
--rw-r--r--   0 ebr        (501) staff       (20)      369 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/sdk/nua.py
--rw-r--r--   0 ebr        (501) staff       (20)     1288 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/sdk/nucliadb.py
--rw-r--r--   0 ebr        (501) staff       (20)     4896 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/sdk/predict.py
--rw-r--r--   0 ebr        (501) staff       (20)     2196 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/sdk/process.py
--rw-r--r--   0 ebr        (501) staff       (20)     6870 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/sdk/resource.py
--rw-r--r--   0 ebr        (501) staff       (20)     7316 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/sdk/search.py
--rw-r--r--   0 ebr        (501) staff       (20)      188 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/sdk/train.py
--rw-r--r--   0 ebr        (501) staff       (20)    19774 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/sdk/upload.py
--rw-r--r--   0 ebr        (501) staff       (20)      342 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/sdk/zones.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-03-18 16:03:49.620647 nuclia-2.0.8/nuclia/tests/
--rw-r--r--   0 ebr        (501) staff       (20)        0 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/tests/__init__.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-03-18 16:03:49.620892 nuclia-2.0.8/nuclia/tests/assets/
--rw-r--r--   0 ebr        (501) staff       (20)      348 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/tests/assets/conversation.json
--rw-r--r--   0 ebr        (501) staff       (20)       74 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/tests/conftest.py
--rw-r--r--   0 ebr        (501) staff       (20)     1527 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/tests/fixtures.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-03-18 16:03:49.622283 nuclia-2.0.8/nuclia/tests/test_kb/
--rw-r--r--   0 ebr        (501) staff       (20)      741 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/tests/test_kb/test_conversation.py
--rw-r--r--   0 ebr        (501) staff       (20)     1019 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/tests/test_kb/test_export_import.py
--rw-r--r--   0 ebr        (501) staff       (20)      879 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/tests/test_kb/test_labels.py
--rw-r--r--   0 ebr        (501) staff       (20)      269 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/tests/test_kb/test_logs.py
--rw-r--r--   0 ebr        (501) staff       (20)      996 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/tests/test_kb/test_resource.py
--rw-r--r--   0 ebr        (501) staff       (20)      990 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/tests/test_kb/test_search.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-03-18 16:03:49.623201 nuclia-2.0.8/nuclia/tests/test_manage/
--rw-r--r--   0 ebr        (501) staff       (20)        0 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/tests/test_manage/__init__.py
--rw-r--r--   0 ebr        (501) staff       (20)      289 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/tests/test_manage/test_account.py
--rw-r--r--   0 ebr        (501) staff       (20)      540 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/tests/test_manage/test_auth.py
--rw-r--r--   0 ebr        (501) staff       (20)     1015 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/tests/test_manage/test_kb.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-03-18 16:03:49.623971 nuclia-2.0.8/nuclia/tests/test_nua/
--rw-r--r--   0 ebr        (501) staff       (20)        0 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/tests/test_nua/__init__.py
--rw-r--r--   0 ebr        (501) staff       (20)      334 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/tests/test_nua/test_agent.py
--rw-r--r--   0 ebr        (501) staff       (20)     1108 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/tests/test_nua/test_predict.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-03-18 16:03:49.624462 nuclia-2.0.8/nuclia/tests/test_nucliadb/
--rw-r--r--   0 ebr        (501) staff       (20)        0 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/tests/test_nucliadb/__init__.py
--rw-r--r--   0 ebr        (501) staff       (20)     1235 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/tests/test_nucliadb/test_crud.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-03-18 16:03:49.624930 nuclia-2.0.8/nuclia/tests/unit/
--rw-r--r--   0 ebr        (501) staff       (20)        0 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/tests/unit/__init__.py
--rw-r--r--   0 ebr        (501) staff       (20)      980 2024-03-18 16:03:48.000000 nuclia-2.0.8/nuclia/tests/unit/test_export_import.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-03-18 16:03:49.612227 nuclia-2.0.8/nuclia.egg-info/
--rw-r--r--   0 ebr        (501) staff       (20)     2053 2024-03-18 16:03:49.000000 nuclia-2.0.8/nuclia.egg-info/PKG-INFO
--rw-r--r--   0 ebr        (501) staff       (20)     1948 2024-03-18 16:03:49.000000 nuclia-2.0.8/nuclia.egg-info/SOURCES.txt
--rw-r--r--   0 ebr        (501) staff       (20)        1 2024-03-18 16:03:49.000000 nuclia-2.0.8/nuclia.egg-info/dependency_links.txt
--rw-r--r--   0 ebr        (501) staff       (20)       47 2024-03-18 16:03:49.000000 nuclia-2.0.8/nuclia.egg-info/entry_points.txt
--rw-r--r--   0 ebr        (501) staff       (20)      137 2024-03-18 16:03:49.000000 nuclia-2.0.8/nuclia.egg-info/requires.txt
--rw-r--r--   0 ebr        (501) staff       (20)        7 2024-03-18 16:03:49.000000 nuclia-2.0.8/nuclia.egg-info/top_level.txt
--rw-r--r--   0 ebr        (501) staff       (20)        1 2024-03-18 16:03:49.000000 nuclia-2.0.8/nuclia.egg-info/zip-safe
--rw-r--r--   0 ebr        (501) staff       (20)      137 2024-03-18 16:03:48.000000 nuclia-2.0.8/requirements.txt
--rw-r--r--   0 ebr        (501) staff       (20)      204 2024-03-18 16:03:49.625792 nuclia-2.0.8/setup.cfg
--rw-r--r--   0 ebr        (501) staff       (20)     1946 2024-03-18 16:03:48.000000 nuclia-2.0.8/setup.py
--rw-r--r--   0 ebr        (501) staff       (20)      211 2024-03-18 16:03:48.000000 nuclia-2.0.8/test-requirements.txt
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-03-20 07:37:03.067428 nuclia-2.0.9/
+-rw-r--r--   0 ebr        (501) staff       (20)       59 2024-03-20 07:37:02.000000 nuclia-2.0.9/.gitignore
+-rw-r--r--   0 ebr        (501) staff       (20)        7 2024-03-20 07:37:02.000000 nuclia-2.0.9/.python-version
+-rw-r--r--   0 ebr        (501) staff       (20)     3647 2024-03-20 07:37:02.000000 nuclia-2.0.9/CHANGELOG.md
+-rw-r--r--   0 ebr        (501) staff       (20)     1063 2024-03-20 07:37:02.000000 nuclia-2.0.9/LICENSE
+-rw-r--r--   0 ebr        (501) staff       (20)       83 2024-03-20 07:37:02.000000 nuclia-2.0.9/MANIFEST.in
+-rw-r--r--   0 ebr        (501) staff       (20)      270 2024-03-20 07:37:02.000000 nuclia-2.0.9/Makefile
+-rw-r--r--   0 ebr        (501) staff       (20)     2053 2024-03-20 07:37:03.067598 nuclia-2.0.9/PKG-INFO
+-rw-r--r--   0 ebr        (501) staff       (20)      967 2024-03-20 07:37:02.000000 nuclia-2.0.9/README.md
+-rw-r--r--   0 ebr        (501) staff       (20)        6 2024-03-20 07:37:02.000000 nuclia-2.0.9/VERSION
+-rw-r--r--   0 ebr        (501) staff       (20)       24 2024-03-20 07:37:02.000000 nuclia-2.0.9/code-requirements.txt
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-03-20 07:37:03.037974 nuclia-2.0.9/docs/
+-rw-r--r--   0 ebr        (501) staff       (20)      871 2024-03-20 07:37:02.000000 nuclia-2.0.9/docs/01-README.md
+-rw-r--r--   0 ebr        (501) staff       (20)     1894 2024-03-20 07:37:02.000000 nuclia-2.0.9/docs/02-auth.md
+-rw-r--r--   0 ebr        (501) staff       (20)     5530 2024-03-20 07:37:02.000000 nuclia-2.0.9/docs/03-kb.md
+-rw-r--r--   0 ebr        (501) staff       (20)     3285 2024-03-20 07:37:02.000000 nuclia-2.0.9/docs/04-upload.md
+-rw-r--r--   0 ebr        (501) staff       (20)     2357 2024-03-20 07:37:02.000000 nuclia-2.0.9/docs/05-search.md
+-rw-r--r--   0 ebr        (501) staff       (20)     1234 2024-03-20 07:37:02.000000 nuclia-2.0.9/docs/06-read.md
+-rw-r--r--   0 ebr        (501) staff       (20)     3247 2024-03-20 07:37:02.000000 nuclia-2.0.9/docs/07-nua.md
+-rw-r--r--   0 ebr        (501) staff       (20)     1987 2024-03-20 07:37:02.000000 nuclia-2.0.9/docs/08-import-export.md
+-rw-r--r--   0 ebr        (501) staff       (20)     2072 2024-03-20 07:37:02.000000 nuclia-2.0.9/docs/09-manage.md
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-03-20 07:37:03.039909 nuclia-2.0.9/nuclia/
+-rw-r--r--   0 ebr        (501) staff       (20)      645 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/__init__.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-03-20 07:37:03.046312 nuclia-2.0.9/nuclia/cli/
+-rw-r--r--   0 ebr        (501) staff       (20)        0 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/cli/__init__.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1522 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/cli/run.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1223 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/cli/utils.py
+-rw-r--r--   0 ebr        (501) staff       (20)     8077 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/config.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1021 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/data.py
+-rw-r--r--   0 ebr        (501) staff       (20)     8242 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/decorators.py
+-rw-r--r--   0 ebr        (501) staff       (20)      521 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/exceptions.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-03-20 07:37:03.047912 nuclia-2.0.9/nuclia/lib/
+-rw-r--r--   0 ebr        (501) staff       (20)        0 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/lib/__init__.py
+-rw-r--r--   0 ebr        (501) staff       (20)      153 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/lib/conversations.py
+-rw-r--r--   0 ebr        (501) staff       (20)    14202 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/lib/kb.py
+-rw-r--r--   0 ebr        (501) staff       (20)    16530 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/lib/nua.py
+-rw-r--r--   0 ebr        (501) staff       (20)    10083 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/lib/nua_responses.py
+-rw-r--r--   0 ebr        (501) staff       (20)      472 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/lib/utils.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-03-20 07:37:03.057603 nuclia-2.0.9/nuclia/sdk/
+-rw-r--r--   0 ebr        (501) staff       (20)      822 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/sdk/__init__.py
+-rw-r--r--   0 ebr        (501) staff       (20)      647 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/sdk/accounts.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1966 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/sdk/agent.py
+-rw-r--r--   0 ebr        (501) staff       (20)    20954 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/sdk/auth.py
+-rw-r--r--   0 ebr        (501) staff       (20)     9654 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/sdk/export_import.py
+-rw-r--r--   0 ebr        (501) staff       (20)     6035 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/sdk/kb.py
+-rw-r--r--   0 ebr        (501) staff       (20)     4648 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/sdk/kbs.py
+-rw-r--r--   0 ebr        (501) staff       (20)       57 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/sdk/logger.py
+-rw-r--r--   0 ebr        (501) staff       (20)      462 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/sdk/logs.py
+-rw-r--r--   0 ebr        (501) staff       (20)      369 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/sdk/nua.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1288 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/sdk/nucliadb.py
+-rw-r--r--   0 ebr        (501) staff       (20)     4896 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/sdk/predict.py
+-rw-r--r--   0 ebr        (501) staff       (20)     2196 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/sdk/process.py
+-rw-r--r--   0 ebr        (501) staff       (20)     6870 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/sdk/resource.py
+-rw-r--r--   0 ebr        (501) staff       (20)     7361 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/sdk/search.py
+-rw-r--r--   0 ebr        (501) staff       (20)      188 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/sdk/train.py
+-rw-r--r--   0 ebr        (501) staff       (20)    19774 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/sdk/upload.py
+-rw-r--r--   0 ebr        (501) staff       (20)      342 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/sdk/zones.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-03-20 07:37:03.058622 nuclia-2.0.9/nuclia/tests/
+-rw-r--r--   0 ebr        (501) staff       (20)        0 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/tests/__init__.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-03-20 07:37:03.059278 nuclia-2.0.9/nuclia/tests/assets/
+-rw-r--r--   0 ebr        (501) staff       (20)      348 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/tests/assets/conversation.json
+-rw-r--r--   0 ebr        (501) staff       (20)       74 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/tests/conftest.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1527 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/tests/fixtures.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-03-20 07:37:03.062492 nuclia-2.0.9/nuclia/tests/test_kb/
+-rw-r--r--   0 ebr        (501) staff       (20)      741 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/tests/test_kb/test_conversation.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1019 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/tests/test_kb/test_export_import.py
+-rw-r--r--   0 ebr        (501) staff       (20)      879 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/tests/test_kb/test_labels.py
+-rw-r--r--   0 ebr        (501) staff       (20)      269 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/tests/test_kb/test_logs.py
+-rw-r--r--   0 ebr        (501) staff       (20)      996 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/tests/test_kb/test_resource.py
+-rw-r--r--   0 ebr        (501) staff       (20)      990 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/tests/test_kb/test_search.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-03-20 07:37:03.064166 nuclia-2.0.9/nuclia/tests/test_manage/
+-rw-r--r--   0 ebr        (501) staff       (20)        0 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/tests/test_manage/__init__.py
+-rw-r--r--   0 ebr        (501) staff       (20)      289 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/tests/test_manage/test_account.py
+-rw-r--r--   0 ebr        (501) staff       (20)      540 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/tests/test_manage/test_auth.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1015 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/tests/test_manage/test_kb.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-03-20 07:37:03.065611 nuclia-2.0.9/nuclia/tests/test_nua/
+-rw-r--r--   0 ebr        (501) staff       (20)        0 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/tests/test_nua/__init__.py
+-rw-r--r--   0 ebr        (501) staff       (20)      334 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/tests/test_nua/test_agent.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1108 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/tests/test_nua/test_predict.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-03-20 07:37:03.066275 nuclia-2.0.9/nuclia/tests/test_nucliadb/
+-rw-r--r--   0 ebr        (501) staff       (20)        0 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/tests/test_nucliadb/__init__.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1235 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/tests/test_nucliadb/test_crud.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-03-20 07:37:03.067059 nuclia-2.0.9/nuclia/tests/unit/
+-rw-r--r--   0 ebr        (501) staff       (20)        0 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/tests/unit/__init__.py
+-rw-r--r--   0 ebr        (501) staff       (20)      980 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/tests/unit/test_export_import.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-03-20 07:37:03.044915 nuclia-2.0.9/nuclia.egg-info/
+-rw-r--r--   0 ebr        (501) staff       (20)     2053 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia.egg-info/PKG-INFO
+-rw-r--r--   0 ebr        (501) staff       (20)     1948 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia.egg-info/SOURCES.txt
+-rw-r--r--   0 ebr        (501) staff       (20)        1 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia.egg-info/dependency_links.txt
+-rw-r--r--   0 ebr        (501) staff       (20)       47 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia.egg-info/entry_points.txt
+-rw-r--r--   0 ebr        (501) staff       (20)      137 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia.egg-info/requires.txt
+-rw-r--r--   0 ebr        (501) staff       (20)        7 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia.egg-info/top_level.txt
+-rw-r--r--   0 ebr        (501) staff       (20)        1 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia.egg-info/zip-safe
+-rw-r--r--   0 ebr        (501) staff       (20)      137 2024-03-20 07:37:02.000000 nuclia-2.0.9/requirements.txt
+-rw-r--r--   0 ebr        (501) staff       (20)      204 2024-03-20 07:37:03.068421 nuclia-2.0.9/setup.cfg
+-rw-r--r--   0 ebr        (501) staff       (20)     1946 2024-03-20 07:37:02.000000 nuclia-2.0.9/setup.py
+-rw-r--r--   0 ebr        (501) staff       (20)      211 2024-03-20 07:37:02.000000 nuclia-2.0.9/test-requirements.txt
```

### Comparing `nuclia-2.0.8/CHANGELOG.md` & `nuclia-2.0.9/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Changelog
 
+## 2.0.9 (2024-03-20)
+
+
+- Chat needs a timeout.
+
+
 ## 2.0.8 (2024-03-18)
 
 
 - Support CSS selector when uploading links
 
 
 ## 2.0.7 (2024-03-18)
```

### Comparing `nuclia-2.0.8/LICENSE` & `nuclia-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.8/PKG-INFO` & `nuclia-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuclia
-Version: 2.0.8
+Version: 2.0.9
 Summary: UNKNOWN
 Home-page: https://nuclia.com
 Author: Nuclia
 Author-email: info@nuclia.com
 License: BSD
 Project-URL: Nuclia, https://nuclia.com
 Project-URL: Github, https://github.com/nuclia/nucliadb
```

### Comparing `nuclia-2.0.8/README.md` & `nuclia-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.8/docs/01-README.md` & `nuclia-2.0.9/docs/01-README.md`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.8/docs/02-auth.md` & `nuclia-2.0.9/docs/02-auth.md`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.8/docs/03-kb.md` & `nuclia-2.0.9/docs/03-kb.md`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.8/docs/04-upload.md` & `nuclia-2.0.9/docs/04-upload.md`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.8/docs/05-search.md` & `nuclia-2.0.9/docs/05-search.md`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.8/docs/06-read.md` & `nuclia-2.0.9/docs/06-read.md`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.8/docs/07-nua.md` & `nuclia-2.0.9/docs/07-nua.md`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.8/docs/08-import-export.md` & `nuclia-2.0.9/docs/08-import-export.md`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.8/docs/09-manage.md` & `nuclia-2.0.9/docs/09-manage.md`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.8/nuclia/__init__.py` & `nuclia-2.0.9/nuclia/__init__.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.8/nuclia/cli/run.py` & `nuclia-2.0.9/nuclia/cli/run.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.8/nuclia/cli/utils.py` & `nuclia-2.0.9/nuclia/cli/utils.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.8/nuclia/config.py` & `nuclia-2.0.9/nuclia/config.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.8/nuclia/data.py` & `nuclia-2.0.9/nuclia/data.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.8/nuclia/decorators.py` & `nuclia-2.0.9/nuclia/decorators.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.8/nuclia/exceptions.py` & `nuclia-2.0.9/nuclia/exceptions.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.8/nuclia/lib/kb.py` & `nuclia-2.0.9/nuclia/lib/kb.py`

 * *Files 0% similar despite different names*

```diff
@@ -303,19 +303,21 @@
             self.reader_session = httpx.AsyncClient(
                 headers=self.reader_headers, base_url=url  # type: ignore
             )
             self.writer_session = httpx.AsyncClient(
                 headers=self.writer_headers, base_url=url  # type: ignore
             )
 
-    async def chat(self, request: ChatRequest):
+    async def chat(self, request: ChatRequest, timeout: int = 1000):
         if self.url is None or self.reader_session is None:
             raise Exception("KB not configured")
         url = f"{self.url}{CHAT_URL}"
-        req = self.reader_session.build_request("POST", url, json=request.dict())
+        req = self.reader_session.build_request(
+            "POST", url, json=request.dict(), timeout=1000
+        )
         response = await self.reader_session.send(req, stream=True)
         handle_http_errors(response)
         return response
 
     async def download_export(self, export_id: str, path: str, chunk_size: int):
         if self.reader_session is None:
             raise Exception("KB not configured")
```

### Comparing `nuclia-2.0.8/nuclia/lib/nua.py` & `nuclia-2.0.9/nuclia/lib/nua.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.8/nuclia/lib/nua_responses.py` & `nuclia-2.0.9/nuclia/lib/nua_responses.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,17 +270,17 @@
     account_seq: Optional[int] = None
     queue: Optional[ProcessingQueueType] = None
     # On Public api, uuid may be generated by the proxy, so we need to return it to the user
     uuid: Optional[str] = None
 
 
 class ProcessingStatusInfo(BaseModel):
-    last_delivered_seqid: Optional[int] = (
-        None  # When none, means we already don't have information about this queue
-    )
+    last_delivered_seqid: Optional[
+        int
+    ] = None  # When none, means we already don't have information about this queue
 
 
 class ProcessingStatus(BaseModel):
     shared: ProcessingStatusInfo
     account: Optional[ProcessingStatusInfo]
```

### Comparing `nuclia-2.0.8/nuclia/sdk/__init__.py` & `nuclia-2.0.9/nuclia/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.8/nuclia/sdk/accounts.py` & `nuclia-2.0.9/nuclia/sdk/accounts.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.8/nuclia/sdk/agent.py` & `nuclia-2.0.9/nuclia/sdk/agent.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.8/nuclia/sdk/auth.py` & `nuclia-2.0.9/nuclia/sdk/auth.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.8/nuclia/sdk/export_import.py` & `nuclia-2.0.9/nuclia/sdk/export_import.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.8/nuclia/sdk/kb.py` & `nuclia-2.0.9/nuclia/sdk/kb.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.8/nuclia/sdk/kbs.py` & `nuclia-2.0.9/nuclia/sdk/kbs.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.8/nuclia/sdk/nucliadb.py` & `nuclia-2.0.9/nuclia/sdk/nucliadb.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.8/nuclia/sdk/predict.py` & `nuclia-2.0.9/nuclia/sdk/predict.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.8/nuclia/sdk/process.py` & `nuclia-2.0.9/nuclia/sdk/process.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.8/nuclia/sdk/resource.py` & `nuclia-2.0.9/nuclia/sdk/resource.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.8/nuclia/sdk/search.py` & `nuclia-2.0.9/nuclia/sdk/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,29 +214,30 @@
 
     @kb
     async def chat(
         self,
         *,
         query: Union[str, ChatRequest],
         filters: Optional[List[str]] = None,
+        timeout: int = 100,
         **kwargs,
     ):
         """
         Answer a question.
 
         See https://docs.nuclia.dev/docs/api#tag/Search/operation/Chat_Knowledge_Box_kb__kbid__chat_post
         """
         ndb: AsyncNucliaDBClient = kwargs["ndb"]
         if isinstance(query, str):
             req = ChatRequest(query=query, filters=(filters or []))
         else:
             req = query
 
         content = b""
-        response = await ndb.chat(req)
+        response = await ndb.chat(req, timeout=timeout)
 
         content = await response.aread()
         stream = BytesIO(content)
         header = stream.read(4)
         payload_size = int.from_bytes(header, byteorder="big", signed=False)
         data = stream.read(payload_size)
```

### Comparing `nuclia-2.0.8/nuclia/sdk/upload.py` & `nuclia-2.0.9/nuclia/sdk/upload.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.8/nuclia/tests/fixtures.py` & `nuclia-2.0.9/nuclia/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.8/nuclia/tests/test_kb/test_conversation.py` & `nuclia-2.0.9/nuclia/tests/test_kb/test_conversation.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.8/nuclia/tests/test_kb/test_export_import.py` & `nuclia-2.0.9/nuclia/tests/test_kb/test_export_import.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.8/nuclia/tests/test_kb/test_labels.py` & `nuclia-2.0.9/nuclia/tests/test_kb/test_labels.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.8/nuclia/tests/test_kb/test_resource.py` & `nuclia-2.0.9/nuclia/tests/test_kb/test_resource.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.8/nuclia/tests/test_kb/test_search.py` & `nuclia-2.0.9/nuclia/tests/test_kb/test_search.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.8/nuclia/tests/test_manage/test_auth.py` & `nuclia-2.0.9/nuclia/tests/test_manage/test_auth.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.8/nuclia/tests/test_manage/test_kb.py` & `nuclia-2.0.9/nuclia/tests/test_manage/test_kb.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.8/nuclia/tests/test_nua/test_predict.py` & `nuclia-2.0.9/nuclia/tests/test_nua/test_predict.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.8/nuclia/tests/test_nucliadb/test_crud.py` & `nuclia-2.0.9/nuclia/tests/test_nucliadb/test_crud.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.8/nuclia/tests/unit/test_export_import.py` & `nuclia-2.0.9/nuclia/tests/unit/test_export_import.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.8/nuclia.egg-info/PKG-INFO` & `nuclia-2.0.9/nuclia.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuclia
-Version: 2.0.8
+Version: 2.0.9
 Summary: UNKNOWN
 Home-page: https://nuclia.com
 Author: Nuclia
 Author-email: info@nuclia.com
 License: BSD
 Project-URL: Nuclia, https://nuclia.com
 Project-URL: Github, https://github.com/nuclia/nucliadb
```

### Comparing `nuclia-2.0.8/nuclia.egg-info/SOURCES.txt` & `nuclia-2.0.9/nuclia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.8/setup.py` & `nuclia-2.0.9/setup.py`

 * *Files identical despite different names*

