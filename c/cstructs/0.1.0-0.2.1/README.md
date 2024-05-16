# Comparing `tmp/cstructs-0.1.0.tar.gz` & `tmp/cstructs-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cstructs-0.1.0.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `cstructs-0.1.0.tar` & `cstructs-0.2.1.tar`

### file list

```diff
@@ -1,4 +1,35 @@
--rw-r--r--   0        0        0        0 2023-11-29 18:33:04.049933 cstructs-0.1.0/cstructs/__init__.py
--rw-r--r--   0        0        0      352 2023-11-29 18:31:45.282699 cstructs-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       10 2023-11-29 18:30:15.921202 cstructs-0.1.0/README.md
--rw-r--r--   0        0        0      447 1970-01-01 00:00:00.000000 cstructs-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 cstructs-0.2.1/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 cstructs-0.2.1/.idea/.gitignore
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 cstructs-0.2.1/.idea/cstructs.iml
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 cstructs-0.2.1/.idea/discord.xml
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 cstructs-0.2.1/.idea/misc.xml
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 cstructs-0.2.1/.idea/modules.xml
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 cstructs-0.2.1/.idea/vcs.xml
+-rw-r--r--   0        0        0    28484 2020-02-02 00:00:00.000000 cstructs-0.2.1/.idea/workspace.xml
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 cstructs-0.2.1/.idea/copyright/gplv3.xml
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 cstructs-0.2.1/.idea/copyright/profiles_settings.xml
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 cstructs-0.2.1/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 cstructs-0.2.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 cstructs-0.2.1/.idea/shelf/Uncommitted_changes_before_Update_at_5_16_2024_2_44_PM__Changes_.xml
+-rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 cstructs-0.2.1/.idea/shelf/Uncommitted_changes_before_Update_at_5_16_2024_2_44_PM_[Changes]/shelved.patch
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 cstructs-0.2.1/docs/nativetypes
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 cstructs-0.2.1/src/cstructs/__about__.py
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 cstructs-0.2.1/src/cstructs/__init__.py
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 cstructs-0.2.1/src/cstructs/exc.py
+-rw-r--r--   0        0        0     7434 2020-02-02 00:00:00.000000 cstructs-0.2.1/src/cstructs/nativetypes.py
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 cstructs-0.2.1/src/cstructs/util.py
+-rw-r--r--   0        0        0     4827 2020-02-02 00:00:00.000000 cstructs-0.2.1/src/cstructs/datastruct/__init__.py
+-rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 cstructs-0.2.1/src/cstructs/datastruct/metadata.py
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 cstructs-0.2.1/src/cstructs/datastruct/reader.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 cstructs-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 cstructs-0.2.1/tests/test_decorator.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 cstructs-0.2.1/tests/test_inheritance.py
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 cstructs-0.2.1/tests/test_metaclass.py
+-rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 cstructs-0.2.1/tests/test_metadata.py
+-rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 cstructs-0.2.1/tests/test_read.py
+-rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 cstructs-0.2.1/tests/test_write.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 cstructs-0.2.1/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 cstructs-0.2.1/LICENSE.txt
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 cstructs-0.2.1/README.md
+-rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 cstructs-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3962 2020-02-02 00:00:00.000000 cstructs-0.2.1/PKG-INFO
```

