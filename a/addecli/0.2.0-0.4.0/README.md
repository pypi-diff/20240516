# Comparing `tmp/addecli-0.2.0.tar.gz` & `tmp/addecli-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "addecli-0.2.0.tar", last modified: Wed May 15 23:00:35 2024, max compression
+gzip compressed data, was "addecli-0.4.0.tar", last modified: Thu May 16 00:59:23 2024, max compression
```

## Comparing `addecli-0.2.0.tar` & `addecli-0.4.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       10 2024-05-15 23:00:25.166730 addecli-0.2.0/README.md
--rw-r--r--   0        0        0      455 2024-05-15 23:00:35.590806 addecli-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-15 23:00:25.166730 addecli-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0      260 1970-01-01 00:00:00.000000 addecli-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       10 2024-05-16 00:59:15.266599 addecli-0.4.0/README.md
+-rw-r--r--   0        0        0      455 2024-05-16 00:59:23.910527 addecli-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-16 00:59:15.266599 addecli-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0      260 1970-01-01 00:00:00.000000 addecli-0.4.0/PKG-INFO
```

