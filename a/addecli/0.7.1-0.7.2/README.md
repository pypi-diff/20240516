# Comparing `tmp/addecli-0.7.1.tar.gz` & `tmp/addecli-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "addecli-0.7.1.tar", last modified: Thu May 16 15:37:27 2024, max compression
+gzip compressed data, was "addecli-0.7.2.tar", last modified: Thu May 16 15:41:41 2024, max compression
```

## Comparing `addecli-0.7.1.tar` & `addecli-0.7.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0       10 2024-05-16 15:37:19.021176 addecli-0.7.1/README.md
--rw-r--r--   0        0        0       10 2024-05-16 15:37:19.021176 addecli-0.7.1/README.md
--rw-r--r--   0        0        0      643 2024-05-16 15:37:27.341194 addecli-0.7.1/pyproject.toml
--rw-r--r--   0        0        0       74 2024-05-16 15:37:19.021176 addecli-0.7.1/src/addecli/__main__.py
--rw-r--r--   0        0        0      364 2024-05-16 15:37:19.021176 addecli-0.7.1/src/addecli/cli_commands.py
--rw-r--r--   0        0        0     4633 2024-05-16 15:37:19.021176 addecli-0.7.1/src/addecli/create.py
--rw-r--r--   0        0        0     3181 2024-05-16 15:37:19.021176 addecli-0.7.1/src/addecli/init_project/.gitignore
--rw-r--r--   0        0        0     1353 2024-05-16 15:37:19.021176 addecli-0.7.1/src/addecli/init_project/.pre-commit-config.yaml
--rw-r--r--   0        0        0       58 2024-05-16 15:37:19.021176 addecli-0.7.1/src/addecli/init_project/conftest.py
--rw-r--r--   0        0        0      757 2024-05-16 15:37:19.021176 addecli-0.7.1/src/addecli/init_project/log-config.yml
--rw-r--r--   0        0        0     4726 2024-05-16 15:37:19.021176 addecli-0.7.1/src/addecli/init_project/scripts/create/__main__.py
--rw-r--r--   0        0        0      256 2024-05-16 15:37:19.021176 addecli-0.7.1/src/addecli/init_project/src/config.py
--rw-r--r--   0        0        0      775 2024-05-16 15:37:19.021176 addecli-0.7.1/src/addecli/init_project/src/main/app/__init__.py
--rw-r--r--   0        0        0      171 2024-05-16 15:37:19.021176 addecli-0.7.1/src/addecli/init_project/src/metadata/__init__.py
--rw-r--r--   0        0        0      407 2024-05-16 15:37:19.021176 addecli-0.7.1/src/addecli/init_project/src/metadata/_extras.py
--rw-r--r--   0        0        0      260 1970-01-01 00:00:00.000000 addecli-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0       10 2024-05-16 15:41:34.008109 addecli-0.7.2/README.md
+-rw-r--r--   0        0        0       10 2024-05-16 15:41:34.008109 addecli-0.7.2/README.md
+-rw-r--r--   0        0        0      643 2024-05-16 15:41:41.024180 addecli-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0       74 2024-05-16 15:41:34.008109 addecli-0.7.2/src/addecli/__main__.py
+-rw-r--r--   0        0        0      364 2024-05-16 15:41:34.008109 addecli-0.7.2/src/addecli/cli_commands.py
+-rw-r--r--   0        0        0     4633 2024-05-16 15:41:34.008109 addecli-0.7.2/src/addecli/create.py
+-rw-r--r--   0        0        0     3181 2024-05-16 15:41:34.008109 addecli-0.7.2/src/addecli/init_project/.gitignore
+-rw-r--r--   0        0        0     1353 2024-05-16 15:41:34.008109 addecli-0.7.2/src/addecli/init_project/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       58 2024-05-16 15:41:34.008109 addecli-0.7.2/src/addecli/init_project/conftest.py
+-rw-r--r--   0        0        0      757 2024-05-16 15:41:34.008109 addecli-0.7.2/src/addecli/init_project/log-config.yml
+-rw-r--r--   0        0        0     4726 2024-05-16 15:41:34.008109 addecli-0.7.2/src/addecli/init_project/scripts/create/__main__.py
+-rw-r--r--   0        0        0      256 2024-05-16 15:41:34.008109 addecli-0.7.2/src/addecli/init_project/src/config.py
+-rw-r--r--   0        0        0      775 2024-05-16 15:41:34.012109 addecli-0.7.2/src/addecli/init_project/src/main/app/__init__.py
+-rw-r--r--   0        0        0      171 2024-05-16 15:41:34.012109 addecli-0.7.2/src/addecli/init_project/src/metadata/__init__.py
+-rw-r--r--   0        0        0      407 2024-05-16 15:41:34.012109 addecli-0.7.2/src/addecli/init_project/src/metadata/_extras.py
+-rw-r--r--   0        0        0      260 1970-01-01 00:00:00.000000 addecli-0.7.2/PKG-INFO
```

### Comparing `addecli-0.7.1/pyproject.toml` & `addecli-0.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "addecli"
-version = "0.7.1"
+version = "0.7.2"
 description = "Default template for PDM package"
 authors = [
     { name = "Victor", email = "victordeonroyale@gmail.com" },
 ]
 dependencies = [
     "typer>=0.12.3",
 ]
```

### Comparing `addecli-0.7.1/src/addecli/create.py` & `addecli-0.7.2/src/addecli/create.py`

 * *Files identical despite different names*

### Comparing `addecli-0.7.1/src/addecli/init_project/.gitignore` & `addecli-0.7.2/src/addecli/init_project/.gitignore`

 * *Files identical despite different names*

### Comparing `addecli-0.7.1/src/addecli/init_project/.pre-commit-config.yaml` & `addecli-0.7.2/src/addecli/init_project/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `addecli-0.7.1/src/addecli/init_project/log-config.yml` & `addecli-0.7.2/src/addecli/init_project/log-config.yml`

 * *Files identical despite different names*

### Comparing `addecli-0.7.1/src/addecli/init_project/scripts/create/__main__.py` & `addecli-0.7.2/src/addecli/init_project/scripts/create/__main__.py`

 * *Files identical despite different names*

### Comparing `addecli-0.7.1/src/addecli/init_project/src/main/app/__init__.py` & `addecli-0.7.2/src/addecli/init_project/src/main/app/__init__.py`

 * *Files identical despite different names*

