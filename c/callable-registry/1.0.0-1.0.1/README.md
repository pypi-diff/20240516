# Comparing `tmp/callable-registry-1.0.0.tar.gz` & `tmp/callable-registry-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "callable-registry-1.0.0.tar", last modified: Thu May 16 15:12:39 2024, max compression
+gzip compressed data, was "callable-registry-1.0.1.tar", last modified: Thu May 16 15:41:15 2024, max compression
```

## Comparing `callable-registry-1.0.0.tar` & `callable-registry-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      168 2024-03-03 15:10:40.743669 callable-registry-1.0.0/README.md
--rw-r--r--   0        0        0     1360 2024-05-16 14:54:12.805777 callable-registry-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      345 2024-03-03 15:10:40.743669 callable-registry-1.0.0/registry/__init__.py
--rw-r--r--   0        0        0     7255 2024-03-03 15:10:40.743669 callable-registry-1.0.0/registry/registry.py
--rw-r--r--   0        0        0       22 2024-03-04 07:03:25.305586 callable-registry-1.0.0/registry/version.py
--rw-r--r--   0        0        0        0 2024-03-03 15:10:40.743669 callable-registry-1.0.0/tests/conftest.py
--rw-r--r--   0        0        0     5783 2024-03-03 15:10:40.743669 callable-registry-1.0.0/tests/test_registry.py
--rw-r--r--   0        0        0      142 2024-03-03 15:10:40.743669 callable-registry-1.0.0/tests/test_version.py
--rw-r--r--   0        0        0      401 1970-01-01 00:00:00.000000 callable-registry-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      168 2024-05-16 15:40:47.536331 callable-registry-1.0.1/README.md
+-rw-r--r--   0        0        0     1360 2024-05-16 15:40:47.536331 callable-registry-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      354 2024-05-16 15:40:47.536331 callable-registry-1.0.1/registry/__init__.py
+-rw-r--r--   0        0        0     7255 2024-05-16 15:40:47.536331 callable-registry-1.0.1/registry/registry.py
+-rw-r--r--   0        0        0       22 2024-05-16 15:40:47.536331 callable-registry-1.0.1/registry/version.py
+-rw-r--r--   0        0        0        0 2024-05-16 15:40:47.536331 callable-registry-1.0.1/tests/conftest.py
+-rw-r--r--   0        0        0     5783 2024-05-16 15:40:47.536331 callable-registry-1.0.1/tests/test_registry.py
+-rw-r--r--   0        0        0      142 2024-05-16 15:40:47.536331 callable-registry-1.0.1/tests/test_version.py
+-rw-r--r--   0        0        0      401 1970-01-01 00:00:00.000000 callable-registry-1.0.1/PKG-INFO
```

### Comparing `callable-registry-1.0.0/pyproject.toml` & `callable-registry-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     { name = "Tim Cogan", email = "tim@cogan.dev" },
 ]
 dependencies = [
     "typing_extensions; python_version < '3.11'",
 ]
 readme = "README.md"
 dynamic = []
-version = "1.0.0"
+version = "1.0.1"
 
 [project.license]
 text = "Apache"
 
 [project.optional-dependencies]
 
 [tool.autoflake]
```

### Comparing `callable-registry-1.0.0/registry/registry.py` & `callable-registry-1.0.1/registry/registry.py`

 * *Files identical despite different names*

### Comparing `callable-registry-1.0.0/tests/test_registry.py` & `callable-registry-1.0.1/tests/test_registry.py`

 * *Files identical despite different names*

