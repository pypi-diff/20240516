# Comparing `tmp/pillory-1.1.0.tar.gz` & `tmp/pillory-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pillory-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pillory-1.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pillory-1.1.0.tar` & `pillory-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      797 2024-05-16 16:02:52.985870 pillory-1.1.0/.circleci/config.yml
--rw-r--r--   0        0        0       50 2024-05-16 16:02:52.985870 pillory-1.1.0/.gitignore
--rw-r--r--   0        0        0      359 2024-05-16 16:02:52.985870 pillory-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     9161 2024-05-16 16:02:52.985870 pillory-1.1.0/LICENSE
--rw-r--r--   0        0        0      354 2024-05-16 16:02:52.985870 pillory-1.1.0/Makefile
--rw-r--r--   0        0        0     4793 2024-05-16 16:02:52.985870 pillory-1.1.0/README.md
--rw-r--r--   0        0        0     1372 2024-05-16 16:02:52.985870 pillory-1.1.0/dev-requirements.txt
--rw-r--r--   0        0        0       41 2024-05-16 16:02:52.985870 pillory-1.1.0/example/__init__.py
--rw-r--r--   0        0        0      311 2024-05-16 16:02:52.985870 pillory-1.1.0/example/definition.py
--rw-r--r--   0        0        0      180 2024-05-16 16:02:52.985870 pillory-1.1.0/example/empty/README.txt
--rw-r--r--   0        0        0      649 2024-05-16 16:02:52.985870 pillory-1.1.0/example/test_use.py
--rw-r--r--   0        0        0      222 2024-05-16 16:02:52.985870 pillory-1.1.0/example/use.py
--rwxr-xr-x   0        0        0     8572 2024-05-16 16:02:52.985870 pillory-1.1.0/pillory.py
--rw-r--r--   0        0        0     1093 2024-05-16 16:02:52.985870 pillory-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1245 2024-05-16 16:02:52.985870 pillory-1.1.0/test_example.py
--rw-r--r--   0        0        0     2599 2024-05-16 16:02:52.985870 pillory-1.1.0/test_pillory.py
--rw-r--r--   0        0        0     5376 1970-01-01 00:00:00.000000 pillory-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      797 2024-05-16 16:46:40.421772 pillory-1.1.1/.circleci/config.yml
+-rw-r--r--   0        0        0       50 2024-05-16 16:46:40.421772 pillory-1.1.1/.gitignore
+-rw-r--r--   0        0        0      359 2024-05-16 16:46:40.421772 pillory-1.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     9161 2024-05-16 16:46:40.421772 pillory-1.1.1/LICENSE
+-rw-r--r--   0        0        0      354 2024-05-16 16:46:40.421772 pillory-1.1.1/Makefile
+-rw-r--r--   0        0        0     4793 2024-05-16 16:46:40.421772 pillory-1.1.1/README.md
+-rw-r--r--   0        0        0     1372 2024-05-16 16:46:40.421772 pillory-1.1.1/dev-requirements.txt
+-rw-r--r--   0        0        0       41 2024-05-16 16:46:40.421772 pillory-1.1.1/example/__init__.py
+-rw-r--r--   0        0        0      311 2024-05-16 16:46:40.421772 pillory-1.1.1/example/definition.py
+-rw-r--r--   0        0        0      180 2024-05-16 16:46:40.421772 pillory-1.1.1/example/empty/README.txt
+-rw-r--r--   0        0        0      649 2024-05-16 16:46:40.421772 pillory-1.1.1/example/test_use.py
+-rw-r--r--   0        0        0      222 2024-05-16 16:46:40.421772 pillory-1.1.1/example/use.py
+-rwxr-xr-x   0        0        0     8702 2024-05-16 16:46:40.421772 pillory-1.1.1/pillory.py
+-rw-r--r--   0        0        0     1093 2024-05-16 16:46:40.421772 pillory-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1245 2024-05-16 16:46:40.421772 pillory-1.1.1/test_example.py
+-rw-r--r--   0        0        0     2797 2024-05-16 16:46:40.421772 pillory-1.1.1/test_pillory.py
+-rw-r--r--   0        0        0     5376 1970-01-01 00:00:00.000000 pillory-1.1.1/PKG-INFO
```

### Comparing `pillory-1.1.0/.circleci/config.yml` & `pillory-1.1.1/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `pillory-1.1.0/LICENSE` & `pillory-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pillory-1.1.0/README.md` & `pillory-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pillory-1.1.0/dev-requirements.txt` & `pillory-1.1.1/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `pillory-1.1.0/example/test_use.py` & `pillory-1.1.1/example/test_use.py`

 * *Files identical despite different names*

### Comparing `pillory-1.1.0/pillory.py` & `pillory-1.1.1/pillory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """A linter to scrutinize how you are using mocks in Python."""
 
-__version__ = "1.1.0"
+__version__ = "1.1.1"
 
 # pyright: strict
 
 import ast
 import pathlib
 import sys
 from collections.abc import Iterator
@@ -111,14 +111,17 @@
             "must be at least two parts in name, one to import and one to patch"
         )
     for path in sys_path:
         path = pathlib.Path(path)
         package_dir = path / first
         if package_dir.is_dir():
             break
+        module_file = package_dir.with_suffix(".py")
+        if module_file.exists():
+            return (str(module_file), rest)
     else:  # no break
         raise LookupError(f"import {name} not found")
     parts = rest.split(".")
     for i, part in enumerate(parts):
         next_dir = package_dir / part
         if not next_dir.is_dir():
             break
```

### Comparing `pillory-1.1.0/pyproject.toml` & `pillory-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pillory-1.1.0/test_example.py` & `pillory-1.1.1/test_example.py`

 * *Files identical despite different names*

### Comparing `pillory-1.1.0/test_pillory.py` & `pillory-1.1.1/test_pillory.py`

 * *Files 9% similar despite different names*

```diff
@@ -53,14 +53,20 @@
 
     def test_find_importable_missing(self):
         self.assertEqual(
             pillory.find_importable("example.missing", ["."]),
             ("example/__init__.py", "missing"),
         )
 
+    def test_find_importable_module(self):
+        self.assertEqual(
+            pillory.find_importable("use.do_something", ["example"]),
+            ("example/use.py", "do_something"),
+        )
+
     def test_find_module_definitions(self):
         self.assertEqual(
             list(
                 pillory.find_module_definitions(
                     cleandoc(
                         """
                         def hey():
```

### Comparing `pillory-1.1.0/PKG-INFO` & `pillory-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillory
-Version: 1.1.0
+Version: 1.1.1
 Summary: A linter to scrutinize how you are using mocks in Python.
 Author-email: Fergal Armstrong <patio.algebra0i@icloud.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: coverage~=7.5 ; extra == "dev"
 Requires-Dist: flit~=3.9 ; extra == "dev"
 Requires-Dist: pip-tools~=7.4 ; extra == "dev"
```

