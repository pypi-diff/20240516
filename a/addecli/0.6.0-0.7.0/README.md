# Comparing `tmp/addecli-0.6.0.tar.gz` & `tmp/addecli-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "addecli-0.6.0.tar", last modified: Thu May 16 15:21:54 2024, max compression
+gzip compressed data, was "addecli-0.7.0.tar", last modified: Thu May 16 15:27:42 2024, max compression
```

## Comparing `addecli-0.6.0.tar` & `addecli-0.7.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       10 2024-05-16 15:21:45.144465 addecli-0.6.0/README.md
--rw-r--r--   0        0        0      459 2024-05-16 15:21:54.252479 addecli-0.6.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-16 15:21:45.144465 addecli-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0      260 1970-01-01 00:00:00.000000 addecli-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0       10 2024-05-16 15:27:35.150319 addecli-0.7.0/README.md
+-rw-r--r--   0        0        0      455 2024-05-16 15:27:42.238407 addecli-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-16 15:27:35.150319 addecli-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0      260 1970-01-01 00:00:00.000000 addecli-0.7.0/PKG-INFO
```

