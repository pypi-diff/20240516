# Comparing `tmp/glbuild-0.1.0.tar.gz` & `tmp/glbuild-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glbuild-0.1.0.tar", max compression
+gzip compressed data, was "glbuild-0.1.1.tar", max compression
```

## Comparing `glbuild-0.1.0.tar` & `glbuild-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,12 @@
--rw-r--r--   0        0        0     1071 2024-05-15 00:09:24.017194 glbuild-0.1.0/LICENSE
--rw-r--r--   0        0        0      805 2024-05-15 00:09:24.017194 glbuild-0.1.0/README.md
--rw-r--r--   0        0        0       45 2024-05-15 00:09:24.017194 glbuild-0.1.0/glbuild/__init__.py
--rw-r--r--   0        0        0      126 2024-05-15 00:09:24.017194 glbuild-0.1.0/glbuild/glbuild.py
--rw-r--r--   0        0        0      715 2024-05-15 00:09:24.018194 glbuild-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1534 1970-01-01 00:00:00.000000 glbuild-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-16 15:41:26.587217 glbuild-0.1.1/LICENSE
+-rw-r--r--   0        0        0      826 2024-05-16 15:41:26.587217 glbuild-0.1.1/README.md
+-rw-r--r--   0        0        0       77 2024-05-16 15:41:26.587217 glbuild-0.1.1/glbuild/__init__.py
+-rw-r--r--   0        0        0       39 2024-05-16 15:41:26.587217 glbuild-0.1.1/glbuild/collector/__init__.py
+-rw-r--r--   0        0        0     1082 2024-05-16 15:41:26.587217 glbuild-0.1.1/glbuild/collector/progress.py
+-rw-r--r--   0        0        0      124 2024-05-16 15:41:26.587217 glbuild-0.1.1/glbuild/constants.py
+-rw-r--r--   0        0        0     6758 2024-05-16 15:41:26.587217 glbuild-0.1.1/glbuild/glbuild.py
+-rw-r--r--   0        0        0       23 2024-05-16 15:41:26.587217 glbuild-0.1.1/glbuild/utils/__init__.py
+-rw-r--r--   0        0        0    32235 2024-05-16 15:41:26.588217 glbuild-0.1.1/glbuild/utils/tempfile.py
+-rw-r--r--   0        0        0     1733 2024-05-16 15:41:26.588217 glbuild-0.1.1/glbuild/utils/utils.py
+-rw-r--r--   0        0        0      844 2024-05-16 15:41:26.588217 glbuild-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1695 1970-01-01 00:00:00.000000 glbuild-0.1.1/PKG-INFO
```

### Comparing `glbuild-0.1.0/LICENSE` & `glbuild-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `glbuild-0.1.0/README.md` & `glbuild-0.1.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -34,23 +34,23 @@
 >```bash
 >pip install glbuild
 >```
 
 Use in a Python script as follows:
 
 ```python
-from glbuild import GitlabBuild
+import glbuild
 
-glb = GitLabBuild(host="https://gitlab.com", token="***")
+glb = glbuild.GitLabBuild(base_url="https://gitlab.com", token="******", projects=[1538, 5427])
 
-glb.get(project=[14, 31], path="./data/")
+glb.get(datapath="./data")
 ```
 
 Use in a Bash command line as follows:
 
 ```bash
-glbuild init --host=https://gitlab.com --token=***
+glbuild init --base_url=https://gitlab.com --token=****** --projects=1538,5427
 ```
 
 ```bash
-glbuild get --project=14,31 --path=./data/
+glbuild get --datapath=./data
 ```
```

### Comparing `glbuild-0.1.0/pyproject.toml` & `glbuild-0.1.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,36 @@
+[build-system]
+requires = [ "poetry-core",]
+build-backend = "poetry.core.masonry.api"
+
 [tool.poetry]
 name = "glbuild"
-version = "0.1.0"
+version = "0.1.1"
 description = "Gitlab build jobs data collector. CLI tool and Python package."
-authors = ["Henri Aïdasso <ahenrij@gmail.com>"]
+authors = [ "Henri Aïdasso <ahenrij@gmail.com>",]
 license = "LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 click = "^8.1.7"
 pydantic = "^2.7.1"
 pydantic-settings = "^2.2.1"
 tqdm = "^4.66.4"
 python-gitlab = "^4.5.0"
-
+pandas = "^2.2.2"
+requests = "^2.31.0"
+types-requests = "^2.31.0.20240406"
 
 [tool.poetry.group.dev.dependencies]
-prospector = {extras = ["with_everything"], version = "^1.3.1"}
 pytest = "^8.2.0"
 pytest-cov = "^5.0.0"
 pytest-mock = "^3.14.0"
 pytest-datadir = "^1.5.0"
 pytest-timeout = "^2.3.1"
 pre-commit = "^3.7.1"
 black = "^24.4.2"
+fire = "^0.6.0"
 
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry.group.dev.dependencies.prospector]
+extras = [ "with_everything",]
+version = "^1.3.1"
```

