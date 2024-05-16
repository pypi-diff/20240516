# Comparing `tmp/pylasu-0.7.0.tar.gz` & `tmp/pylasu-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylasu-0.7.0.tar", last modified: Tue Nov 21 08:51:41 2023, max compression
+gzip compressed data, was "/Users/alessio/projects/polyparser-python-runtime/dist/.tmp-i38dtv9l/pylasu-0.7.1.tar", last modified: Thu May 16 12:11:27 2024, max compression
```

## Comparing `pylasu-0.7.0.tar` & `pylasu-0.7.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 loradd     (501) staff       (20)        0 2023-11-21 08:51:41.365523 pylasu-0.7.0/
--rw-r--r--   0 loradd     (501) staff       (20)    11357 2023-11-20 21:27:53.000000 pylasu-0.7.0/LICENSE
--rw-r--r--   0 loradd     (501) staff       (20)       12 2023-11-20 21:27:53.000000 pylasu-0.7.0/MANIFEST.in
--rw-r--r--   0 loradd     (501) staff       (20)    15743 2023-11-21 08:51:41.365393 pylasu-0.7.0/PKG-INFO
--rw-r--r--   0 loradd     (501) staff       (20)     2041 2023-11-20 21:27:53.000000 pylasu-0.7.0/README.md
-drwxr-xr-x   0 loradd     (501) staff       (20)        0 2023-11-21 08:51:41.357030 pylasu-0.7.0/pylasu/
-drwxr-xr-x   0 loradd     (501) staff       (20)        0 2023-11-21 08:51:41.358555 pylasu-0.7.0/pylasu/StrumentaLanguageSupport/
--rw-r--r--   0 loradd     (501) staff       (20)     8555 2023-11-20 21:27:53.000000 pylasu-0.7.0/pylasu/StrumentaLanguageSupport/StrumentaLanguageSupport.py
--rw-r--r--   0 loradd     (501) staff       (20)     1772 2023-11-20 21:27:53.000000 pylasu-0.7.0/pylasu/StrumentaLanguageSupport/__init__.py
--rw-r--r--   0 loradd     (501) staff       (20)        0 2023-11-20 21:27:53.000000 pylasu-0.7.0/pylasu/__init__.py
--rw-r--r--   0 loradd     (501) staff       (20)       22 2023-11-21 08:47:45.000000 pylasu-0.7.0/pylasu/__version__.py
--rw-r--r--   0 loradd     (501) staff       (20)     2201 2023-11-20 21:33:57.000000 pylasu-0.7.0/pylasu/astruntime.py
-drwxr-xr-x   0 loradd     (501) staff       (20)        0 2023-11-21 08:51:41.359515 pylasu-0.7.0/pylasu/emf/
--rw-r--r--   0 loradd     (501) staff       (20)       84 2023-11-20 21:27:53.000000 pylasu-0.7.0/pylasu/emf/__init__.py
--rw-r--r--   0 loradd     (501) staff       (20)     7089 2023-11-20 21:27:53.000000 pylasu-0.7.0/pylasu/emf/metamodel_builder.py
--rw-r--r--   0 loradd     (501) staff       (20)     2041 2023-11-20 21:27:53.000000 pylasu-0.7.0/pylasu/emf/model.py
-drwxr-xr-x   0 loradd     (501) staff       (20)        0 2023-11-21 08:51:41.359829 pylasu-0.7.0/pylasu/mapping/
--rw-r--r--   0 loradd     (501) staff       (20)        0 2023-11-20 21:27:53.000000 pylasu-0.7.0/pylasu/mapping/__init__.py
--rw-r--r--   0 loradd     (501) staff       (20)     1489 2023-11-20 21:27:53.000000 pylasu-0.7.0/pylasu/mapping/parse_tree_to_ast_transformer.py
-drwxr-xr-x   0 loradd     (501) staff       (20)        0 2023-11-21 08:51:41.361499 pylasu-0.7.0/pylasu/model/
--rw-r--r--   0 loradd     (501) staff       (20)      322 2023-11-20 21:27:53.000000 pylasu-0.7.0/pylasu/model/__init__.py
--rw-r--r--   0 loradd     (501) staff       (20)      634 2023-11-20 21:27:53.000000 pylasu-0.7.0/pylasu/model/errors.py
--rw-r--r--   0 loradd     (501) staff       (20)     5938 2023-11-20 21:27:53.000000 pylasu-0.7.0/pylasu/model/model.py
--rw-r--r--   0 loradd     (501) staff       (20)     2140 2023-11-20 21:27:53.000000 pylasu-0.7.0/pylasu/model/naming.py
--rw-r--r--   0 loradd     (501) staff       (20)     3081 2023-11-20 21:27:53.000000 pylasu-0.7.0/pylasu/model/position.py
--rw-r--r--   0 loradd     (501) staff       (20)     2226 2023-11-20 21:27:53.000000 pylasu-0.7.0/pylasu/model/processing.py
--rw-r--r--   0 loradd     (501) staff       (20)      378 2023-11-20 21:27:53.000000 pylasu-0.7.0/pylasu/model/reflection.py
--rw-r--r--   0 loradd     (501) staff       (20)     2689 2023-11-20 21:27:53.000000 pylasu-0.7.0/pylasu/model/traversing.py
-drwxr-xr-x   0 loradd     (501) staff       (20)        0 2023-11-21 08:51:41.362027 pylasu-0.7.0/pylasu/parsing/
--rw-r--r--   0 loradd     (501) staff       (20)        0 2023-11-20 21:27:53.000000 pylasu-0.7.0/pylasu/parsing/__init__.py
--rw-r--r--   0 loradd     (501) staff       (20)     6250 2023-11-20 21:27:53.000000 pylasu-0.7.0/pylasu/parsing/parse_tree.py
--rw-r--r--   0 loradd     (501) staff       (20)     1045 2023-11-20 21:27:53.000000 pylasu-0.7.0/pylasu/parsing/results.py
-drwxr-xr-x   0 loradd     (501) staff       (20)        0 2023-11-21 08:51:41.362790 pylasu-0.7.0/pylasu/playground/
--rw-r--r--   0 loradd     (501) staff       (20)      147 2023-11-20 21:27:53.000000 pylasu-0.7.0/pylasu/playground/__init__.py
--rw-r--r--   0 loradd     (501) staff       (20)     1476 2023-11-20 21:27:53.000000 pylasu-0.7.0/pylasu/playground/transpilation_trace.py
--rw-r--r--   0 loradd     (501) staff       (20)     2175 2023-11-20 21:27:53.000000 pylasu-0.7.0/pylasu/playground/transpilation_trace_ecore.py
-drwxr-xr-x   0 loradd     (501) staff       (20)        0 2023-11-21 08:51:41.363195 pylasu-0.7.0/pylasu/reflection/
--rw-r--r--   0 loradd     (501) staff       (20)       39 2023-11-20 21:27:53.000000 pylasu-0.7.0/pylasu/reflection/__init__.py
--rw-r--r--   0 loradd     (501) staff       (20)     1218 2023-11-20 21:27:53.000000 pylasu-0.7.0/pylasu/reflection/reflection.py
--rw-r--r--   0 loradd     (501) staff       (20)      412 2023-11-20 21:27:53.000000 pylasu-0.7.0/pylasu/support.py
-drwxr-xr-x   0 loradd     (501) staff       (20)        0 2023-11-21 08:51:41.363442 pylasu-0.7.0/pylasu/testing/
--rw-r--r--   0 loradd     (501) staff       (20)        0 2023-11-20 21:27:53.000000 pylasu-0.7.0/pylasu/testing/__init__.py
--rw-r--r--   0 loradd     (501) staff       (20)     3423 2023-11-20 21:27:53.000000 pylasu-0.7.0/pylasu/testing/testing.py
-drwxr-xr-x   0 loradd     (501) staff       (20)        0 2023-11-21 08:51:41.364001 pylasu-0.7.0/pylasu/transformation/
--rw-r--r--   0 loradd     (501) staff       (20)        0 2023-11-20 21:27:53.000000 pylasu-0.7.0/pylasu/transformation/__init__.py
--rw-r--r--   0 loradd     (501) staff       (20)      244 2023-11-20 21:27:53.000000 pylasu-0.7.0/pylasu/transformation/generic_nodes.py
--rw-r--r--   0 loradd     (501) staff       (20)     9529 2023-11-20 21:27:53.000000 pylasu-0.7.0/pylasu/transformation/transformation.py
-drwxr-xr-x   0 loradd     (501) staff       (20)        0 2023-11-21 08:51:41.364557 pylasu-0.7.0/pylasu/validation/
--rw-r--r--   0 loradd     (501) staff       (20)       64 2023-11-20 21:27:53.000000 pylasu-0.7.0/pylasu/validation/__init__.py
--rw-r--r--   0 loradd     (501) staff       (20)     1033 2023-11-20 21:31:53.000000 pylasu-0.7.0/pylasu/validation/validation.py
-drwxr-xr-x   0 loradd     (501) staff       (20)        0 2023-11-21 08:51:41.364980 pylasu-0.7.0/pylasu.egg-info/
--rw-r--r--   0 loradd     (501) staff       (20)    15743 2023-11-21 08:51:41.000000 pylasu-0.7.0/pylasu.egg-info/PKG-INFO
--rw-r--r--   0 loradd     (501) staff       (20)     1235 2023-11-21 08:51:41.000000 pylasu-0.7.0/pylasu.egg-info/SOURCES.txt
--rw-r--r--   0 loradd     (501) staff       (20)        1 2023-11-21 08:51:41.000000 pylasu-0.7.0/pylasu.egg-info/dependency_links.txt
--rw-r--r--   0 loradd     (501) staff       (20)       17 2023-11-21 08:51:41.000000 pylasu-0.7.0/pylasu.egg-info/requires.txt
--rw-r--r--   0 loradd     (501) staff       (20)       13 2023-11-21 08:51:41.000000 pylasu-0.7.0/pylasu.egg-info/top_level.txt
--rw-r--r--   0 loradd     (501) staff       (20)      842 2023-11-20 21:27:53.000000 pylasu-0.7.0/pyproject.toml
--rw-r--r--   0 loradd     (501) staff       (20)      213 2023-11-21 08:51:41.365795 pylasu-0.7.0/setup.cfg
--rw-r--r--   0 loradd     (501) staff       (20)      483 2023-11-20 21:27:53.000000 pylasu-0.7.0/setup.py
+drwxr-xr-x   0 alessio    (501) staff       (20)        0 2024-05-16 12:11:27.515501 pylasu-0.7.1/
+-rw-r--r--   0 alessio    (501) staff       (20)    11357 2022-05-12 07:18:54.000000 pylasu-0.7.1/LICENSE
+-rw-r--r--   0 alessio    (501) staff       (20)       12 2023-09-06 13:52:38.000000 pylasu-0.7.1/MANIFEST.in
+-rw-r--r--   0 alessio    (501) staff       (20)    15996 2024-05-16 12:11:27.515425 pylasu-0.7.1/PKG-INFO
+-rw-r--r--   0 alessio    (501) staff       (20)     2294 2024-05-16 12:11:03.000000 pylasu-0.7.1/README.md
+drwxr-xr-x   0 alessio    (501) staff       (20)        0 2024-05-16 12:11:27.506678 pylasu-0.7.1/pylasu/
+drwxr-xr-x   0 alessio    (501) staff       (20)        0 2024-05-16 12:11:27.508128 pylasu-0.7.1/pylasu/StrumentaLanguageSupport/
+-rw-r--r--   0 alessio    (501) staff       (20)     8555 2022-09-20 11:57:20.000000 pylasu-0.7.1/pylasu/StrumentaLanguageSupport/StrumentaLanguageSupport.py
+-rw-r--r--   0 alessio    (501) staff       (20)     1772 2022-09-22 13:40:28.000000 pylasu-0.7.1/pylasu/StrumentaLanguageSupport/__init__.py
+-rw-r--r--   0 alessio    (501) staff       (20)        0 2022-05-09 09:13:43.000000 pylasu-0.7.1/pylasu/__init__.py
+-rw-r--r--   0 alessio    (501) staff       (20)       22 2024-05-16 11:50:49.000000 pylasu-0.7.1/pylasu/__version__.py
+-rw-r--r--   0 alessio    (501) staff       (20)     2201 2023-11-21 09:00:10.000000 pylasu-0.7.1/pylasu/astruntime.py
+drwxr-xr-x   0 alessio    (501) staff       (20)        0 2024-05-16 12:11:27.508866 pylasu-0.7.1/pylasu/emf/
+-rw-r--r--   0 alessio    (501) staff       (20)       84 2022-09-19 15:32:55.000000 pylasu-0.7.1/pylasu/emf/__init__.py
+-rw-r--r--   0 alessio    (501) staff       (20)     7089 2023-05-02 07:50:40.000000 pylasu-0.7.1/pylasu/emf/metamodel_builder.py
+-rw-r--r--   0 alessio    (501) staff       (20)     2041 2023-09-05 12:19:01.000000 pylasu-0.7.1/pylasu/emf/model.py
+drwxr-xr-x   0 alessio    (501) staff       (20)        0 2024-05-16 12:11:27.509274 pylasu-0.7.1/pylasu/mapping/
+-rw-r--r--   0 alessio    (501) staff       (20)        0 2023-02-14 16:54:28.000000 pylasu-0.7.1/pylasu/mapping/__init__.py
+-rw-r--r--   0 alessio    (501) staff       (20)     1489 2023-02-14 16:54:28.000000 pylasu-0.7.1/pylasu/mapping/parse_tree_to_ast_transformer.py
+drwxr-xr-x   0 alessio    (501) staff       (20)        0 2024-05-16 12:11:27.511125 pylasu-0.7.1/pylasu/model/
+-rw-r--r--   0 alessio    (501) staff       (20)      322 2023-05-02 07:57:00.000000 pylasu-0.7.1/pylasu/model/__init__.py
+-rw-r--r--   0 alessio    (501) staff       (20)      634 2023-02-14 16:54:28.000000 pylasu-0.7.1/pylasu/model/errors.py
+-rw-r--r--   0 alessio    (501) staff       (20)     6278 2024-01-29 12:15:29.000000 pylasu-0.7.1/pylasu/model/model.py
+-rw-r--r--   0 alessio    (501) staff       (20)     2140 2023-02-14 16:54:28.000000 pylasu-0.7.1/pylasu/model/naming.py
+-rw-r--r--   0 alessio    (501) staff       (20)     3081 2023-10-24 14:07:38.000000 pylasu-0.7.1/pylasu/model/position.py
+-rw-r--r--   0 alessio    (501) staff       (20)     2226 2023-09-05 12:18:28.000000 pylasu-0.7.1/pylasu/model/processing.py
+-rw-r--r--   0 alessio    (501) staff       (20)      378 2023-09-05 11:41:36.000000 pylasu-0.7.1/pylasu/model/reflection.py
+-rw-r--r--   0 alessio    (501) staff       (20)     2689 2023-02-14 16:54:28.000000 pylasu-0.7.1/pylasu/model/traversing.py
+drwxr-xr-x   0 alessio    (501) staff       (20)        0 2024-05-16 12:11:27.511758 pylasu-0.7.1/pylasu/parsing/
+-rw-r--r--   0 alessio    (501) staff       (20)        0 2022-05-09 09:13:43.000000 pylasu-0.7.1/pylasu/parsing/__init__.py
+-rw-r--r--   0 alessio    (501) staff       (20)     6356 2024-05-16 11:47:10.000000 pylasu-0.7.1/pylasu/parsing/parse_tree.py
+-rw-r--r--   0 alessio    (501) staff       (20)     1045 2023-10-10 08:11:55.000000 pylasu-0.7.1/pylasu/parsing/results.py
+drwxr-xr-x   0 alessio    (501) staff       (20)        0 2024-05-16 12:11:27.512592 pylasu-0.7.1/pylasu/playground/
+-rw-r--r--   0 alessio    (501) staff       (20)      147 2022-09-19 14:02:38.000000 pylasu-0.7.1/pylasu/playground/__init__.py
+-rw-r--r--   0 alessio    (501) staff       (20)     1476 2022-09-19 14:45:56.000000 pylasu-0.7.1/pylasu/playground/transpilation_trace.py
+-rw-r--r--   0 alessio    (501) staff       (20)     2175 2022-09-22 13:42:59.000000 pylasu-0.7.1/pylasu/playground/transpilation_trace_ecore.py
+drwxr-xr-x   0 alessio    (501) staff       (20)        0 2024-05-16 12:11:27.513101 pylasu-0.7.1/pylasu/reflection/
+-rw-r--r--   0 alessio    (501) staff       (20)       77 2024-01-29 12:15:34.000000 pylasu-0.7.1/pylasu/reflection/__init__.py
+-rw-r--r--   0 alessio    (501) staff       (20)     1218 2023-02-14 16:54:28.000000 pylasu-0.7.1/pylasu/reflection/reflection.py
+-rw-r--r--   0 alessio    (501) staff       (20)      412 2022-07-28 08:04:25.000000 pylasu-0.7.1/pylasu/support.py
+drwxr-xr-x   0 alessio    (501) staff       (20)        0 2024-05-16 12:11:27.513440 pylasu-0.7.1/pylasu/testing/
+-rw-r--r--   0 alessio    (501) staff       (20)        0 2023-02-14 16:54:28.000000 pylasu-0.7.1/pylasu/testing/__init__.py
+-rw-r--r--   0 alessio    (501) staff       (20)     3423 2023-10-10 11:44:06.000000 pylasu-0.7.1/pylasu/testing/testing.py
+drwxr-xr-x   0 alessio    (501) staff       (20)        0 2024-05-16 12:11:27.514130 pylasu-0.7.1/pylasu/transformation/
+-rw-r--r--   0 alessio    (501) staff       (20)        0 2023-02-14 16:54:28.000000 pylasu-0.7.1/pylasu/transformation/__init__.py
+-rw-r--r--   0 alessio    (501) staff       (20)      244 2023-09-05 08:14:25.000000 pylasu-0.7.1/pylasu/transformation/generic_nodes.py
+-rw-r--r--   0 alessio    (501) staff       (20)     9607 2023-12-11 10:26:10.000000 pylasu-0.7.1/pylasu/transformation/transformation.py
+drwxr-xr-x   0 alessio    (501) staff       (20)        0 2024-05-16 12:11:27.514632 pylasu-0.7.1/pylasu/validation/
+-rw-r--r--   0 alessio    (501) staff       (20)       64 2023-05-02 07:58:09.000000 pylasu-0.7.1/pylasu/validation/__init__.py
+-rw-r--r--   0 alessio    (501) staff       (20)     1033 2023-11-21 08:40:26.000000 pylasu-0.7.1/pylasu/validation/validation.py
+drwxr-xr-x   0 alessio    (501) staff       (20)        0 2024-05-16 12:11:27.514974 pylasu-0.7.1/pylasu.egg-info/
+-rw-r--r--   0 alessio    (501) staff       (20)    15996 2024-05-16 12:11:27.000000 pylasu-0.7.1/pylasu.egg-info/PKG-INFO
+-rw-r--r--   0 alessio    (501) staff       (20)     1235 2024-05-16 12:11:27.000000 pylasu-0.7.1/pylasu.egg-info/SOURCES.txt
+-rw-r--r--   0 alessio    (501) staff       (20)        1 2024-05-16 12:11:27.000000 pylasu-0.7.1/pylasu.egg-info/dependency_links.txt
+-rw-r--r--   0 alessio    (501) staff       (20)       17 2024-05-16 12:11:27.000000 pylasu-0.7.1/pylasu.egg-info/requires.txt
+-rw-r--r--   0 alessio    (501) staff       (20)       13 2024-05-16 12:11:27.000000 pylasu-0.7.1/pylasu.egg-info/top_level.txt
+-rw-r--r--   0 alessio    (501) staff       (20)      842 2023-10-10 11:52:55.000000 pylasu-0.7.1/pyproject.toml
+-rw-r--r--   0 alessio    (501) staff       (20)      213 2024-05-16 12:11:27.515894 pylasu-0.7.1/setup.cfg
+-rw-r--r--   0 alessio    (501) staff       (20)      483 2023-10-10 11:49:44.000000 pylasu-0.7.1/setup.py
```

### Comparing `pylasu-0.7.0/LICENSE` & `pylasu-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pylasu-0.7.0/PKG-INFO` & `pylasu-0.7.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylasu
-Version: 0.7.0
+Version: 0.7.1
 Summary: Pylasu is an AST Library in the StarLasu family, targeting the Python language.
 Author-email: Lorenzo Addazi <lorenzo.addazi@strumenta.com>, Alessio Stalla <alessio.stalla@strumenta.com>, Federico Tomassetti <federico@strumenta.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -232,18 +232,39 @@
 
 ## Linting
 
 ```shell
 flake8 . && flake8 tests
 ```
 
-## Packaging and distributing
+## Testing
+
+```shell
+pytest tests
+```
+
+## Packaging and Distribution
+
+Update version in `setup.cfg` and `pylasu/__version__.py` _(TODO do we need both?)_,
+commit and check that CI completes normally. 
+
+Let's ensure that we have build and twine installed:
+
+```shell
+pip install build twine
+```
+
+Then, check the project can be released by linting and running the test suite:
+
+```shell
+flake8 . && flake8 tests
+pytest tests
+```
 
-Update version in `pyproject.toml`, `setup.cfg` and `pylasu/__version__.py` _(TODO do we need all three?)_,
-commit and check that CI completes normally. Then run:
+Finally, we can run:
 
 ```shell
 rm dist/*
 python -m build
 python -m twine upload dist/*
 ```
```

### Comparing `pylasu-0.7.0/README.md` & `pylasu-0.7.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -14,18 +14,39 @@
 
 ## Linting
 
 ```shell
 flake8 . && flake8 tests
 ```
 
-## Packaging and distributing
+## Testing
 
-Update version in `pyproject.toml`, `setup.cfg` and `pylasu/__version__.py` _(TODO do we need all three?)_,
-commit and check that CI completes normally. Then run:
+```shell
+pytest tests
+```
+
+## Packaging and Distribution
+
+Update version in `setup.cfg` and `pylasu/__version__.py` _(TODO do we need both?)_,
+commit and check that CI completes normally. 
+
+Let's ensure that we have build and twine installed:
+
+```shell
+pip install build twine
+```
+
+Then, check the project can be released by linting and running the test suite:
+
+```shell
+flake8 . && flake8 tests
+pytest tests
+```
+
+Finally, we can run:
 
 ```shell
 rm dist/*
 python -m build
 python -m twine upload dist/*
 ```
```

### Comparing `pylasu-0.7.0/pylasu/StrumentaLanguageSupport/StrumentaLanguageSupport.py` & `pylasu-0.7.1/pylasu/StrumentaLanguageSupport/StrumentaLanguageSupport.py`

 * *Files identical despite different names*

### Comparing `pylasu-0.7.0/pylasu/StrumentaLanguageSupport/__init__.py` & `pylasu-0.7.1/pylasu/StrumentaLanguageSupport/__init__.py`

 * *Files identical despite different names*

### Comparing `pylasu-0.7.0/pylasu/astruntime.py` & `pylasu-0.7.1/pylasu/astruntime.py`

 * *Files identical despite different names*

### Comparing `pylasu-0.7.0/pylasu/emf/metamodel_builder.py` & `pylasu-0.7.1/pylasu/emf/metamodel_builder.py`

 * *Files identical despite different names*

### Comparing `pylasu-0.7.0/pylasu/emf/model.py` & `pylasu-0.7.1/pylasu/emf/model.py`

 * *Files identical despite different names*

### Comparing `pylasu-0.7.0/pylasu/mapping/parse_tree_to_ast_transformer.py` & `pylasu-0.7.1/pylasu/mapping/parse_tree_to_ast_transformer.py`

 * *Files identical despite different names*

### Comparing `pylasu-0.7.0/pylasu/model/errors.py` & `pylasu-0.7.1/pylasu/model/errors.py`

 * *Files identical despite different names*

### Comparing `pylasu-0.7.0/pylasu/model/model.py` & `pylasu-0.7.1/pylasu/model/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import inspect
 from abc import ABC, abstractmethod, ABCMeta
 from dataclasses import Field, MISSING, dataclass, field
 from typing import Optional, Callable, List
 
 from .position import Position, Source
 from .reflection import Multiplicity, PropertyDescription
-from ..reflection import getannotations
-from ..reflection.reflection import is_sequence_type, get_type_arguments
+from ..reflection import getannotations, get_type_arguments, is_sequence_type
 
 
 class internal_property(property):
     pass
 
 
 def internal_properties(*props: str):
@@ -173,7 +172,21 @@
     @internal_property
     def _fields(self):
         yield from (name for name, _ in self.properties)
 
     @internal_property
     def node_type(self):
         return type(self)
+
+
+def concept_of(node):
+    properties = dir(node)
+    if "__concept__" in properties:
+        node_type = node.__concept__
+    elif "node_type" in properties:
+        node_type = node.node_type
+    else:
+        node_type = type(node)
+    if isinstance(node_type, Concept):
+        return node_type
+    else:
+        raise Exception(f"Not a concept: {node_type} of {node}")
```

### Comparing `pylasu-0.7.0/pylasu/model/naming.py` & `pylasu-0.7.1/pylasu/model/naming.py`

 * *Files identical despite different names*

### Comparing `pylasu-0.7.0/pylasu/model/position.py` & `pylasu-0.7.1/pylasu/model/position.py`

 * *Files identical despite different names*

### Comparing `pylasu-0.7.0/pylasu/model/processing.py` & `pylasu-0.7.1/pylasu/model/processing.py`

 * *Files identical despite different names*

### Comparing `pylasu-0.7.0/pylasu/model/traversing.py` & `pylasu-0.7.1/pylasu/model/traversing.py`

 * *Files identical despite different names*

### Comparing `pylasu-0.7.0/pylasu/parsing/parse_tree.py` & `pylasu-0.7.1/pylasu/parsing/parse_tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,16 @@
 
 Token.start_point = property(token_start_point)
 Token.end_point = property(token_end_point)
 
 
 @extension_method(ParserRuleContext)
 def to_position(self: ParserRuleContext, source: Source = None):
-    if self.start.start_point <= self.stop.end_point:
+    # In case of an empty input, the start token will be EOF and the end token will be None
+    if self.stop and self.start.start_point <= self.stop.end_point:
         return Position(self.start.start_point, self.stop.end_point, source)
     else:
         # In case of parse errors, sometimes ANTLR inserts nodes that end before they start
         return Position(self.start.start_point, self.start.end_point, source)
 
 
 @extension_method(TerminalNode)
```

### Comparing `pylasu-0.7.0/pylasu/parsing/results.py` & `pylasu-0.7.1/pylasu/parsing/results.py`

 * *Files identical despite different names*

### Comparing `pylasu-0.7.0/pylasu/playground/transpilation_trace.py` & `pylasu-0.7.1/pylasu/playground/transpilation_trace.py`

 * *Files identical despite different names*

### Comparing `pylasu-0.7.0/pylasu/playground/transpilation_trace_ecore.py` & `pylasu-0.7.1/pylasu/playground/transpilation_trace_ecore.py`

 * *Files identical despite different names*

### Comparing `pylasu-0.7.0/pylasu/reflection/reflection.py` & `pylasu-0.7.1/pylasu/reflection/reflection.py`

 * *Files identical despite different names*

### Comparing `pylasu-0.7.0/pylasu/testing/testing.py` & `pylasu-0.7.1/pylasu/testing/testing.py`

 * *Files identical despite different names*

### Comparing `pylasu-0.7.0/pylasu/transformation/transformation.py` & `pylasu-0.7.1/pylasu/transformation/transformation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import functools
 from dataclasses import dataclass, field
 from inspect import signature
 from typing import Any, Dict, Callable, TypeVar, Generic, Optional, List, Set, Iterable, Type, Union
 
 from pylasu.model import Node, Origin
 from pylasu.model.errors import GenericErrorNode
+from pylasu.model.model import concept_of
 from pylasu.model.reflection import PropertyDescription
 from pylasu.transformation.generic_nodes import GenericNode
 from pylasu.validation import Issue, IssueSeverity
 
 Child = TypeVar('Child')
 Output = TypeVar('Output', bound=Node)
 Source = TypeVar('Source')
@@ -28,15 +29,15 @@
         return setattr(node, self.name, value)
 
 
 @dataclass
 class NodeFactory(Generic[Source, Output]):
     constructor: node_factory_constructor_type
     children: Dict[str, "ChildNodeFactory[Source, Any, Any]"] = field(default_factory=dict)
-    finalizer: Callable[[Source], None] = lambda _: None
+    finalizer: Callable[[Source], None] = field(default=lambda _: None)
 
     def with_child(
             self,
             setter: Union[Callable[[Target, Optional[Child]], None], PropertyRef],
             getter: Union[Callable[[Source], Optional[Any]], PropertyRef],
             name: Optional[str] = None,
             target_type: Optional[type] = None
@@ -100,15 +101,15 @@
             return []
         elif isinstance(source, Iterable):
             raise Exception(f"Mapping error: received collection when value was expected: {source}")
         factory = self.get_node_factory(type(source))
         if factory:
             nodes = self.make_nodes(factory, source)
             for node in nodes:
-                for pd in type(node).node_properties:
+                for pd in concept_of(node).node_properties:
                     self.process_child(source, node, pd, factory)
                 factory.finalizer(node)
                 node.parent = parent
 
         else:
             if self.allow_generic_node:
                 origin = self.as_origin(source)
@@ -130,15 +131,15 @@
             child_node_factory = factory.children[pd.name]
         else:
             child_node_factory = None
         if child_node_factory:
             if child_node_factory != NO_CHILD_NODE:
                 self.set_child(child_node_factory, source, node, pd)
         else:
-            # TODO should we support @Mapped?
+            # TODO should we support @Mapped / dot-notation?
             factory.children[child_key] = NO_CHILD_NODE
 
     def as_origin(self, source: Any) -> Optional[Origin]:
         return source if isinstance(source, Origin) else None
 
     def set_child(self, child_node_factory: ChildNodeFactory, source: Any, node: Node, pd: PropertyDescription):
         src = child_node_factory.get(self.get_source(node, source))
```

### Comparing `pylasu-0.7.0/pylasu/validation/validation.py` & `pylasu-0.7.1/pylasu/validation/validation.py`

 * *Files identical despite different names*

### Comparing `pylasu-0.7.0/pylasu.egg-info/PKG-INFO` & `pylasu-0.7.1/pylasu.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylasu
-Version: 0.7.0
+Version: 0.7.1
 Summary: Pylasu is an AST Library in the StarLasu family, targeting the Python language.
 Author-email: Lorenzo Addazi <lorenzo.addazi@strumenta.com>, Alessio Stalla <alessio.stalla@strumenta.com>, Federico Tomassetti <federico@strumenta.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -232,18 +232,39 @@
 
 ## Linting
 
 ```shell
 flake8 . && flake8 tests
 ```
 
-## Packaging and distributing
+## Testing
+
+```shell
+pytest tests
+```
+
+## Packaging and Distribution
+
+Update version in `setup.cfg` and `pylasu/__version__.py` _(TODO do we need both?)_,
+commit and check that CI completes normally. 
+
+Let's ensure that we have build and twine installed:
+
+```shell
+pip install build twine
+```
+
+Then, check the project can be released by linting and running the test suite:
+
+```shell
+flake8 . && flake8 tests
+pytest tests
+```
 
-Update version in `pyproject.toml`, `setup.cfg` and `pylasu/__version__.py` _(TODO do we need all three?)_,
-commit and check that CI completes normally. Then run:
+Finally, we can run:
 
 ```shell
 rm dist/*
 python -m build
 python -m twine upload dist/*
 ```
```

### Comparing `pylasu-0.7.0/pylasu.egg-info/SOURCES.txt` & `pylasu-0.7.1/pylasu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pylasu-0.7.0/pyproject.toml` & `pylasu-0.7.1/pyproject.toml`

 * *Files identical despite different names*

