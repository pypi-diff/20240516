# Comparing `tmp/dsi_cocoa-0.5.0.tar.gz` & `tmp/dsi_cocoa-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsi_cocoa-0.5.0.tar", last modified: Wed May 15 20:32:10 2024, max compression
+gzip compressed data, was "dsi_cocoa-0.5.1.tar", last modified: Thu May 16 16:51:26 2024, max compression
```

## Comparing `dsi_cocoa-0.5.0.tar` & `dsi_cocoa-0.5.1.tar`

### file list

```diff
@@ -1,32 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:32:10.487812 dsi_cocoa-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-15 20:32:06.000000 dsi_cocoa-0.5.0/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 20:31:57.000000 dsi_cocoa-0.5.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:32:10.483812 dsi_cocoa-0.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:32:10.483812 dsi_cocoa-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-15 20:31:57.000000 dsi_cocoa-0.5.0/.github/workflows/main.workflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-15 20:31:57.000000 dsi_cocoa-0.5.0/.github/workflows/publish.workflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-15 20:31:57.000000 dsi_cocoa-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-15 20:31:57.000000 dsi_cocoa-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-15 20:32:10.487812 dsi_cocoa-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-05-15 20:31:57.000000 dsi_cocoa-0.5.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)       66 2024-05-15 20:31:57.000000 dsi_cocoa-0.5.0/eval-repo.sh
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-15 20:31:57.000000 dsi_cocoa-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-15 20:31:57.000000 dsi_cocoa-0.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-15 20:32:10.487812 dsi_cocoa-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-15 20:32:06.000000 dsi_cocoa-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:32:10.483812 dsi_cocoa-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:32:10.483812 dsi_cocoa-0.5.0/src/cocoa/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-15 20:32:06.000000 dsi_cocoa-0.5.0/src/cocoa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-15 20:31:57.000000 dsi_cocoa-0.5.0/src/cocoa/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-15 20:31:57.000000 dsi_cocoa-0.5.0/src/cocoa/evaluate_repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8865 2024-05-15 20:31:57.000000 dsi_cocoa-0.5.0/src/cocoa/linting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-15 20:31:57.000000 dsi_cocoa-0.5.0/src/cocoa/notebooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-05-15 20:31:57.000000 dsi_cocoa-0.5.0/src/cocoa/repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-15 20:31:57.000000 dsi_cocoa-0.5.0/src/cocoa/spring2024.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:32:10.487812 dsi_cocoa-0.5.0/src/dsi_cocoa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-15 20:32:10.000000 dsi_cocoa-0.5.0/src/dsi_cocoa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-15 20:32:10.000000 dsi_cocoa-0.5.0/src/dsi_cocoa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 20:32:10.000000 dsi_cocoa-0.5.0/src/dsi_cocoa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-15 20:32:10.000000 dsi_cocoa-0.5.0/src/dsi_cocoa.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-15 20:32:10.000000 dsi_cocoa-0.5.0/src/dsi_cocoa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 20:32:10.000000 dsi_cocoa-0.5.0/src/dsi_cocoa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:51:26.302008 dsi_cocoa-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-16 16:51:21.000000 dsi_cocoa-0.5.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:51:26.298008 dsi_cocoa-0.5.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:51:26.298008 dsi_cocoa-0.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-16 16:51:21.000000 dsi_cocoa-0.5.1/.github/workflows/error.badges.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-16 16:51:21.000000 dsi_cocoa-0.5.1/.github/workflows/main.workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-16 16:51:21.000000 dsi_cocoa-0.5.1/.github/workflows/publish.workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-16 16:51:21.000000 dsi_cocoa-0.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-16 16:51:21.000000 dsi_cocoa-0.5.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-16 16:51:26.302008 dsi_cocoa-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-05-16 16:51:21.000000 dsi_cocoa-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-16 16:51:21.000000 dsi_cocoa-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-16 16:51:21.000000 dsi_cocoa-0.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-16 16:51:26.302008 dsi_cocoa-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:51:26.298008 dsi_cocoa-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:51:26.298008 dsi_cocoa-0.5.1/src/cocoa/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 16:51:21.000000 dsi_cocoa-0.5.1/src/cocoa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-16 16:51:21.000000 dsi_cocoa-0.5.1/src/cocoa/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-05-16 16:51:21.000000 dsi_cocoa-0.5.1/src/cocoa/evaluate_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8865 2024-05-16 16:51:21.000000 dsi_cocoa-0.5.1/src/cocoa/linting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-16 16:51:21.000000 dsi_cocoa-0.5.1/src/cocoa/notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-05-16 16:51:21.000000 dsi_cocoa-0.5.1/src/cocoa/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-16 16:51:21.000000 dsi_cocoa-0.5.1/src/cocoa/spring2024.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:51:26.302008 dsi_cocoa-0.5.1/src/dsi_cocoa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-16 16:51:26.000000 dsi_cocoa-0.5.1/src/dsi_cocoa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-16 16:51:26.000000 dsi_cocoa-0.5.1/src/dsi_cocoa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 16:51:26.000000 dsi_cocoa-0.5.1/src/dsi_cocoa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-16 16:51:26.000000 dsi_cocoa-0.5.1/src/dsi_cocoa.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-16 16:51:26.000000 dsi_cocoa-0.5.1/src/dsi_cocoa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-16 16:51:26.000000 dsi_cocoa-0.5.1/src/dsi_cocoa.egg-info/top_level.txt
```

### Comparing `dsi_cocoa-0.5.0/.github/workflows/main.workflow.yml` & `dsi_cocoa-0.5.1/.github/workflows/main.workflow.yml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.5.0/.github/workflows/publish.workflow.yml` & `dsi_cocoa-0.5.1/.github/workflows/publish.workflow.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,68 +1,53 @@
 name: Publish Python Distribution to PyPI
 # adapted from
 # https://packaging.python.org/en/latest/guides/publishing-package-distribution-releases-using-github-actions-ci-cd-workflows/
 
 on:
   push:
-    # trigger the workflow on push events to main branch
-    branches:
-      # - main
-      - publish-to-pypi
+    tags:
+      - 'v[0-9]+.[0-9]+.[0-9]+'
+# publish when a new tag is pushed with semantic version
 
 jobs:
   build:
     name: Build distribution
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v4
       - name: Set up python
         uses: actions/setup-python@v4
         with:
           python-version: "3.x"
-
       - name: Install pypa/build
         run: >-
           python3 -m
           pip install
-          build bump2version
+          build
           --user
-
-      - name: Set up Git identity
-        run: |
-          git config --global user.name "chenhuifei01"
-          git config --global user.email "chenhui1@uchicago.edu"
-
-      - name: Bump minor version
-        # haven't settip the cfg yet
-        # run: bump2version minor --config-file .bumpversion.cfg
-        run: bump2version minor
-
       - name: Build a binary wheel and a source tarball
         run: python3 -m build
-
       - name: Store the distribution packages
         uses: actions/upload-artifact@v3
         with:
           name: python-package-distributions
           path: dist/
-
   publish-to-pypi:
     name: PublishPython distribution to PyPI
     needs:
       - build
     runs-on: ubuntu-latest
     environment:
       name: pypi
       url: https://pypi.org/p/dsi-cocoa
     permissions:
       id-token: write
-
+    
     steps:
       - name: Download all the dists
         uses: actions/download-artifact@v3
         with:
           name: python-package-distributions
           path: dist/
       - name: Publish distributions to PyPI
-        uses: pypa/gh-action-pypi-publish@release/v1
+        uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `dsi_cocoa-0.5.0/.gitignore` & `dsi_cocoa-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.5.0/.pre-commit-config.yaml` & `dsi_cocoa-0.5.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.5.0/PKG-INFO` & `dsi_cocoa-0.5.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsi-cocoa
-Version: 0.5.0
+Version: 0.5.1
 Summary: Clinic Opinionated Codebase Oversight and Analysis
 Author-email: Nick Ross <tspread@uchicago.edu>, Trevor Spreadbury <tspread@uchicago.edu>
 Maintainer: Nick Ross, Trevor Spreadbury
 Keywords: codebase analysis,uchicago dsi
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -15,24 +15,26 @@
 Requires-Dist: ipython
 Requires-Dist: termcolor
 Requires-Dist: black
 Requires-Dist: requests
 
 # Clinic Opinionated Codebase Oversight and Analysis
 
+[![Cocoa Error Analysis](https://github.com/dsi-clinic/cocoa/actions/workflows/error.badges.yml/badge.svg)](https://github.com/dsi-clinic/cocoa/actions/workflows/error.badges.yml)
+
+
 This repository was developed in order to generate automated reports on how well codebases adhere to the [coding standards](https://github.com/dsi-clinic/coding-standards) of the University of Chicago's DSI [Clinic course](https://datascience.uchicago.edu/education/data-science-clinic/).
 
 The goals of this codebase is to provide a quick and easy way to review code and to alert contributors where their code may be failing.
 
 ## Installation
 
-`pip install dsi-cocoa`
-
-To install the package from the local files, run the following command from the root of the repository:
+```pip install dsi-cocoa```
 
+To install the package locally, run the following command from the root of the repository:
 ```bash
 python3 -m pip install .
 ```
 
 ## cocoa
 
 This package contains a module `evaluate_repo` which runs code testing libraries against a repository. There are multiple ways that we want to be able to run this repo:
@@ -40,74 +42,79 @@
 1. We want to be able to clone `cocoa` and then use it as part of their process.
 2. We want administrators to be able to give it a list of repos to generate reports on all repos.
 3. (Eventually) We want it to be able to run as a github action _on the repo itself_.
 4. (Eventually) We want to be able to have adminstrative repo that can run it on other repos.
 
 ### How to run
 
-Via command line:
-
+Via command line: 
 ```bash
 cocoa /path/to/repo
 ```
 
-As a python script:
-
+As a python script: 
 ```bash
 python3 src/cocoa/evaluate_repo.py /path/to/repo
 ```
 
 As a Python module:
-
 ```python
 from cocoa.evaluate_repo import evaluate_repo
 
 evaluate_repo('/path/to/repo', False)
 ```
 
 A few important notes:
 
 1. Make sure to `git pull` _before_ running this code.
 1. This will get branch information for all branches.
 1. This will only run the analysis (`pyflakes` on python files) for the code _in the current branch_. So if you run this while your current branch is `main` it will run on `main`.
 
 #### Options
-
-If you want to do linting on Python files, then you can add the argument "--lint" to the command:
+If you want to turn on linting, add the argument "--lint":
 
 ```bash
 cocoa /path/to/repo --lint
 ```
 
 Results are truncated by default. To print all results, use the verbose option:
 
 ```bash
 cocoa /path/to/repo --verbose
 ```
 
+To report remote branch information, use the `--branchinfo` option.
+
+To run cocoa on files changed after a certain date, use the `--date` option with a date formatted as below.
+```bash
+cocoa /path/to/repo --date YYYY-MM-DD
+```
+
+
 ### Checks
 
 The code run multiple checks on each repo. For each check run there are three possibilities:
 
-1. WARNING: Most likely this needs to be fixed.
+1. WARNING: Most likely this needs to be fixed. 
 1. INFO: Log information for additional context.
 1. ERROR: A critical issue that needs to be addressed.
 
 For each of the checks below we have denoted what the check generates.
 
 - Branch Hygiene:
-  - [WARNING] Branch names
-  - [INFO] Commit information for live branches.
+    - [WARNING] Branch names 
+    - [INFO] Commit information for live branches.
 - File Hygiene:
-  - [ERROR] Unnecessary and cache file (such as .DS_Store or pycache files)
-- Notebook Files (\*.ipynb):
-  - [ERROR] Cells per notebook < 10, lines per cell < 15 and 0 functions defined
-  - [ERROR] Linting: PyLint, Black, Flake and iSort
+    - [ERROR] Unnecessary and cache file (such as .DS\_Store or pycache files)
+- Notebook Files (*.ipynb):
+    - [ERROR] Cells per notebook < 10, lines per cell < 15 and 0 functions defined
+    - [ERROR] Linting: PyLint, Black, Flake and iSort
 - Python Files
-  - [ERROR] All Code in Functions
-  - [ERROR] All functions have docstrings
-  - [ERROR] Code uses off-limit libraries (subprocess)
-  - [ERROR] Linting: PyLint, Black, Flake and iSort
-
+    - [ERROR] All Code in Functions
+    - [ERROR] All functions have docstrings
+    - [ERROR] Code uses off-limit libraries (subprocess)
+    - [ERROR] Linting: PyLint, Black, Flake and iSort
+    
 ### Github actions
 
 For each of the ERRORS and WARNINGS above there is an associated github action that can be run to create a badge which we put in a table at the top of each clinic repo.
+
```

### Comparing `dsi_cocoa-0.5.0/README.md` & `dsi_cocoa-0.5.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # Clinic Opinionated Codebase Oversight and Analysis
 
+[![Cocoa Error Analysis](https://github.com/dsi-clinic/cocoa/actions/workflows/error.badges.yml/badge.svg)](https://github.com/dsi-clinic/cocoa/actions/workflows/error.badges.yml)
+
+
 This repository was developed in order to generate automated reports on how well codebases adhere to the [coding standards](https://github.com/dsi-clinic/coding-standards) of the University of Chicago's DSI [Clinic course](https://datascience.uchicago.edu/education/data-science-clinic/).
 
 The goals of this codebase is to provide a quick and easy way to review code and to alert contributors where their code may be failing.
 
 ## Installation
 
-`pip install dsi-cocoa`
-
-To install the package from the local files, run the following command from the root of the repository:
+```pip install dsi-cocoa```
 
+To install the package locally, run the following command from the root of the repository:
 ```bash
 python3 -m pip install .
 ```
 
 ## cocoa
 
 This package contains a module `evaluate_repo` which runs code testing libraries against a repository. There are multiple ways that we want to be able to run this repo:
@@ -21,74 +23,79 @@
 1. We want to be able to clone `cocoa` and then use it as part of their process.
 2. We want administrators to be able to give it a list of repos to generate reports on all repos.
 3. (Eventually) We want it to be able to run as a github action _on the repo itself_.
 4. (Eventually) We want to be able to have adminstrative repo that can run it on other repos.
 
 ### How to run
 
-Via command line:
-
+Via command line: 
 ```bash
 cocoa /path/to/repo
 ```
 
-As a python script:
-
+As a python script: 
 ```bash
 python3 src/cocoa/evaluate_repo.py /path/to/repo
 ```
 
 As a Python module:
-
 ```python
 from cocoa.evaluate_repo import evaluate_repo
 
 evaluate_repo('/path/to/repo', False)
 ```
 
 A few important notes:
 
 1. Make sure to `git pull` _before_ running this code.
 1. This will get branch information for all branches.
 1. This will only run the analysis (`pyflakes` on python files) for the code _in the current branch_. So if you run this while your current branch is `main` it will run on `main`.
 
 #### Options
-
-If you want to do linting on Python files, then you can add the argument "--lint" to the command:
+If you want to turn on linting, add the argument "--lint":
 
 ```bash
 cocoa /path/to/repo --lint
 ```
 
 Results are truncated by default. To print all results, use the verbose option:
 
 ```bash
 cocoa /path/to/repo --verbose
 ```
 
+To report remote branch information, use the `--branchinfo` option.
+
+To run cocoa on files changed after a certain date, use the `--date` option with a date formatted as below.
+```bash
+cocoa /path/to/repo --date YYYY-MM-DD
+```
+
+
 ### Checks
 
 The code run multiple checks on each repo. For each check run there are three possibilities:
 
-1. WARNING: Most likely this needs to be fixed.
+1. WARNING: Most likely this needs to be fixed. 
 1. INFO: Log information for additional context.
 1. ERROR: A critical issue that needs to be addressed.
 
 For each of the checks below we have denoted what the check generates.
 
 - Branch Hygiene:
-  - [WARNING] Branch names
-  - [INFO] Commit information for live branches.
+    - [WARNING] Branch names 
+    - [INFO] Commit information for live branches.
 - File Hygiene:
-  - [ERROR] Unnecessary and cache file (such as .DS_Store or pycache files)
-- Notebook Files (\*.ipynb):
-  - [ERROR] Cells per notebook < 10, lines per cell < 15 and 0 functions defined
-  - [ERROR] Linting: PyLint, Black, Flake and iSort
+    - [ERROR] Unnecessary and cache file (such as .DS\_Store or pycache files)
+- Notebook Files (*.ipynb):
+    - [ERROR] Cells per notebook < 10, lines per cell < 15 and 0 functions defined
+    - [ERROR] Linting: PyLint, Black, Flake and iSort
 - Python Files
-  - [ERROR] All Code in Functions
-  - [ERROR] All functions have docstrings
-  - [ERROR] Code uses off-limit libraries (subprocess)
-  - [ERROR] Linting: PyLint, Black, Flake and iSort
-
+    - [ERROR] All Code in Functions
+    - [ERROR] All functions have docstrings
+    - [ERROR] Code uses off-limit libraries (subprocess)
+    - [ERROR] Linting: PyLint, Black, Flake and iSort
+    
 ### Github actions
 
 For each of the ERRORS and WARNINGS above there is an associated github action that can be run to create a badge which we put in a table at the top of each clinic repo.
+
```

### Comparing `dsi_cocoa-0.5.0/pyproject.toml` & `dsi_cocoa-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.5.0/src/cocoa/evaluate_repo.py` & `dsi_cocoa-0.5.1/src/cocoa/evaluate_repo.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """
 Main entry point for complete evaluation of a python codebase in git
 """
 
 import argparse
 import os
+import shutil
 
 from termcolor import cprint
 
 from cocoa.constants import (
     MAX_CELLS_PER_NOTEBOOK,
     MAX_FUNCTIONS_PER_NOTEBOOK,
     MAX_LINES_PER_CELL,
+    PREAMBLE_TEXT,
 )
 from cocoa.linting import (
     black_python_file,
     code_contains_subprocess,
     functions_without_docstrings,
     get_pylint_warnings,
     is_code_in_functions_or_main,
@@ -30,15 +32,15 @@
     get_remote_branches_info,
     is_git_remote_repo,
     is_git_repo,
 )
 
 
 def walk_and_process(
-    dir_path, no_filter_flag, lint_flag, start_date=None, verbose=False
+    dir_path, lint_flag, start_date=None, verbose=False
 ):
     """
     Walk through directory and process all python and jupyter notebook files.
     """
     paths_to_flag = ["__pycache__", "DS_Store", "ipynb_checkpoints"]
     cprint(
         f"Currently analyzing branch {get_current_branch(dir_path)}",
@@ -54,111 +56,135 @@
             for f in files
             if not any(x in os.path.join(root, f) for x in paths_to_flag)
         ]
 
     for file_path in files_to_process:
         if os.path.exists(file_path):
             if file_path.endswith(".ipynb") or file_path.endswith(".py"):
-                print(f"Analyzing {file_path}:")
                 if file_path.endswith(".ipynb"):
-                    analyze_notebook(file_path, no_filter_flag, verbose)
+                    analyze_notebook(file_path, verbose)
                 elif file_path.endswith(".py"):
                     analyze_python_file(file_path, lint_flag, verbose)
-                print("-" * 80)
 
 
-def analyze_notebook(file_path, no_filter_flag, verbose):
+def analyze_notebook(file_path, verbose):
     """Analyze a notebook"""
     num_cells, num_lines, num_functions, max_lines_in_cell = process_notebook(
         file_path
     )
     pyflake_results = pyflakes_notebook(file_path)
-    print_results("PyFlakes", pyflake_results, verbose=verbose)
-    if no_filter_flag or (
-        num_cells > MAX_CELLS_PER_NOTEBOOK
+
+    if (
+        pyflake_results
+        or num_cells > MAX_CELLS_PER_NOTEBOOK
         or max_lines_in_cell > MAX_LINES_PER_CELL
         or num_functions > MAX_FUNCTIONS_PER_NOTEBOOK
     ):
-        print(f"\tNumber of cells: {num_cells}")
-        print(f"\tLines of code: {num_lines}")
-        print(f"\tNumber of function definitions: {num_functions}")
-        print(f"\tMax lines in a cell: {max_lines_in_cell}")
+        print(f"Analyzing {file_path}:")
+        if pyflake_results:
+            print_results("PyFlakes", pyflake_results, verbose=verbose)
+
+        if num_cells > MAX_CELLS_PER_NOTEBOOK:
+            print(f"\tMax number of cells exceeded: {num_cells}")
+        if max_lines_in_cell > MAX_LINES_PER_CELL:
+            print(
+                f"\tMax number of lines per cell exceeded: {max_lines_in_cell}"
+            )
+        if num_functions > MAX_FUNCTIONS_PER_NOTEBOOK:
+            print(f"\tFunction definitions detected: {num_functions}")
+
+        print("-" * 80)
 
 
 def analyze_python_file(file_path, lint_flag, verbose):
     """Analyze a Python file"""
     pyflake_results = pyflakes_python_file(file_path)
-    pylint_warnings = get_pylint_warnings(file_path)
     black_results = black_python_file(file_path)
+    functions_no_docstrings = functions_without_docstrings(file_path)
+    contains_subprocess = code_contains_subprocess(file_path)
+    code_in_functions = is_code_in_functions_or_main(file_path)
+    pylint_warnings = get_pylint_warnings(file_path)
 
-    if lint_flag:
-        print_results("Pylint", pylint_warnings, verbose=verbose)
-
-    print_results("PyFlakes", pyflake_results, verbose=verbose)
-
-    if black_results:
-        print(f"\tPlease run black. {len(black_results)} changes needed.")
+    if (
+        (lint_flag and pylint_warnings)
+        or pyflake_results
+        or black_results
+        or functions_no_docstrings
+        or contains_subprocess
+        or not code_in_functions
+    ):
+        print(f"Analyzing {file_path}:")
 
-    if not is_code_in_functions_or_main(file_path):
-        print("\tCode outside functions or main block detected.")
-
-    if code_contains_subprocess(file_path):
-        print("\tWarning: subprocess usage detected.")
-
-    functions_no_docstrings = functions_without_docstrings(file_path)
-    if functions_no_docstrings:
-        print(
-            "\tFunctions without docstrings detected:", functions_no_docstrings
-        )
+        if pyflake_results:
+            print_results("PyFlakes", pyflake_results, verbose=verbose)
+        if black_results:
+            print(f"\tBlack found {len(black_results)} issues")
+        if functions_no_docstrings:
+            print(
+                "\tFunctions without docstrings detected:",
+                functions_no_docstrings,
+            )
+        if contains_subprocess:
+            print("\tSubprocess usage detected.")
+        if not code_in_functions:
+            print("\tCode outside functions or main block detected.")
+        if lint_flag:
+            print_results("Pylint", pylint_warnings, verbose=verbose)
+        print("-" * 80)
 
 
 def print_results(tool_name, results, verbose=False):
     """Print results from pylint or pyflake"""
     if results:
         if verbose:
-            print(f"{tool_name} found {len(results)} issues:")
+            print(f"\t{tool_name} found {len(results)} issues:")
             for result in results:
-                print(f"  {result}")
+                print(f"\t  {result}")
         else:
-            print(f"{tool_name} found {len(results)} issues:")
+            print(f"\t{tool_name} found {len(results)} issues:")
             for result in results[:5]:
-                print(f"  {result}")
+                print(f"\t  {result}")
             if len(results) > 5:
-                print(f"  ...and {len(results) - 5} more issues.")
+                print(f"\t  ...and {len(results) - 5} more issues.")
 
 
-def evaluate_repo(path_or_url, lint_flag, start_date=None, verbose=False):
+def evaluate_repo(
+    path_or_url, lint_flag, start_date=None, verbose=False, branchinfo=False
+):
     """
     This is the entry point to running the automated code review.
     """
-
+    cprint(PREAMBLE_TEXT, color="green")
     if os.path.isdir(path_or_url):
         if not is_git_repo(path_or_url):
             print(f"Error: {path_or_url} is not a Git repository.")
             exit(1)
 
         check_branch_names(path_or_url)
-        get_remote_branches_info(path_or_url)
+        if branchinfo:
+            get_remote_branches_info(path_or_url)
         walk_and_process(
             path_or_url,
-            None,
             lint_flag=lint_flag,
             start_date=start_date,
             verbose=verbose,
         )
     elif is_git_remote_repo(path_or_url):
         repo_path = clone_repo(path_or_url)
         evaluate_repo(
             repo_path,
             lint_flag=lint_flag,
             start_date=start_date,
             verbose=verbose,
         )
+        shutil.rmtree(repo_path)
     else:
-        print(f"Error: {path_or_url} is not a Git repository URL.")
+        print(
+            f"Error: {path_or_url} is either private or not a git repository. 404."
+        )
         exit(1)
     return 0
 
 
 def main():
     parser = argparse.ArgumentParser(description="COCOA CLI")
 
@@ -169,20 +195,24 @@
     )
     parser.add_argument(
         "--date",
         default=None,
         help="Start date in YYYY-MM-DD format to filter files by commit date",
         type=str,
     )
+    parser.add_argument(
+        "--branchinfo", help="Report branch information", action="store_true"
+    )
 
     args = parser.parse_args()
 
     dir_path = args.repo
     lint_flag = args.lint
     start_date = args.date
     verbose = args.verbose
+    branchinfo = args.branchinfo
 
-    evaluate_repo(dir_path, lint_flag, start_date, verbose)
+    evaluate_repo(dir_path, lint_flag, start_date, verbose, branchinfo)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `dsi_cocoa-0.5.0/src/cocoa/linting.py` & `dsi_cocoa-0.5.1/src/cocoa/linting.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.5.0/src/cocoa/notebooks.py` & `dsi_cocoa-0.5.1/src/cocoa/notebooks.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.5.0/src/cocoa/repo.py` & `dsi_cocoa-0.5.1/src/cocoa/repo.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.5.0/src/cocoa/spring2024.py` & `dsi_cocoa-0.5.1/src/cocoa/spring2024.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.5.0/src/dsi_cocoa.egg-info/PKG-INFO` & `dsi_cocoa-0.5.1/src/dsi_cocoa.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsi-cocoa
-Version: 0.5.0
+Version: 0.5.1
 Summary: Clinic Opinionated Codebase Oversight and Analysis
 Author-email: Nick Ross <tspread@uchicago.edu>, Trevor Spreadbury <tspread@uchicago.edu>
 Maintainer: Nick Ross, Trevor Spreadbury
 Keywords: codebase analysis,uchicago dsi
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -15,24 +15,26 @@
 Requires-Dist: ipython
 Requires-Dist: termcolor
 Requires-Dist: black
 Requires-Dist: requests
 
 # Clinic Opinionated Codebase Oversight and Analysis
 
+[![Cocoa Error Analysis](https://github.com/dsi-clinic/cocoa/actions/workflows/error.badges.yml/badge.svg)](https://github.com/dsi-clinic/cocoa/actions/workflows/error.badges.yml)
+
+
 This repository was developed in order to generate automated reports on how well codebases adhere to the [coding standards](https://github.com/dsi-clinic/coding-standards) of the University of Chicago's DSI [Clinic course](https://datascience.uchicago.edu/education/data-science-clinic/).
 
 The goals of this codebase is to provide a quick and easy way to review code and to alert contributors where their code may be failing.
 
 ## Installation
 
-`pip install dsi-cocoa`
-
-To install the package from the local files, run the following command from the root of the repository:
+```pip install dsi-cocoa```
 
+To install the package locally, run the following command from the root of the repository:
 ```bash
 python3 -m pip install .
 ```
 
 ## cocoa
 
 This package contains a module `evaluate_repo` which runs code testing libraries against a repository. There are multiple ways that we want to be able to run this repo:
@@ -40,74 +42,79 @@
 1. We want to be able to clone `cocoa` and then use it as part of their process.
 2. We want administrators to be able to give it a list of repos to generate reports on all repos.
 3. (Eventually) We want it to be able to run as a github action _on the repo itself_.
 4. (Eventually) We want to be able to have adminstrative repo that can run it on other repos.
 
 ### How to run
 
-Via command line:
-
+Via command line: 
 ```bash
 cocoa /path/to/repo
 ```
 
-As a python script:
-
+As a python script: 
 ```bash
 python3 src/cocoa/evaluate_repo.py /path/to/repo
 ```
 
 As a Python module:
-
 ```python
 from cocoa.evaluate_repo import evaluate_repo
 
 evaluate_repo('/path/to/repo', False)
 ```
 
 A few important notes:
 
 1. Make sure to `git pull` _before_ running this code.
 1. This will get branch information for all branches.
 1. This will only run the analysis (`pyflakes` on python files) for the code _in the current branch_. So if you run this while your current branch is `main` it will run on `main`.
 
 #### Options
-
-If you want to do linting on Python files, then you can add the argument "--lint" to the command:
+If you want to turn on linting, add the argument "--lint":
 
 ```bash
 cocoa /path/to/repo --lint
 ```
 
 Results are truncated by default. To print all results, use the verbose option:
 
 ```bash
 cocoa /path/to/repo --verbose
 ```
 
+To report remote branch information, use the `--branchinfo` option.
+
+To run cocoa on files changed after a certain date, use the `--date` option with a date formatted as below.
+```bash
+cocoa /path/to/repo --date YYYY-MM-DD
+```
+
+
 ### Checks
 
 The code run multiple checks on each repo. For each check run there are three possibilities:
 
-1. WARNING: Most likely this needs to be fixed.
+1. WARNING: Most likely this needs to be fixed. 
 1. INFO: Log information for additional context.
 1. ERROR: A critical issue that needs to be addressed.
 
 For each of the checks below we have denoted what the check generates.
 
 - Branch Hygiene:
-  - [WARNING] Branch names
-  - [INFO] Commit information for live branches.
+    - [WARNING] Branch names 
+    - [INFO] Commit information for live branches.
 - File Hygiene:
-  - [ERROR] Unnecessary and cache file (such as .DS_Store or pycache files)
-- Notebook Files (\*.ipynb):
-  - [ERROR] Cells per notebook < 10, lines per cell < 15 and 0 functions defined
-  - [ERROR] Linting: PyLint, Black, Flake and iSort
+    - [ERROR] Unnecessary and cache file (such as .DS\_Store or pycache files)
+- Notebook Files (*.ipynb):
+    - [ERROR] Cells per notebook < 10, lines per cell < 15 and 0 functions defined
+    - [ERROR] Linting: PyLint, Black, Flake and iSort
 - Python Files
-  - [ERROR] All Code in Functions
-  - [ERROR] All functions have docstrings
-  - [ERROR] Code uses off-limit libraries (subprocess)
-  - [ERROR] Linting: PyLint, Black, Flake and iSort
-
+    - [ERROR] All Code in Functions
+    - [ERROR] All functions have docstrings
+    - [ERROR] Code uses off-limit libraries (subprocess)
+    - [ERROR] Linting: PyLint, Black, Flake and iSort
+    
 ### Github actions
 
 For each of the ERRORS and WARNINGS above there is an associated github action that can be run to create a badge which we put in a table at the top of each clinic repo.
+
```

### Comparing `dsi_cocoa-0.5.0/src/dsi_cocoa.egg-info/SOURCES.txt` & `dsi_cocoa-0.5.1/src/dsi_cocoa.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-.bumpversion.cfg
 .gitattributes
 .gitignore
 .pre-commit-config.yaml
 README.md
-eval-repo.sh
 pyproject.toml
 requirements.txt
 setup.cfg
-setup.py
+.github/workflows/error.badges.yml
 .github/workflows/main.workflow.yml
 .github/workflows/publish.workflow.yml
 src/cocoa/__init__.py
 src/cocoa/constants.py
 src/cocoa/evaluate_repo.py
 src/cocoa/linting.py
 src/cocoa/notebooks.py
```

