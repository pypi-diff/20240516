# Comparing `tmp/hmmer_tables-0.6.0.tar.gz` & `tmp/hmmer_tables-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hmmer_tables-0.6.0.tar", max compression
+gzip compressed data, was "hmmer_tables-0.6.1.tar", max compression
```

## Comparing `hmmer_tables-0.6.0.tar` & `hmmer_tables-0.6.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1063 2024-02-22 14:19:19.933340 hmmer_tables-0.6.0/LICENSE
--rw-r--r--   0        0        0       15 2024-02-22 14:19:19.933340 hmmer_tables-0.6.0/README.md
--rw-r--r--   0        0        0        0 2024-02-22 14:19:19.933340 hmmer_tables-0.6.0/hmmer_tables/__init__.py
--rw-r--r--   0        0        0      692 2024-02-22 14:19:19.933340 hmmer_tables-0.6.0/hmmer_tables/cleanup.py
--rw-r--r--   0        0        0      366 2024-02-22 14:19:19.933340 hmmer_tables-0.6.0/hmmer_tables/csv_iter.py
--rw-r--r--   0        0        0     3419 2024-02-22 14:19:19.933340 hmmer_tables-0.6.0/hmmer_tables/domtbl.py
--rw-r--r--   0        0        0     1542 2024-02-22 14:19:19.933340 hmmer_tables-0.6.0/hmmer_tables/output.py
--rw-r--r--   0        0        0       72 2024-02-22 14:19:19.933340 hmmer_tables-0.6.0/hmmer_tables/path_like.py
--rw-r--r--   0        0        0     8262 2024-02-22 14:19:19.933340 hmmer_tables-0.6.0/hmmer_tables/query.py
--rw-r--r--   0        0        0     2197 2024-02-22 14:19:19.933340 hmmer_tables-0.6.0/hmmer_tables/tbl.py
--rw-r--r--   0        0        0      575 2024-02-22 14:19:19.933340 hmmer_tables-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      736 1970-01-01 00:00:00.000000 hmmer_tables-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-16 11:05:25.203067 hmmer_tables-0.6.1/LICENSE
+-rw-r--r--   0        0        0       15 2024-05-16 11:05:25.203067 hmmer_tables-0.6.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-16 11:05:25.203067 hmmer_tables-0.6.1/hmmer_tables/__init__.py
+-rw-r--r--   0        0        0      692 2024-05-16 11:05:25.203067 hmmer_tables-0.6.1/hmmer_tables/cleanup.py
+-rw-r--r--   0        0        0     2061 2024-05-16 11:05:25.203067 hmmer_tables-0.6.1/hmmer_tables/cli.py
+-rw-r--r--   0        0        0      366 2024-05-16 11:05:25.203067 hmmer_tables-0.6.1/hmmer_tables/csv_iter.py
+-rw-r--r--   0        0        0     3419 2024-05-16 11:05:25.203067 hmmer_tables-0.6.1/hmmer_tables/domtbl.py
+-rw-r--r--   0        0        0     1542 2024-05-16 11:05:25.203067 hmmer_tables-0.6.1/hmmer_tables/output.py
+-rw-r--r--   0        0        0       72 2024-05-16 11:05:25.203067 hmmer_tables-0.6.1/hmmer_tables/path_like.py
+-rw-r--r--   0        0        0     8262 2024-05-16 11:05:25.203067 hmmer_tables-0.6.1/hmmer_tables/query.py
+-rw-r--r--   0        0        0     2197 2024-05-16 11:05:25.203067 hmmer_tables-0.6.1/hmmer_tables/tbl.py
+-rw-r--r--   0        0        0      565 2024-05-16 11:05:25.203067 hmmer_tables-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      721 1970-01-01 00:00:00.000000 hmmer_tables-0.6.1/PKG-INFO
```

### Comparing `hmmer_tables-0.6.0/LICENSE` & `hmmer_tables-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hmmer_tables-0.6.0/hmmer_tables/cleanup.py` & `hmmer_tables-0.6.1/hmmer_tables/cleanup.py`

 * *Files identical despite different names*

### Comparing `hmmer_tables-0.6.0/hmmer_tables/domtbl.py` & `hmmer_tables-0.6.1/hmmer_tables/domtbl.py`

 * *Files identical despite different names*

### Comparing `hmmer_tables-0.6.0/hmmer_tables/output.py` & `hmmer_tables-0.6.1/hmmer_tables/output.py`

 * *Files identical despite different names*

### Comparing `hmmer_tables-0.6.0/hmmer_tables/query.py` & `hmmer_tables-0.6.1/hmmer_tables/query.py`

 * *Files identical despite different names*

### Comparing `hmmer_tables-0.6.0/hmmer_tables/tbl.py` & `hmmer_tables-0.6.1/hmmer_tables/tbl.py`

 * *Files identical despite different names*

