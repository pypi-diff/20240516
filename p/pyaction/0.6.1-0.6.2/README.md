# Comparing `tmp/pyaction-0.6.1.tar.gz` & `tmp/pyaction-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaction-0.6.1.tar", last modified: Sat May 11 17:16:23 2024, max compression
+gzip compressed data, was "pyaction-0.6.2.tar", last modified: Thu May 16 12:11:06 2024, max compression
```

## Comparing `pyaction-0.6.1.tar` & `pyaction-0.6.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:16:23.652339 pyaction-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-11 17:16:19.000000 pyaction-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-11 17:16:19.000000 pyaction-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-05-11 17:16:23.652339 pyaction-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-11 17:16:19.000000 pyaction-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:16:23.648339 pyaction-0.6.1/pyaction/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-11 17:16:19.000000 pyaction-0.6.1/pyaction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-11 17:16:19.000000 pyaction-0.6.1/pyaction/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-11 17:16:19.000000 pyaction-0.6.1/pyaction/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-11 17:16:19.000000 pyaction-0.6.1/pyaction/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-11 17:16:19.000000 pyaction-0.6.1/pyaction/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-11 17:16:19.000000 pyaction-0.6.1/pyaction/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:16:23.652339 pyaction-0.6.1/pyaction/issues/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-11 17:16:19.000000 pyaction-0.6.1/pyaction/issues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-11 17:16:19.000000 pyaction-0.6.1/pyaction/issues/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-11 17:16:19.000000 pyaction-0.6.1/pyaction/issues/rendering.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-11 17:16:19.000000 pyaction-0.6.1/pyaction/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:16:23.652339 pyaction-0.6.1/pyaction/template/
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-11 17:16:19.000000 pyaction-0.6.1/pyaction/template/copier.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:16:23.652339 pyaction-0.6.1/pyaction/template/{{action_slug}}/
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-11 17:16:19.000000 pyaction-0.6.1/pyaction/template/{{action_slug}}/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-11 17:16:19.000000 pyaction-0.6.1/pyaction/template/{{action_slug}}/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-11 17:16:19.000000 pyaction-0.6.1/pyaction/template/{{action_slug}}/Dockerfile.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-11 17:16:19.000000 pyaction-0.6.1/pyaction/template/{{action_slug}}/README.md.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-11 17:16:19.000000 pyaction-0.6.1/pyaction/template/{{action_slug}}/action.yml.jinja
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-11 17:16:19.000000 pyaction-0.6.1/pyaction/template/{{action_slug}}/main.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-11 17:16:19.000000 pyaction-0.6.1/pyaction/template/{{action_slug}}/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:16:23.648339 pyaction-0.6.1/pyaction/template/{{action_slug}}/{% if include_cicd_testing %}.github{% endif %}/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:16:23.652339 pyaction-0.6.1/pyaction/template/{{action_slug}}/{% if include_cicd_testing %}.github{% endif %}/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-11 17:16:19.000000 pyaction-0.6.1/pyaction/template/{{action_slug}}/{% if include_cicd_testing %}.github{% endif %}/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-11 17:16:19.000000 pyaction-0.6.1/pyaction/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-11 17:16:19.000000 pyaction-0.6.1/pyaction/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:16:23.652339 pyaction-0.6.1/pyaction.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-05-11 17:16:23.000000 pyaction-0.6.1/pyaction.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-11 17:16:23.000000 pyaction-0.6.1/pyaction.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 17:16:23.000000 pyaction-0.6.1/pyaction.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-11 17:16:23.000000 pyaction-0.6.1/pyaction.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-11 17:16:23.000000 pyaction-0.6.1/pyaction.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-11 17:16:23.000000 pyaction-0.6.1/pyaction.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-11 17:16:19.000000 pyaction-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 17:16:23.652339 pyaction-0.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:11:06.115224 pyaction-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-16 12:11:01.000000 pyaction-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-16 12:11:01.000000 pyaction-0.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-05-16 12:11:06.115224 pyaction-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-16 12:11:01.000000 pyaction-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:11:06.111225 pyaction-0.6.2/pyaction/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-16 12:11:01.000000 pyaction-0.6.2/pyaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-16 12:11:01.000000 pyaction-0.6.2/pyaction/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-16 12:11:01.000000 pyaction-0.6.2/pyaction/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-16 12:11:01.000000 pyaction-0.6.2/pyaction/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-16 12:11:01.000000 pyaction-0.6.2/pyaction/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-16 12:11:01.000000 pyaction-0.6.2/pyaction/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:11:06.111225 pyaction-0.6.2/pyaction/issues/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-16 12:11:01.000000 pyaction-0.6.2/pyaction/issues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-16 12:11:01.000000 pyaction-0.6.2/pyaction/issues/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-16 12:11:01.000000 pyaction-0.6.2/pyaction/issues/rendering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-16 12:11:01.000000 pyaction-0.6.2/pyaction/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:11:06.111225 pyaction-0.6.2/pyaction/template/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-16 12:11:01.000000 pyaction-0.6.2/pyaction/template/copier.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:11:06.115224 pyaction-0.6.2/pyaction/template/{{action_slug}}/
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-16 12:11:01.000000 pyaction-0.6.2/pyaction/template/{{action_slug}}/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-16 12:11:01.000000 pyaction-0.6.2/pyaction/template/{{action_slug}}/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-16 12:11:01.000000 pyaction-0.6.2/pyaction/template/{{action_slug}}/Dockerfile.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-16 12:11:01.000000 pyaction-0.6.2/pyaction/template/{{action_slug}}/README.md.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-16 12:11:01.000000 pyaction-0.6.2/pyaction/template/{{action_slug}}/action.yml.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-16 12:11:01.000000 pyaction-0.6.2/pyaction/template/{{action_slug}}/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-16 12:11:01.000000 pyaction-0.6.2/pyaction/template/{{action_slug}}/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:11:06.107225 pyaction-0.6.2/pyaction/template/{{action_slug}}/{% if include_cicd_testing %}.github{% endif %}/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:11:06.115224 pyaction-0.6.2/pyaction/template/{{action_slug}}/{% if include_cicd_testing %}.github{% endif %}/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-16 12:11:01.000000 pyaction-0.6.2/pyaction/template/{{action_slug}}/{% if include_cicd_testing %}.github{% endif %}/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-16 12:11:01.000000 pyaction-0.6.2/pyaction/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-16 12:11:01.000000 pyaction-0.6.2/pyaction/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:11:06.115224 pyaction-0.6.2/pyaction.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-05-16 12:11:06.000000 pyaction-0.6.2/pyaction.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-16 12:11:06.000000 pyaction-0.6.2/pyaction.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 12:11:06.000000 pyaction-0.6.2/pyaction.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-16 12:11:06.000000 pyaction-0.6.2/pyaction.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-16 12:11:06.000000 pyaction-0.6.2/pyaction.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-16 12:11:06.000000 pyaction-0.6.2/pyaction.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-16 12:11:01.000000 pyaction-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 12:11:06.115224 pyaction-0.6.2/setup.cfg
```

### Comparing `pyaction-0.6.1/LICENSE` & `pyaction-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaction-0.6.1/PKG-INFO` & `pyaction-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaction
-Version: 0.6.1
+Version: 0.6.2
 Summary: Create GitHub Actions using Python
 Author-email: Sadra Yahyapour <lnxpylnxpy@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Sadra Yahyapour
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyaction-0.6.1/README.md` & `pyaction-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `pyaction-0.6.1/pyaction/cli.py` & `pyaction-0.6.2/pyaction/cli.py`

 * *Files identical despite different names*

### Comparing `pyaction-0.6.1/pyaction/consts.py` & `pyaction-0.6.2/pyaction/consts.py`

 * *Files 22% similar despite different names*

```diff
@@ -24,7 +24,16 @@
 
 # path to the copier template
 TEMPLATE_PATH = os.path.join(BASE_URL, "template")
 
 
 # GitHub Action's workflow output environment variable
 GITHUB_OUTPUT = os.environ.get("GITHUB_OUTPUT", sys.stdout)
+
+# Multi-line format
+DELIMITER = "EOF"
+
+MULTILINE_OUTPUT = f"""
+{{variable}}<<{DELIMITER}
+{{value}}
+{DELIMITER}
+"""
```

### Comparing `pyaction-0.6.1/pyaction/io.py` & `pyaction-0.6.2/pyaction/io.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import os
 from contextlib import nullcontext
 from io import TextIOWrapper
 
-from pyaction.consts import GITHUB_OUTPUT
+from pyaction.consts import GITHUB_OUTPUT, MULTILINE_OUTPUT
 from pyaction.exceptions import WorkflowParameterNotFound
 
 
 def write(context: dict[str, str], stream: str | TextIOWrapper = GITHUB_OUTPUT) -> None:
     """writes the key(s) (as variables) and value(s) (as values) into the output stream
 
     Args:
@@ -16,15 +16,18 @@
         stream (str, TextIOWrapper): output stream (set to STDOUT locally, but `GITHUB_OUTPUT` on production)
     """
 
     with nullcontext(stream) if isinstance(stream, TextIOWrapper) else open(
         stream, "w+"
     ) as streamline:
         for var, val in context.items():
-            streamline.write(f"{var}={val}\r\n")
+            if "\n" in val:
+                streamline.write(MULTILINE_OUTPUT.format(variable=var, value=val))
+            else:
+                streamline.write(f"{var}={val}\r\n")
 
 
 def read(param: str) -> str | int | bool | None:
     """reads a parameter from the inputs
 
     Args:
         param (str): parameter name
```

### Comparing `pyaction-0.6.1/pyaction/issues/connector.py` & `pyaction-0.6.2/pyaction/issues/connector.py`

 * *Files identical despite different names*

### Comparing `pyaction-0.6.1/pyaction/issues/rendering.py` & `pyaction-0.6.2/pyaction/issues/rendering.py`

 * *Files identical despite different names*

### Comparing `pyaction-0.6.1/pyaction/logger.py` & `pyaction-0.6.2/pyaction/logger.py`

 * *Files identical despite different names*

### Comparing `pyaction-0.6.1/pyaction/template/copier.yml` & `pyaction-0.6.2/pyaction/template/copier.yml`

 * *Files identical despite different names*

### Comparing `pyaction-0.6.1/pyaction/utils.py` & `pyaction-0.6.2/pyaction/utils.py`

 * *Files identical despite different names*

### Comparing `pyaction-0.6.1/pyaction/workflow.py` & `pyaction-0.6.2/pyaction/workflow.py`

 * *Files identical despite different names*

### Comparing `pyaction-0.6.1/pyaction.egg-info/PKG-INFO` & `pyaction-0.6.2/pyaction.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaction
-Version: 0.6.1
+Version: 0.6.2
 Summary: Create GitHub Actions using Python
 Author-email: Sadra Yahyapour <lnxpylnxpy@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Sadra Yahyapour
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyaction-0.6.1/pyaction.egg-info/SOURCES.txt` & `pyaction-0.6.2/pyaction.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyaction-0.6.1/pyproject.toml` & `pyaction-0.6.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyaction"
-version = "0.6.1"
+version = "0.6.2"
 description = "Create GitHub Actions using Python"
 authors = [{ name = "Sadra Yahyapour", email = "lnxpylnxpy@gmail.com" }]
 requires-python = ">=3.8"
 dependencies = [
     "copier >= 9.2",
     "click >= 8.1",
     "pydantic >= 2.7.0",
@@ -38,16 +38,19 @@
 dev = ["coverage", "pytest-cookies"]
 docs = ["mkdocs-material", "cairosvg", "pillow"]
 
 [project.urls]
 Documentation = "https://pyaction.imsadra.me"
 Repository = "https://github.com/lnxpy/pyaction"
 
+[tool.setuptools.packages.find]
+exclude = ["test*"]
+
 [tool.bumpversion]
-current_version = "0.6.1"
+current_version = "0.6.2"
 commit = "true"
 tag = "true"
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 
 [[tool.bumpversion.files]]
```

