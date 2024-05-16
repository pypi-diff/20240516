# Comparing `tmp/dsi_cocoa-0.4.0.tar.gz` & `tmp/dsi_cocoa-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsi_cocoa-0.4.0.tar", last modified: Wed May 15 20:27:22 2024, max compression
+gzip compressed data, was "dsi_cocoa-0.5.0.tar", last modified: Wed May 15 20:32:10 2024, max compression
```

## Comparing `dsi_cocoa-0.4.0.tar` & `dsi_cocoa-0.5.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:27:22.547509 dsi_cocoa-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-15 20:27:19.000000 dsi_cocoa-0.4.0/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 20:27:12.000000 dsi_cocoa-0.4.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:27:22.543509 dsi_cocoa-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:27:22.547509 dsi_cocoa-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-15 20:27:12.000000 dsi_cocoa-0.4.0/.github/workflows/main.workflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-15 20:27:12.000000 dsi_cocoa-0.4.0/.github/workflows/publish.workflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-15 20:27:12.000000 dsi_cocoa-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-15 20:27:12.000000 dsi_cocoa-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-15 20:27:22.547509 dsi_cocoa-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-05-15 20:27:12.000000 dsi_cocoa-0.4.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)       66 2024-05-15 20:27:12.000000 dsi_cocoa-0.4.0/eval-repo.sh
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-15 20:27:12.000000 dsi_cocoa-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-15 20:27:12.000000 dsi_cocoa-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-15 20:27:22.547509 dsi_cocoa-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-15 20:27:19.000000 dsi_cocoa-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:27:22.543509 dsi_cocoa-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:27:22.547509 dsi_cocoa-0.4.0/src/cocoa/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-15 20:27:19.000000 dsi_cocoa-0.4.0/src/cocoa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-15 20:27:12.000000 dsi_cocoa-0.4.0/src/cocoa/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-15 20:27:12.000000 dsi_cocoa-0.4.0/src/cocoa/evaluate_repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8865 2024-05-15 20:27:12.000000 dsi_cocoa-0.4.0/src/cocoa/linting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-15 20:27:12.000000 dsi_cocoa-0.4.0/src/cocoa/notebooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-05-15 20:27:12.000000 dsi_cocoa-0.4.0/src/cocoa/repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-15 20:27:12.000000 dsi_cocoa-0.4.0/src/cocoa/spring2024.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:27:22.547509 dsi_cocoa-0.4.0/src/dsi_cocoa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-15 20:27:22.000000 dsi_cocoa-0.4.0/src/dsi_cocoa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-15 20:27:22.000000 dsi_cocoa-0.4.0/src/dsi_cocoa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 20:27:22.000000 dsi_cocoa-0.4.0/src/dsi_cocoa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-15 20:27:22.000000 dsi_cocoa-0.4.0/src/dsi_cocoa.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-15 20:27:22.000000 dsi_cocoa-0.4.0/src/dsi_cocoa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 20:27:22.000000 dsi_cocoa-0.4.0/src/dsi_cocoa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:32:10.487812 dsi_cocoa-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-15 20:32:06.000000 dsi_cocoa-0.5.0/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 20:31:57.000000 dsi_cocoa-0.5.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:32:10.483812 dsi_cocoa-0.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:32:10.483812 dsi_cocoa-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-15 20:31:57.000000 dsi_cocoa-0.5.0/.github/workflows/main.workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-15 20:31:57.000000 dsi_cocoa-0.5.0/.github/workflows/publish.workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-15 20:31:57.000000 dsi_cocoa-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-15 20:31:57.000000 dsi_cocoa-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-15 20:32:10.487812 dsi_cocoa-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-05-15 20:31:57.000000 dsi_cocoa-0.5.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)       66 2024-05-15 20:31:57.000000 dsi_cocoa-0.5.0/eval-repo.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-15 20:31:57.000000 dsi_cocoa-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-15 20:31:57.000000 dsi_cocoa-0.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-15 20:32:10.487812 dsi_cocoa-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-15 20:32:06.000000 dsi_cocoa-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:32:10.483812 dsi_cocoa-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:32:10.483812 dsi_cocoa-0.5.0/src/cocoa/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-15 20:32:06.000000 dsi_cocoa-0.5.0/src/cocoa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-15 20:31:57.000000 dsi_cocoa-0.5.0/src/cocoa/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-15 20:31:57.000000 dsi_cocoa-0.5.0/src/cocoa/evaluate_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8865 2024-05-15 20:31:57.000000 dsi_cocoa-0.5.0/src/cocoa/linting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-15 20:31:57.000000 dsi_cocoa-0.5.0/src/cocoa/notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-05-15 20:31:57.000000 dsi_cocoa-0.5.0/src/cocoa/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-15 20:31:57.000000 dsi_cocoa-0.5.0/src/cocoa/spring2024.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:32:10.487812 dsi_cocoa-0.5.0/src/dsi_cocoa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-15 20:32:10.000000 dsi_cocoa-0.5.0/src/dsi_cocoa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-15 20:32:10.000000 dsi_cocoa-0.5.0/src/dsi_cocoa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 20:32:10.000000 dsi_cocoa-0.5.0/src/dsi_cocoa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-15 20:32:10.000000 dsi_cocoa-0.5.0/src/dsi_cocoa.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-15 20:32:10.000000 dsi_cocoa-0.5.0/src/dsi_cocoa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 20:32:10.000000 dsi_cocoa-0.5.0/src/dsi_cocoa.egg-info/top_level.txt
```

### Comparing `dsi_cocoa-0.4.0/.github/workflows/main.workflow.yml` & `dsi_cocoa-0.5.0/.github/workflows/main.workflow.yml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.4.0/.github/workflows/publish.workflow.yml` & `dsi_cocoa-0.5.0/.github/workflows/publish.workflow.yml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.4.0/.gitignore` & `dsi_cocoa-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.4.0/.pre-commit-config.yaml` & `dsi_cocoa-0.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.4.0/PKG-INFO` & `dsi_cocoa-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsi-cocoa
-Version: 0.4.0
+Version: 0.5.0
 Summary: Clinic Opinionated Codebase Oversight and Analysis
 Author-email: Nick Ross <tspread@uchicago.edu>, Trevor Spreadbury <tspread@uchicago.edu>
 Maintainer: Nick Ross, Trevor Spreadbury
 Keywords: codebase analysis,uchicago dsi
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `dsi_cocoa-0.4.0/README.md` & `dsi_cocoa-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.4.0/pyproject.toml` & `dsi_cocoa-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.4.0/src/cocoa/evaluate_repo.py` & `dsi_cocoa-0.5.0/src/cocoa/evaluate_repo.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.4.0/src/cocoa/linting.py` & `dsi_cocoa-0.5.0/src/cocoa/linting.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.4.0/src/cocoa/notebooks.py` & `dsi_cocoa-0.5.0/src/cocoa/notebooks.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.4.0/src/cocoa/repo.py` & `dsi_cocoa-0.5.0/src/cocoa/repo.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.4.0/src/cocoa/spring2024.py` & `dsi_cocoa-0.5.0/src/cocoa/spring2024.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.4.0/src/dsi_cocoa.egg-info/PKG-INFO` & `dsi_cocoa-0.5.0/src/dsi_cocoa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsi-cocoa
-Version: 0.4.0
+Version: 0.5.0
 Summary: Clinic Opinionated Codebase Oversight and Analysis
 Author-email: Nick Ross <tspread@uchicago.edu>, Trevor Spreadbury <tspread@uchicago.edu>
 Maintainer: Nick Ross, Trevor Spreadbury
 Keywords: codebase analysis,uchicago dsi
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `dsi_cocoa-0.4.0/src/dsi_cocoa.egg-info/SOURCES.txt` & `dsi_cocoa-0.5.0/src/dsi_cocoa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

