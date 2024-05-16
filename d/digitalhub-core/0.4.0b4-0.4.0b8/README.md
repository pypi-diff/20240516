# Comparing `tmp/digitalhub_core-0.4.0b4.tar.gz` & `tmp/digitalhub_core-0.4.0b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digitalhub_core-0.4.0b4.tar", last modified: Fri May  3 12:54:09 2024, max compression
+gzip compressed data, was "digitalhub_core-0.4.0b8.tar", last modified: Tue May 14 10:36:05 2024, max compression
```

## Comparing `digitalhub_core-0.4.0b4.tar` & `digitalhub_core-0.4.0b8.tar`

### file list

```diff
@@ -1,128 +1,129 @@
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-03 12:54:09.402963 digitalhub_core-0.4.0b4/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    11585 2023-08-23 08:29:57.000000 digitalhub_core-0.4.0b4/LICENSE.txt
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)    15054 2024-05-03 12:54:09.402963 digitalhub_core-0.4.0b4/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      499 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b4/README.md
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-03 12:54:09.374963 digitalhub_core-0.4.0b4/digitalhub_core/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1259 2024-05-03 12:46:14.000000 digitalhub_core-0.4.0b4/digitalhub_core/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-03 12:54:09.374963 digitalhub_core-0.4.0b4/digitalhub_core/client/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b4/digitalhub_core/client/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2352 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b4/digitalhub_core/client/builder.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-03 12:54:09.374963 digitalhub_core-0.4.0b4/digitalhub_core/client/objects/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-10-10 11:19:53.000000 digitalhub_core-0.4.0b4/digitalhub_core/client/objects/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1166 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b4/digitalhub_core/client/objects/base.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8892 2024-05-02 13:03:59.000000 digitalhub_core-0.4.0b4/digitalhub_core/client/objects/dhcore.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    15662 2024-04-24 12:58:10.000000 digitalhub_core-0.4.0b4/digitalhub_core/client/objects/local.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-03 12:54:09.378963 digitalhub_core-0.4.0b4/digitalhub_core/context/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b4/digitalhub_core/context/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3098 2024-03-12 14:22:03.000000 digitalhub_core-0.4.0b4/digitalhub_core/context/builder.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2926 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b4/digitalhub_core/context/context.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-03 12:54:09.378963 digitalhub_core-0.4.0b4/digitalhub_core/entities/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-03 12:54:09.378963 digitalhub_core-0.4.0b4/digitalhub_core/entities/_base/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/_base/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1521 2024-02-05 10:28:22.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/_base/base.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3172 2024-05-02 12:54:20.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/_base/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2485 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/_base/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1024 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/_base/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1567 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/_base/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-03 12:54:09.378963 digitalhub_core-0.4.0b4/digitalhub_core/entities/_builders/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-09-27 11:31:31.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/_builders/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1801 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/_builders/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1442 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/_builders/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1755 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/_builders/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-03 12:54:09.378963 digitalhub_core-0.4.0b4/digitalhub_core/entities/artifacts/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/artifacts/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6563 2024-05-03 12:46:15.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/artifacts/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    13877 2024-05-03 12:46:15.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/artifacts/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      339 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/artifacts/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1876 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/artifacts/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      322 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/artifacts/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-03 12:54:09.382963 digitalhub_core-0.4.0b4/digitalhub_core/entities/functions/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/functions/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6220 2024-05-03 12:46:15.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/functions/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    16504 2024-05-03 12:46:15.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/functions/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      227 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/functions/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1699 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/functions/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      218 2024-02-22 07:49:08.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/functions/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-03 12:54:09.382963 digitalhub_core-0.4.0b4/digitalhub_core/entities/projects/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/projects/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8627 2024-05-03 12:46:15.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/projects/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    21749 2024-05-03 12:46:16.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/projects/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      224 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/projects/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1467 2024-02-29 07:59:41.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/projects/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      215 2024-02-15 09:23:23.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/projects/status.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1894 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/registries.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-03 12:54:09.382963 digitalhub_core-0.4.0b4/digitalhub_core/entities/runs/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/runs/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4819 2024-05-03 12:46:15.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/runs/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    14158 2024-05-03 12:46:15.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/runs/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      212 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/runs/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3620 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/runs/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2692 2024-03-20 12:21:43.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/runs/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-03 12:54:09.382963 digitalhub_core-0.4.0b4/digitalhub_core/entities/secrets/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-06 10:39:09.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/secrets/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6082 2024-05-03 12:46:15.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/secrets/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8589 2024-05-03 12:46:15.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/secrets/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      221 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/secrets/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      746 2024-02-15 09:49:55.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/secrets/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      212 2024-02-15 09:23:29.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/secrets/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-03 12:54:09.386963 digitalhub_core-0.4.0b4/digitalhub_core/entities/services/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-06 10:49:32.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/services/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6043 2024-05-03 12:46:15.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/services/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     7249 2024-05-03 12:46:15.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/services/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      224 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/services/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      368 2024-02-15 09:49:55.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/services/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      215 2024-02-15 09:23:37.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/services/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-03 12:54:09.386963 digitalhub_core-0.4.0b4/digitalhub_core/entities/tasks/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/tasks/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5472 2024-05-03 12:46:15.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/tasks/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    10491 2024-05-03 12:46:15.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/tasks/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      215 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/tasks/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5151 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/tasks/models.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      431 2024-03-19 10:12:26.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/tasks/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      206 2023-11-17 12:02:01.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/tasks/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-03 12:54:09.386963 digitalhub_core-0.4.0b4/digitalhub_core/entities/workflows/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/workflows/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6280 2024-05-03 12:46:15.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/workflows/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    15763 2024-05-03 12:46:16.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/workflows/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      227 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/workflows/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      295 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/workflows/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      218 2024-02-15 09:23:47.000000 digitalhub_core-0.4.0b4/digitalhub_core/entities/workflows/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-03 12:54:09.386963 digitalhub_core-0.4.0b4/digitalhub_core/registry/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b4/digitalhub_core/registry/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2543 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b4/digitalhub_core/registry/import_utils.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1468 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b4/digitalhub_core/registry/models.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1866 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b4/digitalhub_core/registry/registry.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-03 12:54:09.386963 digitalhub_core-0.4.0b4/digitalhub_core/runtimes/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-09-05 11:37:04.000000 digitalhub_core-0.4.0b4/digitalhub_core/runtimes/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3931 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b4/digitalhub_core/runtimes/base.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1012 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b4/digitalhub_core/runtimes/builder.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-03 12:54:09.390963 digitalhub_core-0.4.0b4/digitalhub_core/stores/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b4/digitalhub_core/stores/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6767 2024-05-03 12:46:15.000000 digitalhub_core-0.4.0b4/digitalhub_core/stores/builder.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-03 12:54:09.394963 digitalhub_core-0.4.0b4/digitalhub_core/stores/objects/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b4/digitalhub_core/stores/objects/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4587 2024-04-19 08:14:45.000000 digitalhub_core-0.4.0b4/digitalhub_core/stores/objects/base.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4508 2024-03-12 13:41:08.000000 digitalhub_core-0.4.0b4/digitalhub_core/stores/objects/local.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5039 2024-04-19 08:14:45.000000 digitalhub_core-0.4.0b4/digitalhub_core/stores/objects/remote.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8844 2024-04-19 08:14:45.000000 digitalhub_core-0.4.0b4/digitalhub_core/stores/objects/s3.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8927 2024-04-19 08:14:45.000000 digitalhub_core-0.4.0b4/digitalhub_core/stores/objects/sql.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-03 12:54:09.398963 digitalhub_core-0.4.0b4/digitalhub_core/utils/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b4/digitalhub_core/utils/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3646 2024-03-12 14:23:02.000000 digitalhub_core-0.4.0b4/digitalhub_core/utils/api.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2215 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b4/digitalhub_core/utils/env_utils.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      346 2023-12-11 08:31:30.000000 digitalhub_core-0.4.0b4/digitalhub_core/utils/exceptions.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1332 2024-04-08 14:07:02.000000 digitalhub_core-0.4.0b4/digitalhub_core/utils/file_utils.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4237 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b4/digitalhub_core/utils/generic_utils.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3054 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b4/digitalhub_core/utils/git_utils.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1794 2024-02-01 10:08:51.000000 digitalhub_core-0.4.0b4/digitalhub_core/utils/io_utils.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      460 2023-11-21 13:33:17.000000 digitalhub_core-0.4.0b4/digitalhub_core/utils/logger.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      805 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b4/digitalhub_core/utils/uri_utils.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-03 12:54:09.398963 digitalhub_core-0.4.0b4/digitalhub_core.egg-info/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)    15054 2024-05-03 12:54:09.000000 digitalhub_core-0.4.0b4/digitalhub_core.egg-info/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4131 2024-05-03 12:54:09.000000 digitalhub_core-0.4.0b4/digitalhub_core.egg-info/SOURCES.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-05-03 12:54:09.000000 digitalhub_core-0.4.0b4/digitalhub_core.egg-info/dependency_links.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      250 2024-05-03 12:54:09.000000 digitalhub_core-0.4.0b4/digitalhub_core.egg-info/requires.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-05-03 12:54:09.000000 digitalhub_core-0.4.0b4/digitalhub_core.egg-info/top_level.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1731 2024-05-03 12:31:18.000000 digitalhub_core-0.4.0b4/pyproject.toml
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-05-03 12:54:09.402963 digitalhub_core-0.4.0b4/setup.cfg
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:36:05.005934 digitalhub_core-0.4.0b8/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    11585 2023-08-23 08:29:57.000000 digitalhub_core-0.4.0b8/LICENSE.txt
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)    15054 2024-05-14 10:36:05.005934 digitalhub_core-0.4.0b8/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      499 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/README.md
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:36:04.957934 digitalhub_core-0.4.0b8/digitalhub_core/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1259 2024-05-13 12:39:44.000000 digitalhub_core-0.4.0b8/digitalhub_core/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:36:04.961934 digitalhub_core-0.4.0b8/digitalhub_core/client/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b8/digitalhub_core/client/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2352 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/client/builder.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:36:04.961934 digitalhub_core-0.4.0b8/digitalhub_core/client/objects/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-10-10 11:19:53.000000 digitalhub_core-0.4.0b8/digitalhub_core/client/objects/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1166 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/client/objects/base.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8892 2024-05-02 13:03:59.000000 digitalhub_core-0.4.0b8/digitalhub_core/client/objects/dhcore.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    16292 2024-05-13 12:38:37.000000 digitalhub_core-0.4.0b8/digitalhub_core/client/objects/local.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:36:04.965934 digitalhub_core-0.4.0b8/digitalhub_core/context/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b8/digitalhub_core/context/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3098 2024-03-12 14:22:03.000000 digitalhub_core-0.4.0b8/digitalhub_core/context/builder.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2926 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/context/context.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:36:04.965934 digitalhub_core-0.4.0b8/digitalhub_core/entities/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:36:04.969934 digitalhub_core-0.4.0b8/digitalhub_core/entities/_base/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/_base/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1521 2024-02-05 10:28:22.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/_base/base.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3172 2024-05-02 12:54:20.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/_base/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2485 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/_base/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1024 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/_base/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1567 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/_base/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:36:04.969934 digitalhub_core-0.4.0b8/digitalhub_core/entities/_builders/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-09-27 11:31:31.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/_builders/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1794 2024-05-06 11:10:34.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/_builders/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1435 2024-05-06 11:10:34.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/_builders/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1748 2024-05-06 11:10:34.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/_builders/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:36:04.973934 digitalhub_core-0.4.0b8/digitalhub_core/entities/artifacts/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/artifacts/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6641 2024-05-13 12:39:44.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/artifacts/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    14010 2024-05-13 12:39:44.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/artifacts/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      339 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/artifacts/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1876 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/artifacts/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      322 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/artifacts/status.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      318 2024-05-06 11:13:11.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/entity_types.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:36:04.977934 digitalhub_core-0.4.0b8/digitalhub_core/entities/functions/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/functions/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6298 2024-05-13 12:39:44.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/functions/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    16737 2024-05-13 12:39:44.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/functions/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      227 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/functions/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1699 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/functions/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      218 2024-02-22 07:49:08.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/functions/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:36:04.977934 digitalhub_core-0.4.0b8/digitalhub_core/entities/projects/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/projects/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8705 2024-05-13 12:39:44.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/projects/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    22032 2024-05-13 12:39:44.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/projects/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      224 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/projects/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1467 2024-02-29 07:59:41.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/projects/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      215 2024-02-15 09:23:23.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/projects/status.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      927 2024-05-06 11:13:11.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/registries.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:36:04.981934 digitalhub_core-0.4.0b8/digitalhub_core/entities/runs/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/runs/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4897 2024-05-13 12:39:44.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/runs/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    14326 2024-05-13 12:39:44.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/runs/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      212 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/runs/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3532 2024-05-09 11:08:45.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/runs/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2620 2024-05-13 12:22:42.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/runs/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:36:04.985934 digitalhub_core-0.4.0b8/digitalhub_core/entities/secrets/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-06 10:39:09.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/secrets/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6160 2024-05-13 12:39:44.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/secrets/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8742 2024-05-13 12:39:44.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/secrets/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      221 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/secrets/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      746 2024-02-15 09:49:55.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/secrets/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      212 2024-02-15 09:23:29.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/secrets/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:36:04.989934 digitalhub_core-0.4.0b8/digitalhub_core/entities/services/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-06 10:49:32.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/services/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6121 2024-05-13 12:39:44.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/services/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     7385 2024-05-13 12:39:44.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/services/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      224 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/services/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      368 2024-02-15 09:49:55.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/services/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      215 2024-02-15 09:23:37.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/services/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:36:04.993934 digitalhub_core-0.4.0b8/digitalhub_core/entities/tasks/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/tasks/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5550 2024-05-13 12:39:44.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/tasks/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    10643 2024-05-13 12:39:44.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/tasks/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      215 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/tasks/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5151 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/tasks/models.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      431 2024-03-19 10:12:26.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/tasks/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      206 2023-11-17 12:02:01.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/tasks/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:36:04.993934 digitalhub_core-0.4.0b8/digitalhub_core/entities/workflows/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/workflows/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6358 2024-05-13 12:39:44.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/workflows/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    16023 2024-05-13 12:39:44.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/workflows/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      227 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/workflows/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      295 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/workflows/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      218 2024-02-15 09:23:47.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/workflows/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:36:04.993934 digitalhub_core-0.4.0b8/digitalhub_core/registry/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/registry/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1468 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/registry/models.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1866 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/registry/registry.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3714 2024-05-06 11:10:35.000000 digitalhub_core-0.4.0b8/digitalhub_core/registry/utils.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:36:04.997934 digitalhub_core-0.4.0b8/digitalhub_core/runtimes/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-09-05 11:37:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/runtimes/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3931 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/runtimes/base.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1005 2024-05-06 11:10:34.000000 digitalhub_core-0.4.0b8/digitalhub_core/runtimes/builder.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:36:04.997934 digitalhub_core-0.4.0b8/digitalhub_core/stores/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b8/digitalhub_core/stores/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6767 2024-05-13 12:39:44.000000 digitalhub_core-0.4.0b8/digitalhub_core/stores/builder.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:36:04.997934 digitalhub_core-0.4.0b8/digitalhub_core/stores/objects/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b8/digitalhub_core/stores/objects/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4587 2024-04-19 08:14:45.000000 digitalhub_core-0.4.0b8/digitalhub_core/stores/objects/base.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4508 2024-03-12 13:41:08.000000 digitalhub_core-0.4.0b8/digitalhub_core/stores/objects/local.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5039 2024-04-19 08:14:45.000000 digitalhub_core-0.4.0b8/digitalhub_core/stores/objects/remote.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8844 2024-04-19 08:14:45.000000 digitalhub_core-0.4.0b8/digitalhub_core/stores/objects/s3.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8927 2024-04-19 08:14:45.000000 digitalhub_core-0.4.0b8/digitalhub_core/stores/objects/sql.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:36:05.001934 digitalhub_core-0.4.0b8/digitalhub_core/utils/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b8/digitalhub_core/utils/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3646 2024-03-12 14:23:02.000000 digitalhub_core-0.4.0b8/digitalhub_core/utils/api.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2215 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/utils/env_utils.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      346 2023-12-11 08:31:30.000000 digitalhub_core-0.4.0b8/digitalhub_core/utils/exceptions.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1332 2024-04-08 14:07:02.000000 digitalhub_core-0.4.0b8/digitalhub_core/utils/file_utils.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4237 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/utils/generic_utils.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3054 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/utils/git_utils.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1794 2024-02-01 10:08:51.000000 digitalhub_core-0.4.0b8/digitalhub_core/utils/io_utils.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      460 2023-11-21 13:33:17.000000 digitalhub_core-0.4.0b8/digitalhub_core/utils/logger.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      805 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/utils/uri_utils.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:36:05.001934 digitalhub_core-0.4.0b8/digitalhub_core.egg-info/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)    15054 2024-05-14 10:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core.egg-info/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4165 2024-05-14 10:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-05-14 10:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      250 2024-05-14 10:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core.egg-info/requires.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-05-14 10:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core.egg-info/top_level.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1731 2024-05-13 12:41:00.000000 digitalhub_core-0.4.0b8/pyproject.toml
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-05-14 10:36:05.005934 digitalhub_core-0.4.0b8/setup.cfg
```

### Comparing `digitalhub_core-0.4.0b4/LICENSE.txt` & `digitalhub_core-0.4.0b8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b4/PKG-INFO` & `digitalhub_core-0.4.0b8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalhub-core
-Version: 0.4.0b4
+Version: 0.4.0b8
 Summary: Python SDK for DHCore
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 License:                               Apache License
                                 Version 2.0, January 2004
                              http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/__init__.py` & `digitalhub_core-0.4.0b8/digitalhub_core/__init__.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/client/builder.py` & `digitalhub_core-0.4.0b8/digitalhub_core/client/builder.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/client/objects/base.py` & `digitalhub_core-0.4.0b8/digitalhub_core/client/objects/base.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/client/objects/dhcore.py` & `digitalhub_core-0.4.0b8/digitalhub_core/client/objects/dhcore.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/client/objects/local.py` & `digitalhub_core-0.4.0b8/digitalhub_core/client/objects/local.py`

 * *Files 6% similar despite different names*

```diff
@@ -310,16 +310,33 @@
 
         # Name is optional and extracted from kwargs
         # "params": {"name": <name>}
         name = kwargs.get("params", {}).get("name")
         if name is not None:
             return [self._db[entity_type][name]["latest"]]
 
-        # If no name is provided, return objects by entity_type
-        return [v["latest"] for _, v in self._db[entity_type].items()]
+        try:
+            # If no name is provided, get latest objects
+            listed_objects = [v["latest"] for _, v in self._db[entity_type].items()]
+        except KeyError:
+            listed_objects = []
+
+        # If kind is provided, return objects by kind
+        kind = kwargs.get("params", {}).get("kind")
+        if kind is not None:
+            listed_objects = [obj for obj in listed_objects if obj["kind"] == kind]
+
+        # If function is provided, return objects by function
+        spec_params = ["function", "task"]
+        for i in spec_params:
+            p = kwargs.get("params", {}).get(i)
+            if p is not None:
+                listed_objects = [obj for obj in listed_objects if obj["spec"][i] == p]
+
+        return listed_objects
 
     ########################
     # Helpers
     ########################
 
     def _parse_api(self, api: str) -> tuple:
         """
```

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/context/builder.py` & `digitalhub_core-0.4.0b8/digitalhub_core/context/builder.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/context/context.py` & `digitalhub_core-0.4.0b8/digitalhub_core/context/context.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/entities/_base/base.py` & `digitalhub_core-0.4.0b8/digitalhub_core/entities/_base/base.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/entities/_base/entity.py` & `digitalhub_core-0.4.0b8/digitalhub_core/entities/_base/entity.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/entities/_base/metadata.py` & `digitalhub_core-0.4.0b8/digitalhub_core/entities/_base/metadata.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/entities/_base/spec.py` & `digitalhub_core-0.4.0b8/digitalhub_core/entities/_base/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/entities/_base/status.py` & `digitalhub_core-0.4.0b8/digitalhub_core/entities/_base/status.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/entities/_builders/metadata.py` & `digitalhub_core-0.4.0b8/digitalhub_core/entities/_builders/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 Metadata factory entity.
 """
 from __future__ import annotations
 
 import typing
 
-from digitalhub_core.registry.import_utils import import_class
 from digitalhub_core.registry.registry import registry
+from digitalhub_core.registry.utils import import_class
 from digitalhub_core.utils.generic_utils import get_timestamp
 
 if typing.TYPE_CHECKING:
     from digitalhub_core.entities._base.metadata import Metadata
     from digitalhub_core.registry.models import RegistryEntry
```

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/entities/_builders/spec.py` & `digitalhub_core-0.4.0b8/digitalhub_core/entities/_builders/spec.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 Spec factory entity.
 """
 from __future__ import annotations
 
 import typing
 
-from digitalhub_core.registry.import_utils import import_class
 from digitalhub_core.registry.registry import registry
+from digitalhub_core.registry.utils import import_class
 
 if typing.TYPE_CHECKING:
     from digitalhub_core.entities._base.spec import Spec
     from digitalhub_core.registry.models import RegistryEntry
 
 
 def build_spec(kind: str, validate: bool = True, **kwargs) -> Spec:
```

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/entities/_builders/status.py` & `digitalhub_core-0.4.0b8/digitalhub_core/entities/_builders/status.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 Status factory entity.
 """
 from __future__ import annotations
 
 import typing
 
 from digitalhub_core.entities._base.status import State
-from digitalhub_core.registry.import_utils import import_class
 from digitalhub_core.registry.registry import registry
+from digitalhub_core.registry.utils import import_class
 
 if typing.TYPE_CHECKING:
     from digitalhub_core.entities._base.status import Status
     from digitalhub_core.registry.models import RegistryEntry
 
 
 def build_status(kind: str, **kwargs) -> Status:
```

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/entities/artifacts/crud.py` & `digitalhub_core-0.4.0b8/digitalhub_core/entities/artifacts/crud.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 """
 from __future__ import annotations
 
 import typing
 
 from digitalhub_core.context.builder import check_context, get_context
 from digitalhub_core.entities.artifacts.entity import artifact_from_dict, artifact_from_parameters
+from digitalhub_core.entities.entity_types import EntityTypes
 from digitalhub_core.utils.api import api_ctx_delete, api_ctx_list, api_ctx_read, api_ctx_update
 from digitalhub_core.utils.generic_utils import parse_entity_key
 from digitalhub_core.utils.io_utils import read_yaml
 
 if typing.TYPE_CHECKING:
     from digitalhub_core.entities.artifacts.entity import Artifact
 
 
-ENTITY_TYPE = "artifacts"
+ENTITY_TYPE = EntityTypes.ARTIFACTS.value
 
 
 def create_artifact(**kwargs) -> Artifact:
     """
     Create a new artifact with the provided parameters.
 
     Parameters
```

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/entities/artifacts/entity.py` & `digitalhub_core-0.4.0b8/digitalhub_core/entities/artifacts/entity.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from urllib.parse import urlparse
 
 from digitalhub_core.context.builder import get_context
 from digitalhub_core.entities._base.entity import Entity
 from digitalhub_core.entities._builders.metadata import build_metadata
 from digitalhub_core.entities._builders.spec import build_spec
 from digitalhub_core.entities._builders.status import build_status
+from digitalhub_core.entities.entity_types import EntityTypes
 from digitalhub_core.stores.builder import get_store
 from digitalhub_core.utils.api import api_ctx_create, api_ctx_read, api_ctx_update
 from digitalhub_core.utils.exceptions import EntityError
 from digitalhub_core.utils.generic_utils import build_uuid, get_timestamp
 from digitalhub_core.utils.io_utils import write_yaml
 from digitalhub_core.utils.uri_utils import map_uri_scheme
 
@@ -31,14 +32,16 @@
     A class representing a artifact.
 
     Artifacts are (binary) objects stored in one of the artifact
     stores of the platform, and available to every process, module
     and component as files.
     """
 
+    ENTITY_TYPE = EntityTypes.ARTIFACTS.value
+
     def __init__(
         self,
         project: str,
         name: str,
         uuid: str,
         kind: str,
         metadata: ArtifactMetadata,
@@ -69,15 +72,15 @@
             Owner of the object.
         """
         super().__init__()
         self.project = project
         self.name = name
         self.id = uuid
         self.kind = kind
-        self.key = f"store://{project}/artifacts/{kind}/{name}:{uuid}"
+        self.key = f"store://{project}/{self.ENTITY_TYPE}/{kind}/{name}:{uuid}"
         self.metadata = metadata
         self.spec = spec
         self.status = status
         self.user = user
 
         # Add attributes to be used in the to_dict method
         self._obj_attr.extend(["project", "name", "id", "key"])
@@ -99,35 +102,35 @@
         -------
         Artifact
             Entity saved.
         """
         obj = self.to_dict()
 
         if not update:
-            api = api_ctx_create(self.project, "artifacts")
+            api = api_ctx_create(self.project, self.ENTITY_TYPE)
             new_obj = self._context().create_object(api, obj)
             self._update_attributes(new_obj)
             return self
 
         self.metadata.updated = obj["metadata"]["updated"] = get_timestamp()
-        api = api_ctx_update(self.project, "artifacts", self.id)
+        api = api_ctx_update(self.project, self.ENTITY_TYPE, self.id)
         new_obj = self._context().update_object(api, obj)
         self._update_attributes(new_obj)
         return self
 
     def refresh(self) -> Artifact:
         """
         Refresh object from backend.
 
         Returns
         -------
         Artifact
             Entity refreshed.
         """
-        api = api_ctx_read(self.project, "artifacts", self.id)
+        api = api_ctx_read(self.project, self.ENTITY_TYPE, self.id)
         obj = self._context().read_object(api)
         self._update_attributes(obj)
         return self
 
     def export(self, filename: str | None = None) -> None:
         """
         Export object as a YAML file.
```

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/entities/artifacts/spec.py` & `digitalhub_core-0.4.0b8/digitalhub_core/entities/artifacts/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/entities/functions/crud.py` & `digitalhub_core-0.4.0b8/digitalhub_core/entities/functions/crud.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 Module for performing operations on functions.
 """
 from __future__ import annotations
 
 import typing
 
 from digitalhub_core.context.builder import check_context, get_context
+from digitalhub_core.entities.entity_types import EntityTypes
 from digitalhub_core.entities.functions.entity import function_from_dict, function_from_parameters
 from digitalhub_core.utils.api import api_ctx_delete, api_ctx_list, api_ctx_read, api_ctx_update
 from digitalhub_core.utils.io_utils import read_yaml
 
 if typing.TYPE_CHECKING:
     from digitalhub_core.entities.functions.entity import Function
 
-ENTITY_TYPE = "functions"
+ENTITY_TYPE = EntityTypes.FUNCTIONS.value
 
 
 def create_function(**kwargs) -> Function:
     """
     Create a new object instance.
 
     Parameters
```

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/entities/functions/entity.py` & `digitalhub_core-0.4.0b8/digitalhub_core/entities/functions/entity.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 from pathlib import Path
 
 from digitalhub_core.context.builder import get_context
 from digitalhub_core.entities._base.entity import Entity
 from digitalhub_core.entities._builders.metadata import build_metadata
 from digitalhub_core.entities._builders.spec import build_spec
 from digitalhub_core.entities._builders.status import build_status
-from digitalhub_core.entities.tasks.crud import create_task, create_task_from_dict, delete_task, new_task
+from digitalhub_core.entities.entity_types import EntityTypes
+from digitalhub_core.entities.tasks.crud import create_task, create_task_from_dict, delete_task
 from digitalhub_core.utils.api import api_ctx_create, api_ctx_list, api_ctx_read, api_ctx_update
 from digitalhub_core.utils.exceptions import BackendError, EntityError
 from digitalhub_core.utils.generic_utils import build_uuid, get_timestamp
 from digitalhub_core.utils.io_utils import write_yaml
 
 if typing.TYPE_CHECKING:
     from digitalhub_core.context.context import Context
@@ -28,14 +29,16 @@
 
 
 class Function(Entity):
     """
     A class representing a function.
     """
 
+    ENTITY_TYPE = EntityTypes.FUNCTIONS.value
+
     def __init__(
         self,
         project: str,
         name: str,
         uuid: str,
         kind: str,
         metadata: FunctionMetadata,
@@ -66,15 +69,15 @@
             Owner of the object.
         """
         super().__init__()
         self.project = project
         self.name = name
         self.id = uuid
         self.kind = kind
-        self.key = f"store://{project}/functions/{kind}/{name}:{uuid}"
+        self.key = f"store://{project}/{self.ENTITY_TYPE}/{kind}/{name}:{uuid}"
         self.metadata = metadata
         self.spec = spec
         self.status = status
         self.user = user
 
         # Add attributes to be used in the to_dict method
         self._obj_attr.extend(["project", "name", "id", "key"])
@@ -99,35 +102,35 @@
         -------
         Function
             Entity saved.
         """
         obj = self.to_dict(include_all_non_private=True)
 
         if not update:
-            api = api_ctx_create(self.project, "functions")
+            api = api_ctx_create(self.project, self.ENTITY_TYPE)
             new_obj = self._context().create_object(api, obj)
             self._update_attributes(new_obj)
             return self
 
         self.metadata.updated = obj["metadata"]["updated"] = get_timestamp()
-        api = api_ctx_update(self.project, "functions", self.id)
+        api = api_ctx_update(self.project, self.ENTITY_TYPE, self.id)
         new_obj = self._context().update_object(api, obj)
         self._update_attributes(new_obj)
         return self
 
     def refresh(self) -> Function:
         """
         Refresh object from backend.
 
         Returns
         -------
         Function
             Entity refreshed.
         """
-        api = api_ctx_read(self.project, "functions", self.id)
+        api = api_ctx_read(self.project, self.ENTITY_TYPE, self.id)
         obj = self._context().read_object(api)
         self._update_attributes(obj)
         return self
 
     def export(self, filename: str | None = None) -> None:
         """
         Export object as a YAML file.
@@ -182,16 +185,16 @@
         affinity: dict | None = None,
         tolerations: list[dict] | None = None,
         env: list[dict] | None = None,
         secrets: list[str] | None = None,
         backoff_limit: int | None = None,
         schedule: str | None = None,
         replicas: int | None = None,
-        inputs: list | None = None,
-        outputs: list | None = None,
+        inputs: dict | None = None,
+        outputs: dict | None = None,
         parameters: dict | None = None,
         values: list | None = None,
         local_execution: bool = False,
         **kwargs,
     ) -> Run:
         """
         Run function. This method creates a new run and executes it.
@@ -216,17 +219,17 @@
             The secrets of the task. Task parameter.
         backoff_limit : int
             The backoff limit of the task. Task parameter.
         schedule : str
             The schedule of the task. Task parameter.
         replicas : int
             The replicas of the task. Task parameter.
-        inputs : list
+        inputs : dict
             Function inputs. Run parameter.
-        outputs : list
+        outputs : dict
             Function outputs. Run parameter.
         parameters : dict
             Function parameters. Run parameter.
         values : list
             Function values. Run parameter.
         local_execution : bool
             Flag to determine if object has local execution. Run parameter.
@@ -234,38 +237,29 @@
             Keyword arguments passed to Task builder.
 
         Returns
         -------
         Run
             Run instance.
         """
-
-        # Create task if does not exists
-        task = self._tasks.get(action)
-
-        # Check in backend
-        if task is None and not self._context().local:
-            task = self._check_task_in_backend(action)
-
-        # Create new task
-        if task is None:
-            task = self.new_task(
-                kind=f"{self.kind}+{action}",
-                node_selector=node_selector,
-                volumes=volumes,
-                resources=resources,
-                affinity=affinity,
-                tolerations=tolerations,
-                env=env,
-                secrets=secrets,
-                backoff_limit=backoff_limit,
-                schedule=schedule,
-                replicas=replicas,
-                **kwargs,
-            )
+        # Create or update new task
+        task = self.new_task(
+            kind=f"{self.kind}+{action}",
+            node_selector=node_selector,
+            volumes=volumes,
+            resources=resources,
+            affinity=affinity,
+            tolerations=tolerations,
+            env=env,
+            secrets=secrets,
+            backoff_limit=backoff_limit,
+            schedule=schedule,
+            replicas=replicas,
+            **kwargs,
+        )
 
         # Run function from task
         run = task.run(inputs, outputs, parameters, values, local_execution)
 
         # If execution is done by DHCore backend, return the object
         if not local_execution:
             if self._context().local:
@@ -275,35 +269,14 @@
         # If local execution, build and launch run.
         # Detach the run from the main thread
         run.build()
         with ThreadPoolExecutor(max_workers=1) as executor:
             result = executor.submit(run.run)
         return result.result()
 
-    def _check_task_in_backend(self, action: str) -> None | Task:
-        """
-        Check if task exists in backend.
-
-        Parameters
-        ----------
-        action : str
-            Action to check.
-
-        Returns
-        -------
-        None | Task
-            Task if exists, None otherwise.
-        """
-        api = api_ctx_list(self.project, "tasks")
-        params = {"function": self._get_function_string(), "kind": f"{self.kind}+{action}"}
-        objs = self._context().list_objects(api, params=params)
-        for i in objs:
-            self._tasks[action] = create_task_from_dict(i)
-            return self._tasks[action]
-
     def _get_function_string(self) -> str:
         """
         Get function string.
 
         Returns
         -------
         str
@@ -364,18 +337,31 @@
             Keyword arguments.
 
         Returns
         -------
         Task
             New task.
         """
+        # Override kwargs
         kwargs["project"] = self.project
         kwargs["function"] = self._get_function_string()
         kwargs["kind"] = kwargs["kind"]
-        task = new_task(**kwargs)
+
+        # Create object instance
+        task = create_task(**kwargs)
+
+        exists, task_id = self._check_task_in_backend(kwargs["kind"])
+
+        # Save or update task
+        if not exists:
+            task.save()
+        else:
+            task.id = task_id
+            task.save(update=True)
+
         self._tasks[kwargs["kind"]] = task
         return task
 
     def update_task(self, kind: str, **kwargs) -> None:
         """
         Update task.
 
@@ -447,17 +433,40 @@
 
         Raises
         ------
         EntityError
             If task is not created.
         """
         self._raise_if_not_exists(kind)
-        delete_task(self.project, self._tasks[kind].name, cascade=cascade)
+        delete_task(self.project, entity_id=self._tasks[kind].id, cascade=cascade)
         self._tasks.pop(kind, None)
 
+    def _check_task_in_backend(self, kind: str) -> tuple[bool, str | None]:
+        """
+        Check if task exists in backend.
+
+        Parameters
+        ----------
+        kind : str
+            Kind of the task.
+
+        Returns
+        -------
+        tuple[bool, str | None]
+            Flag to determine if task exists in backend and ID if exists.
+        """
+        # List tasks from backend filtered by function and kind
+        api = api_ctx_list(self.project, EntityTypes.TASKS.value)
+        params = {"function": self._get_function_string(), "kind": kind}
+        objs = self._context().list_objects(api, params=params)
+        try:
+            return True, objs[0]["id"]
+        except IndexError:
+            return False, None
+
     def _raise_if_not_exists(self, kind: str) -> None:
         """
         Raise error if task is not created.
 
         Parameters
         ----------
         kind : str
```

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/entities/functions/spec.py` & `digitalhub_core-0.4.0b8/digitalhub_core/entities/functions/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/entities/projects/crud.py` & `digitalhub_core-0.4.0b8/digitalhub_core/entities/projects/crud.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,24 +5,25 @@
 
 import importlib.util as imputil
 import typing
 from pathlib import Path
 
 from digitalhub_core.client.builder import build_client, get_client
 from digitalhub_core.context.builder import delete_context
+from digitalhub_core.entities.entity_types import EntityTypes
 from digitalhub_core.entities.projects.entity import project_from_dict, project_from_parameters
 from digitalhub_core.utils.api import api_base_delete, api_base_read, api_base_update
 from digitalhub_core.utils.exceptions import BackendError, EntityError
 from digitalhub_core.utils.io_utils import read_yaml
 
 if typing.TYPE_CHECKING:
     from digitalhub_core.entities.projects.entity import Project
 
 
-ENTITY_TYPE = "projects"
+ENTITY_TYPE = EntityTypes.PROJECTS.value
 
 
 def create_project(**kwargs) -> Project:
     """
     Create a new project.
 
     Parameters
```

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/entities/projects/entity.py` & `digitalhub_core-0.4.0b8/digitalhub_core/entities/projects/entity.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from digitalhub_core.entities.artifacts.crud import (
     create_artifact_from_dict,
     delete_artifact,
     get_artifact,
     list_artifacts,
     new_artifact,
 )
+from digitalhub_core.entities.entity_types import EntityTypes
 from digitalhub_core.entities.functions.crud import (
     create_function_from_dict,
     delete_function,
     get_function,
     list_functions,
     new_function,
 )
@@ -51,28 +52,40 @@
     from digitalhub_core.entities.projects.metadata import ProjectMetadata
     from digitalhub_core.entities.projects.spec import ProjectSpec
     from digitalhub_core.entities.projects.status import ProjectStatus
     from digitalhub_core.entities.secrets.entity import Secret
     from digitalhub_core.entities.workflows.entity import Workflow
 
 
-CTX_ENTITIES = ["artifacts", "functions", "workflows", "secrets"]
+ARTIFACTS = EntityTypes.ARTIFACTS.value
+FUNCTIONS = EntityTypes.FUNCTIONS.value
+WORKFLOWS = EntityTypes.WORKFLOWS.value
+SECRETS = EntityTypes.SECRETS.value
+
+CTX_ENTITIES = [
+    ARTIFACTS,
+    FUNCTIONS,
+    WORKFLOWS,
+    SECRETS,
+]
 FUNC_MAP = {
-    "artifacts": create_artifact_from_dict,
-    "functions": create_function_from_dict,
-    "workflows": create_workflow_from_dict,
-    "secrets": create_secret_from_dict,
+    ARTIFACTS: create_artifact_from_dict,
+    FUNCTIONS: create_function_from_dict,
+    WORKFLOWS: create_workflow_from_dict,
+    SECRETS: create_secret_from_dict,
 }
 
 
 class Project(Entity):
     """
     A class representing a project.
     """
 
+    ENTITY_TYPE = EntityTypes.PROJECTS.value
+
     def __init__(
         self,
         name: str,
         kind: str,
         metadata: ProjectMetadata,
         spec: ProjectSpec,
         status: ProjectStatus,
@@ -96,24 +109,25 @@
             Status of the object.
         user : str
             Owner of the object.
         local: bool
             If True, export locally.
         """
         super().__init__()
+        self.id = name
         self.name = name
         self.kind = kind
         self.key = f"store://{name}"
         self.metadata = metadata
         self.spec = spec
         self.status = status
         self.user = user
 
         # Add attributes to be used in the to_dict method
-        self._obj_attr.extend(["name", "key"])
+        self._obj_attr.extend(["id", "name", "key"])
 
         # Set client
         self._client = get_client(local)
 
         # Set context
         set_context(self)
 
@@ -134,37 +148,37 @@
         -------
         Project
             Entity saved.
         """
         obj = self._refresh_to_dict()
 
         if not update:
-            api = api_base_create("projects")
+            api = api_base_create(self.ENTITY_TYPE)
             new_obj = self._client.create_object(api, obj)
             new_obj["local"] = self._client.is_local()
             self._update_attributes(new_obj)
             return self
 
         self.metadata.updated = obj["metadata"]["updated"] = get_timestamp()
-        api = api_base_update("projects", self.id)
+        api = api_base_update(self.ENTITY_TYPE, self.id)
         new_obj = self._client.update_object(api, obj)
         new_obj["local"] = self._client.is_local()
         self._update_attributes(new_obj)
         return self
 
     def refresh(self) -> Project:
         """
         Refresh object from backend.
 
         Returns
         -------
         Project
             Project object.
         """
-        api = api_base_read("projects", self.name)
+        api = api_base_read(self.ENTITY_TYPE, self.name)
         obj = self._client.read_object(api)
         self._update_attributes(obj)
         return self
 
     def export(self, filename: str | None = None) -> None:
         """
         Export object as a YAML file. If the objects are not embedded, the objects are
@@ -338,15 +352,15 @@
         -------
         Artifact
            Object instance.
         """
         kwargs["project"] = self.name
         kwargs["kind"] = "artifact"
         obj = new_artifact(**kwargs)
-        self._add_object(obj, "artifacts")
+        self._add_object(obj, ARTIFACTS)
         return obj
 
     def get_artifact(self, entity_name: str | None = None, entity_id: str | None = None, **kwargs) -> Artifact:
         """
         Get object from backend.
 
         Parameters
@@ -360,15 +374,15 @@
 
         Returns
         -------
         Artifact
             Instance of Artifact class.
         """
         obj = get_artifact(self.name, entity_name=entity_name, entity_id=entity_id, **kwargs)
-        self._add_object(obj, "artifacts")
+        self._add_object(obj, ARTIFACTS)
         return obj
 
     def delete_artifact(self, entity_name: str | None = None, entity_id: str | None = None, **kwargs) -> None:
         """
         Delete a Artifact from project.
 
         Parameters
@@ -381,30 +395,30 @@
             Parameters to pass to the API call.
 
         Returns
         -------
         None
         """
         delete_artifact(self.name, entity_name=entity_name, entity_id=entity_id, **kwargs)
-        self._delete_object("artifacts", entity_name, entity_id)
+        self._delete_object(ARTIFACTS, entity_name, entity_id)
 
     def set_artifact(self, artifact: Artifact) -> None:
         """
         Set a Artifact.
 
         Parameters
         ----------
         artifact : Artifact
             Artifact to set.
 
         Returns
         -------
         None
         """
-        self._add_object(artifact, "artifacts")
+        self._add_object(artifact, ARTIFACTS)
 
     def list_artifacts(self, **kwargs) -> list[dict]:
         """
         List artifacts associated with the project.
 
         Parameters
         ----------
@@ -434,15 +448,15 @@
         Returns
         -------
         Function
            Object instance.
         """
         kwargs["project"] = self.name
         obj = new_function(**kwargs)
-        self._add_object(obj, "functions")
+        self._add_object(obj, FUNCTIONS)
         return obj
 
     def get_function(self, entity_name: str | None = None, entity_id: str | None = None, **kwargs) -> Function:
         """
         Get object from backend.
 
         Parameters
@@ -456,15 +470,15 @@
 
         Returns
         -------
         Function
             Instance of Function class.
         """
         obj = get_function(self.name, entity_name=entity_name, entity_id=entity_id, **kwargs)
-        self._add_object(obj, "functions")
+        self._add_object(obj, FUNCTIONS)
         return obj
 
     def delete_function(self, entity_name: str | None = None, entity_id: str | None = None, **kwargs) -> None:
         """
         Delete a Function from project.
 
         Parameters
@@ -477,30 +491,30 @@
             Parameters to pass to the API call.
 
         Returns
         -------
         None
         """
         delete_function(self.name, entity_name=entity_name, entity_id=entity_id, **kwargs)
-        self._delete_object("functions", entity_name, entity_id)
+        self._delete_object(FUNCTIONS, entity_name, entity_id)
 
     def set_function(self, function: Function) -> None:
         """
         Set a Function.
 
         Parameters
         ----------
         function : Function
             Function to set.
 
         Returns
         -------
         None
         """
-        self._add_object(function, "functions")
+        self._add_object(function, FUNCTIONS)
 
     def list_functions(self, **kwargs) -> list[dict]:
         """
         List functions associated with the project.
 
         Parameters
         ----------
@@ -530,15 +544,15 @@
         Returns
         -------
         Workflow
             An instance of the created workflow.
         """
         kwargs["project"] = self.name
         obj = new_workflow(**kwargs)
-        self._add_object(obj, "workflows")
+        self._add_object(obj, WORKFLOWS)
         return obj
 
     def get_workflow(self, entity_name: str | None = None, entity_id: str | None = None, **kwargs) -> Workflow:
         """
         Get object from backend.
 
         Parameters
@@ -552,15 +566,15 @@
 
         Returns
         -------
         Workflow
             Instance of Workflow class.
         """
         obj = get_workflow(self.name, entity_name=entity_name, entity_id=entity_id, **kwargs)
-        self._add_object(obj, "workflows")
+        self._add_object(obj, WORKFLOWS)
         return obj
 
     def delete_workflow(self, entity_name: str | None = None, entity_id: str | None = None, **kwargs) -> None:
         """
         Delete a Workflow from project.
 
         Parameters
@@ -573,30 +587,30 @@
             Parameters to pass to the API call.
 
         Returns
         -------
         None
         """
         delete_workflow(self.name, entity_name=entity_name, entity_id=entity_id, **kwargs)
-        self._delete_object("workflows", entity_name, entity_id)
+        self._delete_object(WORKFLOWS, entity_name, entity_id)
 
     def set_workflow(self, workflow: Workflow) -> None:
         """
         Set a Workflow.
 
         Parameters
         ----------
         workflow : Workflow
             Workflow to set.
 
         Returns
         -------
         None
         """
-        self._add_object(workflow, "workflows")
+        self._add_object(workflow, WORKFLOWS)
 
     def list_workflows(self, **kwargs) -> list[dict]:
         """
         List workflows associated with the project.
 
         Parameters
         ----------
@@ -626,15 +640,15 @@
         Returns
         -------
         Secret
             An instance of the created secret.
         """
         kwargs["project"] = self.name
         obj = new_secret(**kwargs)
-        self._add_object(obj, "secrets")
+        self._add_object(obj, SECRETS)
         return obj
 
     def get_secret(self, entity_name: str | None = None, entity_id: str | None = None, **kwargs) -> Secret:
         """
         Get object from backend.
 
         Parameters
@@ -648,15 +662,15 @@
 
         Returns
         -------
         Secret
             Instance of Secret class.
         """
         obj = get_secret(self.name, entity_name=entity_name, entity_id=entity_id, **kwargs)
-        self._add_object(obj, "secrets")
+        self._add_object(obj, SECRETS)
         return obj
 
     def delete_secret(self, entity_name: str | None = None, entity_id: str | None = None, **kwargs) -> None:
         """
         Delete a Secret from project.
 
         Parameters
@@ -669,30 +683,30 @@
             Parameters to pass to the API call.
 
         Returns
         -------
         None
         """
         delete_secret(self.name, entity_name=entity_name, entity_id=entity_id, **kwargs)
-        self._delete_object("secrets", entity_name, entity_id)
+        self._delete_object(SECRETS, entity_name, entity_id)
 
     def set_secret(self, secret: Secret) -> None:
         """
         Set a Secret.
 
         Parameters
         ----------
         secret : Secret
             Secret to set.
 
         Returns
         -------
         None
         """
-        self._add_object(secret, "secrets")
+        self._add_object(secret, SECRETS)
 
     def list_secrets(self, **kwargs) -> list[dict]:
         """
         List secrets associated with the project.
 
         Parameters
         ----------
```

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/entities/projects/spec.py` & `digitalhub_core-0.4.0b8/digitalhub_core/entities/projects/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/entities/runs/crud.py` & `digitalhub_core-0.4.0b8/digitalhub_core/entities/runs/crud.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 Module for performing operations on runs.
 """
 from __future__ import annotations
 
 import typing
 
 from digitalhub_core.context.builder import check_context, get_context
+from digitalhub_core.entities.entity_types import EntityTypes
 from digitalhub_core.entities.runs.entity import run_from_dict, run_from_parameters
 from digitalhub_core.utils.api import api_ctx_delete, api_ctx_list, api_ctx_read, api_ctx_update
 from digitalhub_core.utils.io_utils import read_yaml
 
 if typing.TYPE_CHECKING:
     from digitalhub_core.entities.runs.entity import Run
 
 
-ENTITY_TYPE = "runs"
+ENTITY_TYPE = EntityTypes.RUNS.value
 
 
 def create_run(**kwargs) -> Run:
     """
     Create a new object instance.
 
     Parameters
@@ -79,17 +80,17 @@
         Kind of the object.
     uuid : str
         ID of the object in form of UUID.
     source : str
         Remote git source for object.
     labels : list[str]
         List of labels.
-    inputs : list
+    inputs : dict
         Inputs of the run.
-    outputs : list
+    outputs : dict
         Outputs of the run.
     parameters : dict
         Parameters of the run.
     values : list
         Values of the run.
     local_execution : bool
         Flag to determine if object has local execution.
```

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/entities/runs/entity.py` & `digitalhub_core-0.4.0b8/digitalhub_core/entities/runs/entity.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 from digitalhub_core.context.builder import get_context
 from digitalhub_core.entities._base.entity import Entity
 from digitalhub_core.entities._base.status import State
 from digitalhub_core.entities._builders.metadata import build_metadata
 from digitalhub_core.entities._builders.spec import build_spec
 from digitalhub_core.entities._builders.status import build_status
+from digitalhub_core.entities.entity_types import EntityTypes
 from digitalhub_core.registry.registry import registry
 from digitalhub_core.runtimes.builder import build_runtime
 from digitalhub_core.utils.api import api_base_list, api_ctx_create, api_ctx_list, api_ctx_read, api_ctx_update
 from digitalhub_core.utils.exceptions import EntityError
 from digitalhub_core.utils.generic_utils import build_uuid, get_timestamp
 from digitalhub_core.utils.io_utils import write_yaml
 
@@ -35,14 +36,16 @@
 
 
 class Run(Entity):
     """
     A class representing a run.
     """
 
+    ENTITY_TYPE = EntityTypes.RUNS.value
+
     def __init__(
         self,
         project: str,
         uuid: str,
         kind: str,
         metadata: RunMetadata,
         spec: RunSpec,
@@ -69,15 +72,15 @@
         user : str
             Owner of the object.
         """
         super().__init__()
         self.project = project
         self.id = uuid
         self.kind = kind
-        self.key = f"store://{project}/runs/{kind}/{uuid}"
+        self.key = f"store://{project}/{self.ENTITY_TYPE}/{kind}/{uuid}"
         self.metadata = metadata
         self.spec = spec
         self.status = status
         self.user = user
 
         # Add attributes to be used in the to_dict method
         self._obj_attr.extend(["project", "id", "key"])
@@ -99,21 +102,21 @@
         -------
         Run
             Entity saved.
         """
         obj = self.to_dict(include_all_non_private=True)
 
         if not update:
-            api = api_ctx_create(self.project, "runs")
+            api = api_ctx_create(self.project, self.ENTITY_TYPE)
             new_obj = self._context().create_object(api, obj)
             self._update_attributes(new_obj)
             return self
 
         self.metadata.updated = obj["metadata"]["updated"] = get_timestamp()
-        api = api_ctx_update(self.project, "runs", self.id)
+        api = api_ctx_update(self.project, self.ENTITY_TYPE, self.id)
         new_obj = self._context().update_object(api, obj)
         self._update_attributes(new_obj)
         return self
 
     def export(self, filename: str | None = None) -> None:
         """
         Export object as a YAML file.
@@ -241,21 +244,21 @@
         Returns
         -------
         list
             List of output objects.
         """
         return self.status.get_outputs(as_key=as_key, as_dict=as_dict)
 
-    def values(self) -> list:
+    def values(self) -> dict:
         """
         Get values from runtime execution.
 
         Returns
         -------
-        list
+        dict
             Values from backend.
         """
         value_list = getattr(self.spec, "values", [])
         value_list = value_list if value_list is not None else []
         return self.status.get_values(value_list)
 
     def refresh(self) -> Run:
@@ -263,15 +266,15 @@
         Refresh object from backend.
 
         Returns
         -------
         Run
             Run object.
         """
-        api = api_ctx_read(self.project, "runs", self.id)
+        api = api_ctx_read(self.project, self.ENTITY_TYPE, self.id)
         obj = self._context().read_object(api)
         self._update_attributes(obj)
         return self
 
     def logs(self) -> dict:
         """
         Get object from backend.
@@ -280,29 +283,29 @@
         Returns
         -------
         dict
             Logs from backend.
         """
         if self._context().local:
             return {}
-        api = api_ctx_read(self.project, "runs", self.id) + "/log"
+        api = api_ctx_read(self.project, self.ENTITY_TYPE, self.id) + "/log"
         return self._context().read_object(api)
 
     def stop(self) -> None:
         """
         Stop run.
 
         Returns
         -------
         None
         """
         # Do nothing if context is local
         if self._context().local:
             return
-        api = api_ctx_create(self.project, "runs") + f"/{self.id}/stop"
+        api = api_ctx_create(self.project, self.ENTITY_TYPE) + f"/{self.id}/stop"
         self._context().create_object(api)
         self.status.state = State.STOPPED.value
 
     def _set_status(self, status: dict) -> None:
         """
         Set run status.
 
@@ -464,17 +467,17 @@
         Kind of the object.
     uuid : str
         ID of the object in form of UUID.
     source : str
         Remote git source for object.
     labels : list[str]
         List of labels.
-    inputs : list
+    inputs : dict
         Inputs of the run.
-    outputs : list
+    outputs : dict
         Outputs of the run.
     parameters : dict
         Parameters of the run.
     values : list
         Values of the run.
     local_execution : bool
         Flag to determine if object has local execution.
```

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/entities/runs/spec.py` & `digitalhub_core-0.4.0b8/digitalhub_core/entities/runs/spec.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 
 class RunSpec(Spec):
     """Run specification."""
 
     def __init__(
         self,
         task: str,
-        inputs: list | None = None,
-        outputs: list | None = None,
+        inputs: dict | None = None,
+        outputs: dict | None = None,
         parameters: dict | None = None,
         values: list | None = None,
         local_execution: bool = False,
     ) -> None:
         """
         Constructor.
         """
@@ -46,33 +46,32 @@
         Get inputs.
 
         Returns
         -------
         list[dict[str, Entity]]
             The inputs.
         """
-        inputs = []
+        inputs = {}
         if self.inputs is None:
             return inputs
 
-        for i in self.inputs:
-            for parameter, item in i.items():
-                parameter_type = self._parse_parameter(parameter)
-
-                # Get entity from key
-                if parameter_type == "key":
-                    key = self._collect_key(item)
-                    entity = self._collect_entity(key)
-                    if as_dict:
-                        entity = entity.to_dict()
-                    inputs.append({parameter: entity})
-
-                # Create entity from parameter
-                elif parameter_type == "create":
-                    raise NotImplementedError
+        for parameter, item in self.inputs.items():
+            parameter_type = self._parse_parameter(parameter)
+
+            # Get entity from key
+            if parameter_type == "key":
+                key = self._collect_key(item)
+                entity = self._collect_entity(key)
+                if as_dict:
+                    entity = entity.to_dict()
+                inputs[parameter] = entity
+
+            # Create entity from parameter
+            elif parameter_type == "create":
+                raise NotImplementedError
 
         return inputs
 
     @staticmethod
     def _parse_parameter(parameter: str) -> str:
         """
         Parse parameter.
@@ -133,18 +132,18 @@
     """
     Run parameters.
     """
 
     task: str = None
     """The task string associated with the run."""
 
-    inputs: list[dict[str, Union[str, dict]]] = None
+    inputs: dict[str, Union[str, dict]] = None
     """Run inputs."""
 
-    outputs: list[dict[str, Union[str, dict]]] = None
+    outputs: dict[str, Union[str, dict]] = None
     """Run outputs."""
 
     parameters: dict = None
     """Parameters to be used in the run."""
 
     values: list = None
     """Values to be used in the run."""
```

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/entities/runs/status.py` & `digitalhub_core-0.4.0b8/digitalhub_core/entities/runs/status.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,43 +43,42 @@
         Returns
         -------
         dict
             The results.
         """
         return self.results if self.results is not None else {}
 
-    def get_outputs(self, as_key: bool = False, as_dict: bool = False) -> list[dict[str, str | dict | Entity]]:
+    def get_outputs(self, as_key: bool = False, as_dict: bool = False) -> dict[str, str | dict | Entity]:
         """
         Get outputs.
 
         Parameters
         ----------
         as_key : bool
             If True, return outputs as keys.
         as_dict : bool
             If True, return outputs as dictionaries.
 
         Returns
         -------
-        list[dict[str, str | dict | Entity]]
+        dict[str, str | dict | Entity]
             The outputs.
         """
-        outputs = []
+        outputs = {}
         if self.outputs is None:
             return outputs
 
-        for i in self.outputs:
-            for parameter, key in i.items():
-                entity_type = self._get_entity_type(key)
-                entity = ENTITY_FUNC[entity_type](key)
-                if as_key:
-                    entity = entity.key
-                if as_dict:
-                    entity = entity.to_dict()
-                outputs.append({parameter: entity})
+        for parameter, key in self.outputs.items():
+            entity_type = self._get_entity_type(key)
+            entity = ENTITY_FUNC[entity_type](key)
+            if as_key:
+                entity = entity.key
+            if as_dict:
+                entity = entity.to_dict()
+            outputs[parameter] = entity
 
         return outputs
 
     @staticmethod
     def _get_entity_type(key: str) -> str:
         """
         Get entity type.
@@ -93,22 +92,22 @@
         -------
         str
             The entity type.
         """
         _, entity_type, _, _, _ = parse_entity_key(key)
         return entity_type
 
-    def get_values(self, values_list: list) -> list:
+    def get_values(self, values_list: list) -> dict:
         """
         Get values.
 
         Parameters
         ----------
         values_list : list
             The values list to search in.
 
         Returns
         -------
-        list
+        dict
             The values.
         """
         return {k: v for k, v in self.get_results().items() if k in values_list}
```

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/entities/secrets/crud.py` & `digitalhub_core-0.4.0b8/digitalhub_core/entities/secrets/crud.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 Secret operations module.
 """
 from __future__ import annotations
 
 import typing
 
 from digitalhub_core.context.builder import check_context, get_context
+from digitalhub_core.entities.entity_types import EntityTypes
 from digitalhub_core.entities.secrets.entity import secret_from_dict, secret_from_parameters
 from digitalhub_core.utils.api import api_ctx_delete, api_ctx_list, api_ctx_read, api_ctx_update
 from digitalhub_core.utils.io_utils import read_yaml
 
 if typing.TYPE_CHECKING:
     from digitalhub_core.entities.secrets.entity import Secret
 
 
-ENTITY_TYPE = "secrets"
+ENTITY_TYPE = EntityTypes.SECRETS.value
 
 
 def create_secret(**kwargs) -> Secret:
     """
     Create a new Secret instance with the specified parameters.
 
     Parameters
```

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/entities/secrets/entity.py` & `digitalhub_core-0.4.0b8/digitalhub_core/entities/secrets/entity.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from pathlib import Path
 
 from digitalhub_core.context.builder import get_context
 from digitalhub_core.entities._base.entity import Entity
 from digitalhub_core.entities._builders.metadata import build_metadata
 from digitalhub_core.entities._builders.spec import build_spec
 from digitalhub_core.entities._builders.status import build_status
+from digitalhub_core.entities.entity_types import EntityTypes
 from digitalhub_core.utils.api import api_ctx_create, api_ctx_list, api_ctx_read, api_ctx_update
 from digitalhub_core.utils.generic_utils import build_uuid, get_timestamp
 from digitalhub_core.utils.io_utils import write_yaml
 
 if typing.TYPE_CHECKING:
     from digitalhub_core.context.context import Context
     from digitalhub_core.entities.secrets.metadata import SecretMetadata
@@ -23,14 +24,16 @@
 
 
 class Secret(Entity):
     """
     A class representing a secret.
     """
 
+    ENTITY_TYPE = EntityTypes.SECRETS.value
+
     def __init__(
         self,
         project: str,
         name: str,
         uuid: str,
         kind: str,
         metadata: SecretMetadata,
@@ -61,15 +64,15 @@
             Owner of the object.
         """
         super().__init__()
         self.project = project
         self.name = name
         self.id = uuid
         self.kind = kind
-        self.key = f"store://{project}/secrets/{kind}/{name}:{uuid}"
+        self.key = f"store://{project}/{self.ENTITY_TYPE}/{kind}/{name}:{uuid}"
         self.metadata = metadata
         self.spec = spec
         self.status = status
         self.user = user
 
         # Add attributes to be used in the to_dict method
         self._obj_attr.extend(["project", "name", "id", "key"])
@@ -91,35 +94,35 @@
         -------
         Secret
             Entity saved.
         """
         obj = self.to_dict()
 
         if not update:
-            api = api_ctx_create(self.project, "secrets")
+            api = api_ctx_create(self.project, self.ENTITY_TYPE)
             new_obj = self._context().create_object(api, obj)
             self._update_attributes(new_obj)
             return self
 
         self.metadata.updated = obj["metadata"]["updated"] = get_timestamp()
-        api = api_ctx_update(self.project, "secrets", self.id)
+        api = api_ctx_update(self.project, self.ENTITY_TYPE, self.id)
         new_obj = self._context().update_object(api, obj)
         self._update_attributes(new_obj)
         return self
 
     def refresh(self) -> Secret:
         """
         Refresh object from backend.
 
         Returns
         -------
         Secret
             Entity refreshed.
         """
-        api = api_ctx_read(self.project, "secrets", self.id)
+        api = api_ctx_read(self.project, self.ENTITY_TYPE, self.id)
         obj = self._context().read_object(api)
         self._update_attributes(obj)
         return self
 
     def export(self, filename: str | None = None) -> None:
         """
         Export object as a YAML file.
@@ -174,15 +177,15 @@
         -------
         None
         """
         if self._context().local:
             raise NotImplementedError("set_secret() is not implemented for local projects.")
 
         obj = {self.name: value}
-        api = api_ctx_list(self.project, "secrets") + "/data"
+        api = api_ctx_list(self.project, self.ENTITY_TYPE) + "/data"
         self._context().update_object(api, obj)
 
     def read_secret_value(self) -> dict:
         """
         Read a secret from backend.
 
         Parameters
@@ -195,15 +198,15 @@
         str
             Value of the secret.
         """
         if self._context().local:
             raise NotImplementedError("read_secret() is not implemented for local projects.")
 
         params = {"keys": self.name}
-        api = api_ctx_list(self.project, "secrets") + "/data"
+        api = api_ctx_list(self.project, self.ENTITY_TYPE) + "/data"
         return self._context().read_object(api, params=params)
 
     #############################
     #  Static interface methods
     #############################
 
     @staticmethod
```

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/entities/secrets/spec.py` & `digitalhub_core-0.4.0b8/digitalhub_core/entities/secrets/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/entities/services/crud.py` & `digitalhub_core-0.4.0b8/digitalhub_core/entities/services/crud.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 Service operations module.
 """
 from __future__ import annotations
 
 import typing
 
 from digitalhub_core.context.builder import check_context, get_context
+from digitalhub_core.entities.entity_types import EntityTypes
 from digitalhub_core.entities.services.entity import service_from_dict, service_from_parameters
 from digitalhub_core.utils.api import api_ctx_delete, api_ctx_list, api_ctx_read, api_ctx_update
 from digitalhub_core.utils.io_utils import read_yaml
 
 if typing.TYPE_CHECKING:
     from digitalhub_core.entities.services.entity import Service
 
 
-ENTITY_TYPE = "services"
+ENTITY_TYPE = EntityTypes.SERVICES.value
 
 
 def create_service(**kwargs) -> Service:
     """
     Create a new Service instance with the specified parameters.
 
     Parameters
```

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/entities/services/entity.py` & `digitalhub_core-0.4.0b8/digitalhub_core/entities/services/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from pathlib import Path
 
 from digitalhub_core.context.builder import get_context
 from digitalhub_core.entities._base.entity import Entity
 from digitalhub_core.entities._builders.metadata import build_metadata
 from digitalhub_core.entities._builders.spec import build_spec
 from digitalhub_core.entities._builders.status import build_status
+from digitalhub_core.entities.entity_types import EntityTypes
 from digitalhub_core.utils.api import api_ctx_create, api_ctx_read, api_ctx_update
 from digitalhub_core.utils.generic_utils import build_uuid, get_timestamp
 from digitalhub_core.utils.io_utils import write_yaml
 
 if typing.TYPE_CHECKING:
     from digitalhub_core.context.context import Context
     from digitalhub_core.entities.services.metadata import ServiceMetadata
@@ -23,14 +24,16 @@
 
 
 class Service(Entity):
     """
     A class representing a service.
     """
 
+    ENTITY_TYPE = EntityTypes.SERVICES.value
+
     def __init__(
         self,
         project: str,
         name: str,
         uuid: str,
         kind: str,
         metadata: ServiceMetadata,
@@ -61,15 +64,15 @@
             Owner of the object.
         """
         super().__init__()
         self.project = project
         self.name = name
         self.id = uuid
         self.kind = kind
-        self.key = f"store://{project}/services/{kind}/{name}:{uuid}"
+        self.key = f"store://{project}/{self.ENTITY_TYPE}/{kind}/{name}:{uuid}"
         self.metadata = metadata
         self.spec = spec
         self.status = status
         self.user = user
 
         # Add attributes to be used in the to_dict method
         self._obj_attr.extend(["project", "name", "id", "key"])
@@ -91,35 +94,35 @@
         -------
         Service
             Entity saved.
         """
         obj = self.to_dict()
 
         if not update:
-            api = api_ctx_create(self.project, "services")
+            api = api_ctx_create(self.project, self.ENTITY_TYPE)
             new_obj = self._context().create_object(api, obj)
             self._update_attributes(new_obj)
             return self
 
         self.metadata.updated = obj["metadata"]["updated"] = get_timestamp()
-        api = api_ctx_update(self.project, "services", self.id)
+        api = api_ctx_update(self.project, self.ENTITY_TYPE, self.id)
         new_obj = self._context().update_object(api, obj)
         self._update_attributes(new_obj)
         return self
 
     def refresh(self) -> Service:
         """
         Refresh object from backend.
 
         Returns
         -------
         Service
             Entity refreshed.
         """
-        api = api_ctx_read(self.project, "services", self.id)
+        api = api_ctx_read(self.project, self.ENTITY_TYPE, self.id)
         obj = self._context().read_object(api)
         self._update_attributes(obj)
         return self
 
     def export(self, filename: str | None = None) -> None:
         """
         Export object as a YAML file.
```

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/entities/tasks/crud.py` & `digitalhub_core-0.4.0b8/digitalhub_core/entities/tasks/crud.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 Module for performing operations on tasks.
 """
 from __future__ import annotations
 
 import typing
 
 from digitalhub_core.context.builder import check_context, get_context
+from digitalhub_core.entities.entity_types import EntityTypes
 from digitalhub_core.entities.tasks.entity import task_from_dict, task_from_parameters
 from digitalhub_core.utils.api import api_ctx_delete, api_ctx_list, api_ctx_read, api_ctx_update
 from digitalhub_core.utils.io_utils import read_yaml
 
 if typing.TYPE_CHECKING:
     from digitalhub_core.entities.tasks.entity import Task
 
 
-ENTITY_TYPE = "tasks"
+ENTITY_TYPE = EntityTypes.TASKS.value
 
 
 def create_task(**kwargs) -> Task:
     """
     Create a new object instance.
 
     Parameters
```

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/entities/tasks/entity.py` & `digitalhub_core-0.4.0b8/digitalhub_core/entities/tasks/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from pathlib import Path
 
 from digitalhub_core.context.builder import get_context
 from digitalhub_core.entities._base.entity import Entity
 from digitalhub_core.entities._builders.metadata import build_metadata
 from digitalhub_core.entities._builders.spec import build_spec
 from digitalhub_core.entities._builders.status import build_status
+from digitalhub_core.entities.entity_types import EntityTypes
 from digitalhub_core.entities.runs.crud import delete_run, get_run, new_run, run_from_parameters
 from digitalhub_core.utils.api import api_ctx_create, api_ctx_read, api_ctx_update
 from digitalhub_core.utils.generic_utils import build_uuid, get_timestamp
 from digitalhub_core.utils.io_utils import write_yaml
 
 if typing.TYPE_CHECKING:
     from digitalhub_core.context.context import Context
@@ -25,14 +26,16 @@
 
 
 class Task(Entity):
     """
     A class representing a task.
     """
 
+    ENTITY_TYPE = EntityTypes.TASKS.value
+
     def __init__(
         self,
         project: str,
         uuid: str,
         kind: str,
         metadata: TaskMetadata,
         spec: TaskSpec,
@@ -59,15 +62,15 @@
         user : str
             Owner of the object.
         """
         super().__init__()
         self.project = project
         self.id = uuid
         self.kind = kind
-        self.key = f"store://{project}/tasks/{kind}/{uuid}"
+        self.key = f"store://{project}/{self.ENTITY_TYPE}/{kind}/{uuid}"
         self.metadata = metadata
         self.spec = spec
         self.status = status
         self.user = user
 
         # Add attributes to be used in the to_dict method
         self._obj_attr.extend(["project", "id", "key"])
@@ -89,35 +92,35 @@
         -------
         Task
             Entity saved.
         """
         obj = self.to_dict()
 
         if not update:
-            api = api_ctx_create(self.project, "tasks")
+            api = api_ctx_create(self.project, self.ENTITY_TYPE)
             new_obj = self._context().create_object(api, obj)
             self._update_attributes(new_obj)
             return self
 
         self.metadata.updated = obj["metadata"]["updated"] = get_timestamp()
-        api = api_ctx_update(self.project, "tasks", self.id)
+        api = api_ctx_update(self.project, self.ENTITY_TYPE, self.id)
         new_obj = self._context().update_object(api, obj)
         self._update_attributes(new_obj)
         return self
 
     def refresh(self) -> Task:
         """
         Refresh object from backend.
 
         Returns
         -------
         Task
             Entity refreshed.
         """
-        api = api_ctx_read(self.project, "tasks", self.id)
+        api = api_ctx_read(self.project, self.ENTITY_TYPE, self.id)
         obj = self._context().read_object(api)
         self._update_attributes(obj)
         return self
 
     def export(self, filename: str | None = None) -> None:
         """
         Export object as a YAML file.
@@ -155,28 +158,28 @@
 
     #############################
     #  Task methods
     #############################
 
     def run(
         self,
-        inputs: list | None,
-        outputs: list | None = None,
+        inputs: dict | None = None,
+        outputs: dict | None = None,
         parameters: dict | None = None,
         values: list | None = None,
         local_execution: bool = False,
     ) -> Run:
         """
         Run task.
 
         Parameters
         ----------
-        inputs : list
+        inputs : dict
             The inputs of the run.
-        outputs : list
+        outputs : dict
             The outputs of the run.
         parameters : dict
             The parameters of the run.
         values : list
             The values of the run.
         local_execution : bool
             Flag to indicate if the run will be executed locally.
```

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/entities/tasks/models.py` & `digitalhub_core-0.4.0b8/digitalhub_core/entities/tasks/models.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/entities/workflows/crud.py` & `digitalhub_core-0.4.0b8/digitalhub_core/entities/workflows/crud.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 Workflow operations module.
 """
 from __future__ import annotations
 
 import typing
 
 from digitalhub_core.context.builder import check_context, get_context
+from digitalhub_core.entities.entity_types import EntityTypes
 from digitalhub_core.entities.workflows.entity import workflow_from_dict, workflow_from_parameters
 from digitalhub_core.utils.api import api_ctx_delete, api_ctx_list, api_ctx_read, api_ctx_update
 from digitalhub_core.utils.io_utils import read_yaml
 
 if typing.TYPE_CHECKING:
     from digitalhub_core.entities.workflows.entity import Workflow
 
 
-ENTITY_TYPE = "workflows"
+ENTITY_TYPE = EntityTypes.WORKFLOWS.value
 
 
 def create_workflow(**kwargs) -> Workflow:
     """
     Create a new Workflow instance with the specified parameters.
 
     Parameters
```

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/entities/workflows/entity.py` & `digitalhub_core-0.4.0b8/digitalhub_core/entities/workflows/entity.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from pathlib import Path
 
 from digitalhub_core.context.builder import get_context
 from digitalhub_core.entities._base.entity import Entity
 from digitalhub_core.entities._builders.metadata import build_metadata
 from digitalhub_core.entities._builders.spec import build_spec
 from digitalhub_core.entities._builders.status import build_status
+from digitalhub_core.entities.entity_types import EntityTypes
 from digitalhub_core.entities.tasks.crud import create_task, create_task_from_dict, delete_task, new_task
 from digitalhub_core.utils.api import api_ctx_create, api_ctx_list, api_ctx_read, api_ctx_update
 from digitalhub_core.utils.exceptions import BackendError, EntityError
 from digitalhub_core.utils.generic_utils import build_uuid, get_timestamp
 from digitalhub_core.utils.io_utils import write_yaml
 
 if typing.TYPE_CHECKING:
@@ -28,14 +29,16 @@
 
 
 class Workflow(Entity):
     """
     A class representing a workflow.
     """
 
+    ENTITY_TYPE = EntityTypes.WORKFLOWS.value
+
     def __init__(
         self,
         project: str,
         name: str,
         uuid: str,
         kind: str,
         metadata: WorkflowMetadata,
@@ -66,15 +69,15 @@
             Owner of the object.
         """
         super().__init__()
         self.project = project
         self.name = name
         self.id = uuid
         self.kind = kind
-        self.key = f"store://{project}/workflows/{kind}/{name}:{uuid}"
+        self.key = f"store://{project}/{self.ENTITY_TYPE}/{kind}/{name}:{uuid}"
         self.metadata = metadata
         self.spec = spec
         self.status = status
         self.user = user
 
         # Add attributes to be used in the to_dict method
         self._obj_attr.extend(["project", "name", "id", "key"])
@@ -99,35 +102,35 @@
         -------
         Workflow
             Entity saved.
         """
         obj = self.to_dict()
 
         if not update:
-            api = api_ctx_create(self.project, "workflows")
+            api = api_ctx_create(self.project, self.ENTITY_TYPE)
             new_obj = self._context().create_object(api, obj)
             self._update_attributes(new_obj)
             return self
 
         self.metadata.updated = obj["metadata"]["updated"] = get_timestamp()
-        api = api_ctx_update(self.project, "workflows", self.id)
+        api = api_ctx_update(self.project, self.ENTITY_TYPE, self.id)
         new_obj = self._context().update_object(api, obj)
         self._update_attributes(new_obj)
         return self
 
     def refresh(self) -> Workflow:
         """
         Refresh object from backend.
 
         Returns
         -------
         Workflow
             Entity refreshed.
         """
-        api = api_ctx_read(self.project, "workflows", self.id)
+        api = api_ctx_read(self.project, self.ENTITY_TYPE, self.id)
         obj = self._context().read_object(api)
         self._update_attributes(obj)
         return self
 
     def export(self, filename: str | None = None) -> None:
         """
         Export object as a YAML file.
@@ -175,16 +178,16 @@
     def run(
         self,
         action: str = "pipeline",
         labels: list[dict] | None = None,
         env: list[dict] | None = None,
         secrets: list[str] | None = None,
         schedule: str | None = None,
-        inputs: list | None = None,
-        outputs: list | None = None,
+        inputs: dict | None = None,
+        outputs: dict | None = None,
         parameters: dict | None = None,
         values: list | None = None,
         local_execution: bool = False,
         **kwargs,
     ) -> Run:
         """
         Run workflow.
@@ -195,17 +198,17 @@
             The labels of the task.
         env : list[dict]
             The env variables of the task. Task parameter.
         secrets : list[str]
             The secrets of the task. Task parameter.
         schedule : str
             The schedule of the task. Task parameter.
-        inputs : list
+        inputs : dict
             Workflow inputs. Run parameter.
-        outputs : list
+        outputs : dict
             Workflow outputs. Run parameter.
         parameters : dict
             Workflow parameters. Run parameter.
         values : list
             Workflow values. Run parameter.
         local_execution : bool
             Flag to determine if object has local execution. Run parameter.
@@ -232,14 +235,17 @@
                 labels=labels,
                 env=env,
                 secrets=secrets,
                 schedule=schedule,
                 **kwargs,
             )
 
+        if local_execution:
+            raise BackendError("Local execution is not supported for workflows.")
+
         # Run function from task
         run = task.run(inputs, outputs, parameters, values, local_execution)
 
         # If execution is done by DHCore backend, return the object
         if not local_execution:
             if self._context().local:
                 raise BackendError("Cannot run remote function with local backend.")
@@ -261,15 +267,15 @@
             Action to check.
 
         Returns
         -------
         None | Task
             Task if exists, None otherwise.
         """
-        api = api_ctx_list(self.project, "tasks")
+        api = api_ctx_list(self.project, EntityTypes.TASKS.value)
         params = {"function": self._get_workflow_string(), "kind": f"{self.kind}+{action}"}
         objs = self._context().list_objects(api, params=params)
         for i in objs:
             self._tasks[action] = create_task_from_dict(i)
             return self._tasks[action]
 
     def _get_workflow_string(self) -> str:
```

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/registry/import_utils.py` & `digitalhub_core-0.4.0b8/digitalhub_core/registry/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -103,7 +103,54 @@
             return
 
         # Try ot import registry from entities.registries module
         try:
             import_module(f"{package}.entities.registries")
         except Exception:
             pass
+
+
+def create_info(
+    root: str, entity_type: str, prefix: str, suffix: str | None = "", runtime_info: dict | None = None
+) -> dict:
+    """
+    Create entity info.
+
+    Parameters
+    ----------
+    root : str
+        Root module.
+    entity_type : str
+        Entity type.
+    prefix : str
+        Entity prefix.
+    suffix : str
+        Entity suffix.
+    runtime_info : dict
+        Runtime info.
+
+    Returns
+    -------
+    dict
+        Entity info.
+    """
+    dict_ = {
+        "entity_type": entity_type,
+        "spec": {
+            "module": f"{root}.{entity_type}.spec",
+            "class_name": f"{prefix}Spec{suffix}",
+            "parameters_validator": f"{prefix}Params{suffix}",
+        },
+        "status": {
+            "module": f"{root}.{entity_type}.status",
+            "class_name": f"{prefix}Status{suffix}",
+        },
+        "metadata": {
+            "module": f"{root}.{entity_type}.metadata",
+            "class_name": f"{prefix}Metadata{suffix}",
+        },
+    }
+    # Add runtime only if provided
+    # (in functions, tasks, runs and workflows)
+    if runtime_info is not None:
+        dict_["runtime"] = runtime_info
+    return dict_
```

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/registry/models.py` & `digitalhub_core-0.4.0b8/digitalhub_core/registry/models.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/registry/registry.py` & `digitalhub_core-0.4.0b8/digitalhub_core/registry/registry.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/runtimes/base.py` & `digitalhub_core-0.4.0b8/digitalhub_core/runtimes/base.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/runtimes/builder.py` & `digitalhub_core-0.4.0b8/digitalhub_core/runtimes/builder.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 Runtime builder function.
 """
 from __future__ import annotations
 
 import typing
 
-from digitalhub_core.registry.import_utils import import_class
 from digitalhub_core.registry.registry import registry
+from digitalhub_core.registry.utils import import_class
 
 if typing.TYPE_CHECKING:
     from digitalhub_core.registry.models import RegistryEntry
     from digitalhub_core.runtimes.base import Runtime
 
 
 def build_runtime(kind: str) -> Runtime:
```

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/stores/builder.py` & `digitalhub_core-0.4.0b8/digitalhub_core/stores/builder.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/stores/objects/base.py` & `digitalhub_core-0.4.0b8/digitalhub_core/stores/objects/base.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/stores/objects/local.py` & `digitalhub_core-0.4.0b8/digitalhub_core/stores/objects/local.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/stores/objects/remote.py` & `digitalhub_core-0.4.0b8/digitalhub_core/stores/objects/remote.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/stores/objects/s3.py` & `digitalhub_core-0.4.0b8/digitalhub_core/stores/objects/s3.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/stores/objects/sql.py` & `digitalhub_core-0.4.0b8/digitalhub_core/stores/objects/sql.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/utils/api.py` & `digitalhub_core-0.4.0b8/digitalhub_core/utils/api.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/utils/env_utils.py` & `digitalhub_core-0.4.0b8/digitalhub_core/utils/env_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/utils/file_utils.py` & `digitalhub_core-0.4.0b8/digitalhub_core/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/utils/generic_utils.py` & `digitalhub_core-0.4.0b8/digitalhub_core/utils/generic_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/utils/git_utils.py` & `digitalhub_core-0.4.0b8/digitalhub_core/utils/git_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/utils/io_utils.py` & `digitalhub_core-0.4.0b8/digitalhub_core/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core/utils/uri_utils.py` & `digitalhub_core-0.4.0b8/digitalhub_core/utils/uri_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core.egg-info/PKG-INFO` & `digitalhub_core-0.4.0b8/digitalhub_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalhub-core
-Version: 0.4.0b4
+Version: 0.4.0b8
 Summary: Python SDK for DHCore
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 License:                               Apache License
                                 Version 2.0, January 2004
                              http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `digitalhub_core-0.4.0b4/digitalhub_core.egg-info/SOURCES.txt` & `digitalhub_core-0.4.0b8/digitalhub_core.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 digitalhub_core/client/objects/base.py
 digitalhub_core/client/objects/dhcore.py
 digitalhub_core/client/objects/local.py
 digitalhub_core/context/__init__.py
 digitalhub_core/context/builder.py
 digitalhub_core/context/context.py
 digitalhub_core/entities/__init__.py
+digitalhub_core/entities/entity_types.py
 digitalhub_core/entities/registries.py
 digitalhub_core/entities/_base/__init__.py
 digitalhub_core/entities/_base/base.py
 digitalhub_core/entities/_base/entity.py
 digitalhub_core/entities/_base/metadata.py
 digitalhub_core/entities/_base/spec.py
 digitalhub_core/entities/_base/status.py
@@ -74,17 +75,17 @@
 digitalhub_core/entities/workflows/__init__.py
 digitalhub_core/entities/workflows/crud.py
 digitalhub_core/entities/workflows/entity.py
 digitalhub_core/entities/workflows/metadata.py
 digitalhub_core/entities/workflows/spec.py
 digitalhub_core/entities/workflows/status.py
 digitalhub_core/registry/__init__.py
-digitalhub_core/registry/import_utils.py
 digitalhub_core/registry/models.py
 digitalhub_core/registry/registry.py
+digitalhub_core/registry/utils.py
 digitalhub_core/runtimes/__init__.py
 digitalhub_core/runtimes/base.py
 digitalhub_core/runtimes/builder.py
 digitalhub_core/stores/__init__.py
 digitalhub_core/stores/builder.py
 digitalhub_core/stores/objects/__init__.py
 digitalhub_core/stores/objects/base.py
```

### Comparing `digitalhub_core-0.4.0b4/pyproject.toml` & `digitalhub_core-0.4.0b8/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "digitalhub-core"
-version = "0.4.0b4"
+version = "0.4.0b8"
 description = "Python SDK for DHCore"
 readme = "README.md"
 authors = [
     { name = "Fondazione Bruno Kessler", email = "dslab@fbk.eu" },
     { name = "Matteo Martini", email = "mmartini@fbk.eu" }
 ]
 license = { file = "LICENSE.txt" }
@@ -61,15 +61,15 @@
 [tool.ruff.extend-per-file-ignores]
 "__init__.py" = ["F401"]
 
 [tool.ruff.pydocstyle]
 convention = "numpy"
 
 [tool.bumpver]
-current_version = "0.4.0b4"
+current_version = "0.4.0b8"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = false
 tag             = false
 push            = false
 
 [tool.bumpver.file_patterns]
```

