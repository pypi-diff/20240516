# Comparing `tmp/prefect_shell-0.2.4.tar.gz` & `tmp/prefect_shell-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect_shell-0.2.4.tar", last modified: Fri Apr 26 15:04:12 2024, max compression
+gzip compressed data, was "prefect_shell-0.2.5.tar", last modified: Thu May 16 20:58:44 2024, max compression
```

## Comparing `prefect_shell-0.2.4.tar` & `prefect_shell-0.2.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:12.089886 prefect_shell-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-26 15:03:58.000000 prefect_shell-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-26 15:03:58.000000 prefect_shell-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8579 2024-04-26 15:04:12.089886 prefect_shell-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-04-26 15:03:58.000000 prefect_shell-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:12.085886 prefect_shell-0.2.4/prefect_shell/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-26 15:03:58.000000 prefect_shell-0.2.4/prefect_shell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-26 15:04:11.000000 prefect_shell-0.2.4/prefect_shell/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    15327 2024-04-26 15:03:58.000000 prefect_shell-0.2.4/prefect_shell/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:12.089886 prefect_shell-0.2.4/prefect_shell.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8579 2024-04-26 15:04:11.000000 prefect_shell-0.2.4/prefect_shell.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-26 15:04:12.000000 prefect_shell-0.2.4/prefect_shell.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:04:11.000000 prefect_shell-0.2.4/prefect_shell.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-26 15:04:11.000000 prefect_shell-0.2.4/prefect_shell.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-26 15:04:11.000000 prefect_shell-0.2.4/prefect_shell.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-26 15:04:11.000000 prefect_shell-0.2.4/prefect_shell.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-26 15:03:58.000000 prefect_shell-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:04:12.089886 prefect_shell-0.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:12.089886 prefect_shell-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-26 15:03:58.000000 prefect_shell-0.2.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-26 15:03:58.000000 prefect_shell-0.2.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-26 15:03:58.000000 prefect_shell-0.2.4/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (127)     8341 2024-04-26 15:03:58.000000 prefect_shell-0.2.4/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     8091 2024-04-26 15:03:58.000000 prefect_shell-0.2.4/tests/test_commands_windows.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-26 15:03:58.000000 prefect_shell-0.2.4/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:44.141058 prefect_shell-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-16 20:58:32.000000 prefect_shell-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-16 20:58:32.000000 prefect_shell-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8586 2024-05-16 20:58:44.141058 prefect_shell-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-05-16 20:58:32.000000 prefect_shell-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:44.137058 prefect_shell-0.2.5/prefect_shell/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-16 20:58:32.000000 prefect_shell-0.2.5/prefect_shell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-16 20:58:43.000000 prefect_shell-0.2.5/prefect_shell/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15327 2024-05-16 20:58:32.000000 prefect_shell-0.2.5/prefect_shell/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:44.141058 prefect_shell-0.2.5/prefect_shell.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8586 2024-05-16 20:58:43.000000 prefect_shell-0.2.5/prefect_shell.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-16 20:58:44.000000 prefect_shell-0.2.5/prefect_shell.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 20:58:43.000000 prefect_shell-0.2.5/prefect_shell.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-16 20:58:43.000000 prefect_shell-0.2.5/prefect_shell.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-16 20:58:43.000000 prefect_shell-0.2.5/prefect_shell.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-16 20:58:43.000000 prefect_shell-0.2.5/prefect_shell.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-16 20:58:32.000000 prefect_shell-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 20:58:44.141058 prefect_shell-0.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:44.141058 prefect_shell-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-16 20:58:32.000000 prefect_shell-0.2.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-16 20:58:32.000000 prefect_shell-0.2.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-16 20:58:32.000000 prefect_shell-0.2.5/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8341 2024-05-16 20:58:32.000000 prefect_shell-0.2.5/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8091 2024-05-16 20:58:32.000000 prefect_shell-0.2.5/tests/test_commands_windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-16 20:58:32.000000 prefect_shell-0.2.5/tests/test_version.py
```

### Comparing `prefect_shell-0.2.4/LICENSE` & `prefect_shell-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect_shell-0.2.4/PKG-INFO` & `prefect_shell-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-shell
-Version: 0.2.4
+Version: 0.2.5
 Summary: Prefect integrations for interacting with shell commands.
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-shell
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: prefect>=2.14.10
+Requires-Dist: prefect<3.0.0,>=2.14.10
 Provides-Extra: dev
 Requires-Dist: aiohttp; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
```

### Comparing `prefect_shell-0.2.4/README.md` & `prefect_shell-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `prefect_shell-0.2.4/prefect_shell/commands.py` & `prefect_shell-0.2.5/prefect_shell/commands.py`

 * *Files identical despite different names*

### Comparing `prefect_shell-0.2.4/prefect_shell.egg-info/PKG-INFO` & `prefect_shell-0.2.5/prefect_shell.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-shell
-Version: 0.2.4
+Version: 0.2.5
 Summary: Prefect integrations for interacting with shell commands.
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-shell
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: prefect>=2.14.10
+Requires-Dist: prefect<3.0.0,>=2.14.10
 Provides-Extra: dev
 Requires-Dist: aiohttp; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
```

### Comparing `prefect_shell-0.2.4/pyproject.toml` & `prefect_shell-0.2.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Topic :: Software Development :: Libraries",
 ]
-dependencies = ["prefect>=2.14.10"]
+dependencies = ["prefect>=2.14.10, < 3.0.0"]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = [
   "aiohttp",
   "coverage",
   "interrogate",
```

### Comparing `prefect_shell-0.2.4/tests/conftest.py` & `prefect_shell-0.2.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `prefect_shell-0.2.4/tests/test_block_standards.py` & `prefect_shell-0.2.5/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect_shell-0.2.4/tests/test_commands.py` & `prefect_shell-0.2.5/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `prefect_shell-0.2.4/tests/test_commands_windows.py` & `prefect_shell-0.2.5/tests/test_commands_windows.py`

 * *Files identical despite different names*

