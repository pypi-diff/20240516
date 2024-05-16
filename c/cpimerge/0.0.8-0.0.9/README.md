# Comparing `tmp/cpimerge-0.0.8.tar.gz` & `tmp/cpimerge-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpimerge-0.0.8.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `cpimerge-0.0.8.tar` & `cpimerge-0.0.9.tar`

### file list

```diff
@@ -1,5 +1,8 @@
--rw-r--r--   0        0        0     1073 2024-05-16 14:41:39.767562 cpimerge-0.0.8/LICENSE
--rw-r--r--   0        0        0      423 2024-05-16 19:08:03.347546 cpimerge-0.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-16 14:41:37.832006 cpimerge-0.0.8/src/cpimerge/__init__.py
--rw-r--r--   0        0        0        0 2024-05-16 15:31:06.257693 cpimerge-0.0.8/src/cpimerge/__main__.py
--rw-r--r--   0        0        0      541 1970-01-01 00:00:00.000000 cpimerge-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpimerge-0.0.9/src/cpimerge/__init__.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 cpimerge-0.0.9/src/cpimerge/__main__.py
+-rw-r--r--   0        0        0    15454 2020-02-02 00:00:00.000000 cpimerge-0.0.9/src/cpimerge/cpimerge.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 cpimerge-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 cpimerge-0.0.9/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpimerge-0.0.9/README.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 cpimerge-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 cpimerge-0.0.9/PKG-INFO
```

### Comparing `cpimerge-0.0.8/LICENSE` & `cpimerge-0.0.9/LICENSE`

 * *Files identical despite different names*

