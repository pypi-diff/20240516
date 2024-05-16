# Comparing `tmp/ondivi-0.0.1a0.tar.gz` & `tmp/ondivi-0.0.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ondivi-0.0.1a0.tar", max compression
+gzip compressed data, was "ondivi-0.0.2a0.tar", max compression
```

## Comparing `ondivi-0.0.1a0.tar` & `ondivi-0.0.2a0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1109 2024-05-16 09:32:56.849244 ondivi-0.0.1a0/LICENSE
--rw-r--r--   0        0        0      793 2024-05-16 10:27:17.085708 ondivi-0.0.1a0/README.md
--rw-r--r--   0        0        0        0 2024-05-16 09:30:49.208583 ondivi-0.0.1a0/ondivi/__init__.py
--rw-r--r--   0        0        0     3066 2024-05-16 10:22:17.975555 ondivi-0.0.1a0/ondivi/__main__.py
--rw-r--r--   0        0        0     2271 2024-05-16 09:59:31.617235 ondivi-0.0.1a0/pyproject.toml
--rw-r--r--   0        0        0     1277 1970-01-01 00:00:00.000000 ondivi-0.0.1a0/PKG-INFO
+-rw-r--r--   0        0        0     1109 2024-05-16 09:32:56.849244 ondivi-0.0.2a0/LICENSE
+-rw-r--r--   0        0        0      793 2024-05-16 10:27:17.085708 ondivi-0.0.2a0/README.md
+-rw-r--r--   0        0        0        0 2024-05-16 09:30:49.208583 ondivi-0.0.2a0/ondivi/__init__.py
+-rw-r--r--   0        0        0     3066 2024-05-16 10:22:17.975555 ondivi-0.0.2a0/ondivi/__main__.py
+-rw-r--r--   0        0        0     2271 2024-05-16 10:28:39.322437 ondivi-0.0.2a0/pyproject.toml
+-rw-r--r--   0        0        0     1277 1970-01-01 00:00:00.000000 ondivi-0.0.2a0/PKG-INFO
```

### Comparing `ondivi-0.0.1a0/LICENSE` & `ondivi-0.0.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `ondivi-0.0.1a0/README.md` & `ondivi-0.0.2a0/README.md`

 * *Files identical despite different names*

### Comparing `ondivi-0.0.1a0/ondivi/__main__.py` & `ondivi-0.0.2a0/ondivi/__main__.py`

 * *Files identical despite different names*

### Comparing `ondivi-0.0.1a0/pyproject.toml` & `ondivi-0.0.2a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ondivi"
-version = "0.0.1a"
+version = "0.0.2a"
 description = ""
 authors = ["Almaz Ilaletdinov <a.ilaletdinov@yandex.ru>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
 gitpython = "3.1.43"
```

### Comparing `ondivi-0.0.1a0/PKG-INFO` & `ondivi-0.0.2a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ondivi
-Version: 0.0.1a0
+Version: 0.0.2a0
 Summary: 
 Author: Almaz Ilaletdinov
 Author-email: a.ilaletdinov@yandex.ru
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

