# Comparing `tmp/aipkgs_database-1.0.1.tar.gz` & `tmp/aipkgs_database-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aipkgs_database-1.0.1.tar", max compression
+gzip compressed data, was "aipkgs_database-1.0.2.tar", max compression
```

## Comparing `aipkgs_database-1.0.1.tar` & `aipkgs_database-1.0.2.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0        0 2023-11-26 13:36:17.132915 aipkgs_database-1.0.1/README.md
--rw-r--r--   0        0        0        0 2023-11-26 13:36:17.132866 aipkgs_database-1.0.1/aipkgs_database/__init__.py
--rw-r--r--   0        0        0      991 2023-11-26 14:05:45.319440 aipkgs_database-1.0.1/aipkgs_database/core.py
--rw-r--r--   0        0        0     1906 2023-11-26 18:17:16.222025 aipkgs_database-1.0.1/aipkgs_database/helpers.py
--rw-r--r--   0        0        0      330 2024-05-15 22:19:25.647215 aipkgs_database-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      393 1970-01-01 00:00:00.000000 aipkgs_database-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-11-26 13:36:17.132915 aipkgs_database-1.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-11-26 13:36:17.132866 aipkgs_database-1.0.2/aipkgs_database/__init__.py
+-rw-r--r--   0        0        0      991 2023-11-26 14:05:45.319440 aipkgs_database-1.0.2/aipkgs_database/core.py
+-rw-r--r--   0        0        0     1756 2024-05-15 23:24:32.255088 aipkgs_database-1.0.2/aipkgs_database/db_engine/helpers.py
+-rw-r--r--   0        0        0     1906 2023-11-26 18:17:16.222025 aipkgs_database-1.0.2/aipkgs_database/helpers.py
+-rw-r--r--   0        0        0      330 2024-05-15 23:24:37.669706 aipkgs_database-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      393 1970-01-01 00:00:00.000000 aipkgs_database-1.0.2/PKG-INFO
```

### Comparing `aipkgs_database-1.0.1/aipkgs_database/core.py` & `aipkgs_database-1.0.2/aipkgs_database/core.py`

 * *Files identical despite different names*

### Comparing `aipkgs_database-1.0.1/aipkgs_database/helpers.py` & `aipkgs_database-1.0.2/aipkgs_database/helpers.py`

 * *Files identical despite different names*

