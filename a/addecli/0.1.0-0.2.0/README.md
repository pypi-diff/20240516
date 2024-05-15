# Comparing `tmp/addecli-0.1.0.tar.gz` & `tmp/addecli-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "addecli-0.1.0.tar", last modified: Wed May 15 22:14:11 2024, max compression
+gzip compressed data, was "addecli-0.2.0.tar", last modified: Wed May 15 23:00:35 2024, max compression
```

## Comparing `addecli-0.1.0.tar` & `addecli-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0       10 2024-05-15 22:13:58.796246 addecli-0.1.0/README.md
--rw-r--r--   0        0        0      381 2024-05-15 22:14:11.832248 addecli-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-15 22:13:58.796246 addecli-0.1.0/src/addecli/__init__.py
--rw-r--r--   0        0        0        0 2024-05-15 22:13:58.796246 addecli-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      231 1970-01-01 00:00:00.000000 addecli-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       10 2024-05-15 23:00:25.166730 addecli-0.2.0/README.md
+-rw-r--r--   0        0        0      455 2024-05-15 23:00:35.590806 addecli-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-15 23:00:25.166730 addecli-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      260 1970-01-01 00:00:00.000000 addecli-0.2.0/PKG-INFO
```

