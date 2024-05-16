# Comparing `tmp/dodonacli-2024.5.15.tar.gz` & `tmp/dodonacli-2024.5.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dodonacli-2024.5.15.tar", last modified: Wed May 15 06:36:11 2024, max compression
+gzip compressed data, was "dodonacli-2024.5.16.tar", last modified: Thu May 16 12:25:51 2024, max compression
```

## Comparing `dodonacli-2024.5.15.tar` & `dodonacli-2024.5.16.tar`

### file list

```diff
@@ -1,47 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:36:11.955651 dodonacli-2024.5.15/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:36:11.951651 dodonacli-2024.5.15/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-15 06:35:55.000000 dodonacli-2024.5.15/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:36:11.951651 dodonacli-2024.5.15/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-15 06:35:55.000000 dodonacli-2024.5.15/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-05-15 06:35:55.000000 dodonacli-2024.5.15/.github/workflows/publishOLD.yml
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-15 06:35:55.000000 dodonacli-2024.5.15/.github/workflows/publish_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-15 06:35:55.000000 dodonacli-2024.5.15/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:36:11.955651 dodonacli-2024.5.15/DodonaCLI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9948 2024-05-15 06:36:11.000000 dodonacli-2024.5.15/DodonaCLI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-15 06:36:11.000000 dodonacli-2024.5.15/DodonaCLI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 06:36:11.000000 dodonacli-2024.5.15/DodonaCLI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-15 06:36:11.000000 dodonacli-2024.5.15/DodonaCLI.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-15 06:36:11.000000 dodonacli-2024.5.15/DodonaCLI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 06:36:11.000000 dodonacli-2024.5.15/DodonaCLI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-15 06:35:55.000000 dodonacli-2024.5.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9948 2024-05-15 06:36:11.955651 dodonacli-2024.5.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8083 2024-05-15 06:35:55.000000 dodonacli-2024.5.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:36:11.951651 dodonacli-2024.5.15/dodonacli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 06:35:55.000000 dodonacli-2024.5.15/dodonacli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:36:11.955651 dodonacli-2024.5.15/dodonacli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 06:35:55.000000 dodonacli-2024.5.15/dodonacli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8060 2024-05-15 06:35:55.000000 dodonacli-2024.5.15/dodonacli/commands/cli_next.py
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-15 06:35:55.000000 dodonacli-2024.5.15/dodonacli/commands/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-05-15 06:35:55.000000 dodonacli-2024.5.15/dodonacli/commands/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-05-15 06:35:55.000000 dodonacli-2024.5.15/dodonacli/commands/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     8779 2024-05-15 06:35:55.000000 dodonacli-2024.5.15/dodonacli/commands/select.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-15 06:35:55.000000 dodonacli-2024.5.15/dodonacli/commands/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-15 06:35:55.000000 dodonacli-2024.5.15/dodonacli/commands/submission.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-15 06:35:55.000000 dodonacli-2024.5.15/dodonacli/commands/tutorial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-15 06:35:55.000000 dodonacli-2024.5.15/dodonacli/commands/up.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      945 2024-05-15 06:35:55.000000 dodonacli-2024.5.15/dodonacli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:36:11.955651 dodonacli-2024.5.15/dodonacli/source/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-15 06:35:55.000000 dodonacli-2024.5.15/dodonacli/source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10629 2024-05-15 06:35:55.000000 dodonacli-2024.5.15/dodonacli/source/get_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    11938 2024-05-15 06:35:55.000000 dodonacli-2024.5.15/dodonacli/source/interactive_tutorial.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-15 06:35:55.000000 dodonacli-2024.5.15/dodonacli/source/pretty_console.py
--rw-r--r--   0 runner    (1001) docker     (127)    13631 2024-05-15 06:35:55.000000 dodonacli-2024.5.15/dodonacli/source/pretty_print.py
--rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-05-15 06:35:55.000000 dodonacli-2024.5.15/dodonacli/source/set_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-05-15 06:35:55.000000 dodonacli-2024.5.15/dodonacli/source/submission_data_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-05-15 06:35:55.000000 dodonacli-2024.5.15/dodonacli/source/syntax_checker.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1465 2024-05-15 06:35:55.000000 dodonacli-2024.5.15/dodonacli_completion_script.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:36:11.955651 dodonacli-2024.5.15/man-page/
--rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-05-15 06:35:55.000000 dodonacli-2024.5.15/man-page/dodonacli.1
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-05-15 06:35:55.000000 dodonacli-2024.5.15/man-page/dodonacli.1.gz
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-15 06:35:55.000000 dodonacli-2024.5.15/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 06:36:11.955651 dodonacli-2024.5.15/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:25:51.597000 dodonacli-2024.5.16/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:25:51.589000 dodonacli-2024.5.16/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:25:51.589000 dodonacli-2024.5.16/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/.github/workflows/publish_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:25:51.593000 dodonacli-2024.5.16/DodonaCLI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9745 2024-05-16 12:25:51.000000 dodonacli-2024.5.16/DodonaCLI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-16 12:25:51.000000 dodonacli-2024.5.16/DodonaCLI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 12:25:51.000000 dodonacli-2024.5.16/DodonaCLI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-16 12:25:51.000000 dodonacli-2024.5.16/DodonaCLI.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-16 12:25:51.000000 dodonacli-2024.5.16/DodonaCLI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-16 12:25:51.000000 dodonacli-2024.5.16/DodonaCLI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9745 2024-05-16 12:25:51.597000 dodonacli-2024.5.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7881 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:25:51.589000 dodonacli-2024.5.16/dodonacli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/dodonacli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:25:51.593000 dodonacli-2024.5.16/dodonacli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/dodonacli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8060 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/dodonacli/commands/cli_next.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/dodonacli/commands/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/dodonacli/commands/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/dodonacli/commands/post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8779 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/dodonacli/commands/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/dodonacli/commands/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/dodonacli/commands/submission.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/dodonacli/commands/tutorial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/dodonacli/commands/up.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      945 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/dodonacli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:25:51.593000 dodonacli-2024.5.16/dodonacli/source/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/dodonacli/source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10688 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/dodonacli/source/get_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12448 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/dodonacli/source/interactive_tutorial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/dodonacli/source/pretty_console.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13922 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/dodonacli/source/pretty_print.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5291 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/dodonacli/source/set_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/dodonacli/source/submission_data_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5166 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/dodonacli/source/syntax_checker.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1628 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/dodonacli_completion_script.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:25:51.593000 dodonacli-2024.5.16/man-page/
+-rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/man-page/dodonacli.1
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/man-page/dodonacli.1.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 12:25:51.597000 dodonacli-2024.5.16/setup.cfg
```

### Comparing `dodonacli-2024.5.15/.github/workflows/publish.yml` & `dodonacli-2024.5.16/.github/workflows/publish.yml`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 on:
   release:
     type: created
 
 jobs:
   build-and-publish:
     runs-on: ubuntu-latest
+    environment: Publish release
+    permissions:
+      id-token: write
 
     steps:
       - name: Checkout code
         uses: actions/checkout@v4
 
       - name: Set version
         run: |
@@ -25,12 +28,9 @@
         run: |
           python -m pip install --upgrade pip
           pip install build
 
       - name: Build package
         run: python -m build
 
-      - name: Publish package
+      - name: Publish package to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
-        with:
-          user: __token__
-          password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `dodonacli-2024.5.15/.github/workflows/publish_test.yml` & `dodonacli-2024.5.16/.github/workflows/publish_test.yml`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.5.15/DodonaCLI.egg-info/PKG-INFO` & `dodonacli-2024.5.16/DodonaCLI.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DodonaCLI
-Version: 2024.5.15
+Version: 2024.5.16
 Summary: A CLI tool for Dodona
 Author-email: Bram Windey <windey.bram@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Bram Windey
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -34,15 +34,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bs4
 Requires-Dist: click
 Requires-Dist: click-default-group
 Requires-Dist: markdownify
 Requires-Dist: packaging
-Requires-Dist: pkg_info
+Requires-Dist: pkg-info
 Requires-Dist: rich
 
 # Command Line Interface for [Dodona](https://dodona.be)
 
 PyPI page: https://pypi.org/project/DodonaCLI/#description
 
 **Contents**:
@@ -175,20 +175,14 @@
 to see if this is indeed the issue.
 
 
 ## Roadmap
 This section has a bunch of ideas for me to work on, but also for you, the potential contributor!
 Remember to look at the recent branches/commits to see if I’m not working on one of these:
 - user-settings (f.e. auto-download of files, language, formatting, number of submissions shown, config location, ...)
-- improve `info` command (man-page and such)
-- improve `tutorial`
 - easy (automatic?) downloading of files mentioned in exercise description
 - improve the rendering of all html/markdown frankensteins, in descriptions of exercises and exercise-descriptions 
 - add connection time-out to prevent long waiting when IPv6 doesn’t want to work along
 - add support for more languages syntax checkers
 - caching some info for faster navigation and/or autocompletion
 - add indicator to series to mark if all their exercises are completely solved (maybe fetch from html-version)
 - get exercise-names via html-parsing for a submission list to only need 1 API call (instead of 30)
-
-GitHub stuff to figure out:
-- release by tag/release
-- action to check valid version before trying to push, if not valid, make it valid
```

### Comparing `dodonacli-2024.5.15/DodonaCLI.egg-info/SOURCES.txt` & `dodonacli-2024.5.16/DodonaCLI.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 .gitignore
 LICENSE
 README.md
 dodonacli_completion_script.sh
 pyproject.toml
 .github/PULL_REQUEST_TEMPLATE.md
 .github/workflows/publish.yml
-.github/workflows/publishOLD.yml
 .github/workflows/publish_test.yml
 DodonaCLI.egg-info/PKG-INFO
 DodonaCLI.egg-info/SOURCES.txt
 DodonaCLI.egg-info/dependency_links.txt
 DodonaCLI.egg-info/entry_points.txt
 DodonaCLI.egg-info/requires.txt
 DodonaCLI.egg-info/top_level.txt
```

### Comparing `dodonacli-2024.5.15/LICENSE` & `dodonacli-2024.5.16/LICENSE`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.5.15/PKG-INFO` & `dodonacli-2024.5.16/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DodonaCLI
-Version: 2024.5.15
+Version: 2024.5.16
 Summary: A CLI tool for Dodona
 Author-email: Bram Windey <windey.bram@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Bram Windey
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -34,15 +34,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bs4
 Requires-Dist: click
 Requires-Dist: click-default-group
 Requires-Dist: markdownify
 Requires-Dist: packaging
-Requires-Dist: pkg_info
+Requires-Dist: pkg-info
 Requires-Dist: rich
 
 # Command Line Interface for [Dodona](https://dodona.be)
 
 PyPI page: https://pypi.org/project/DodonaCLI/#description
 
 **Contents**:
@@ -175,20 +175,14 @@
 to see if this is indeed the issue.
 
 
 ## Roadmap
 This section has a bunch of ideas for me to work on, but also for you, the potential contributor!
 Remember to look at the recent branches/commits to see if I’m not working on one of these:
 - user-settings (f.e. auto-download of files, language, formatting, number of submissions shown, config location, ...)
-- improve `info` command (man-page and such)
-- improve `tutorial`
 - easy (automatic?) downloading of files mentioned in exercise description
 - improve the rendering of all html/markdown frankensteins, in descriptions of exercises and exercise-descriptions 
 - add connection time-out to prevent long waiting when IPv6 doesn’t want to work along
 - add support for more languages syntax checkers
 - caching some info for faster navigation and/or autocompletion
 - add indicator to series to mark if all their exercises are completely solved (maybe fetch from html-version)
 - get exercise-names via html-parsing for a submission list to only need 1 API call (instead of 30)
-
-GitHub stuff to figure out:
-- release by tag/release
-- action to check valid version before trying to push, if not valid, make it valid
```

### Comparing `dodonacli-2024.5.15/README.md` & `dodonacli-2024.5.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -132,20 +132,14 @@
 to see if this is indeed the issue.
 
 
 ## Roadmap
 This section has a bunch of ideas for me to work on, but also for you, the potential contributor!
 Remember to look at the recent branches/commits to see if I’m not working on one of these:
 - user-settings (f.e. auto-download of files, language, formatting, number of submissions shown, config location, ...)
-- improve `info` command (man-page and such)
-- improve `tutorial`
 - easy (automatic?) downloading of files mentioned in exercise description
 - improve the rendering of all html/markdown frankensteins, in descriptions of exercises and exercise-descriptions 
 - add connection time-out to prevent long waiting when IPv6 doesn’t want to work along
 - add support for more languages syntax checkers
 - caching some info for faster navigation and/or autocompletion
 - add indicator to series to mark if all their exercises are completely solved (maybe fetch from html-version)
 - get exercise-names via html-parsing for a submission list to only need 1 API call (instead of 30)
-
-GitHub stuff to figure out:
-- release by tag/release
-- action to check valid version before trying to push, if not valid, make it valid
```

### Comparing `dodonacli-2024.5.15/dodonacli/commands/cli_next.py` & `dodonacli-2024.5.16/dodonacli/commands/cli_next.py`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.5.15/dodonacli/commands/display.py` & `dodonacli-2024.5.16/dodonacli/commands/display.py`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.5.15/dodonacli/commands/post.py` & `dodonacli-2024.5.16/dodonacli/commands/post.py`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.5.15/dodonacli/commands/select.py` & `dodonacli-2024.5.16/dodonacli/commands/select.py`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.5.15/dodonacli/commands/submission.py` & `dodonacli-2024.5.16/dodonacli/commands/submission.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,24 +4,18 @@
 
 @click.group(help="Get submission data. Default = view",
              cls=DefaultGroup, default='view', default_if_no_args=True)
 def sub():
     pass
 
 
-def validate_positive_int(ctx, param, value):
-    if value is not None and value < 0:
-        raise click.BadParameter('Number should be greater then 0')
-    return value
-
-
 @click.command(help="Load a submission to the prev_submission file, and display more info about it. "
                     "You can specify a number, else it takes the last submission for that exercise.")
 @click.argument('number',
-                type=int, default=0, callback=validate_positive_int)
+                type=click.IntRange(min=0), default=0)
 def load(number):
     import http.client
     from dodonacli.source import get_data, set_data
 
     # Read configs in
     config = get_data.get_configs()
```

### Comparing `dodonacli-2024.5.15/dodonacli/commands/up.py` & `dodonacli-2024.5.16/dodonacli/commands/up.py`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.5.15/dodonacli/main.py` & `dodonacli-2024.5.16/dodonacli/main.py`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.5.15/dodonacli/source/get_data.py` & `dodonacli-2024.5.16/dodonacli/source/get_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,15 +219,15 @@
     Returns the path of the config home, this directory stores the config.json file
     :return: The path to the config directory
     """
     # The case switch syntax was introduced in python 3.10
     system = platform.system()
     if system == "Linux":
         platform_config_path = os.getenv("XDG_CONFIG_HOME", default=os.getenv("HOME") + "/.config/")
-    elif system == "Darwin":    # aka macOS
+    elif system == "Darwin":  # aka macOS
         platform_config_path = os.path.join(os.getenv("HOME"), "Library/Application Support")
     elif system == "Windows":
         platform_config_path = os.getenv("APPDATA")
     else:
         return os.path.join(os.path.dirname(os.path.abspath(__file__)), "../../config.json")
     return os.path.join(platform_config_path, "DodonaCLI")
 
@@ -253,16 +253,19 @@
             config = validate_config(config)
             if needs_migration:
                 set_data.dump_config(config)
                 print("config.json has been migrated, the old file is at", os.path.abspath(config_file_path))
 
     except FileNotFoundError:
         # Create config dictionary
-        config = {e: None
-                  for e in ["course_id", "course_name", "serie_id", "serie_name", "exercise_id", "exercise_name"]}
+        config: dict[str, str | None] = {
+            e: None
+            for e in ["course_id", "course_name", "serie_id", "serie_name", "exercise_id",
+                      "exercise_name"]
+        }
 
         print("\nThis may be your first time using DodonaCLI, do you wish to follow a short tutorial?")
         answer = input("(yes/no): ")
 
         if answer.lower().startswith("yes"):
             config = interactive_tutorial.start_tutorial(config)
         else:
```

### Comparing `dodonacli-2024.5.15/dodonacli/source/interactive_tutorial.py` & `dodonacli-2024.5.16/dodonacli/source/interactive_tutorial.py`

 * *Files 26% similar despite different names*

```diff
@@ -15,32 +15,30 @@
     Runs the tutorial and asks for API token if it wasn't present yet.
     :param config: dict
     :return: config: dict
     """
     # Clear screen for tutorial
     os.system('cls' if os.name == 'nt' else 'clear')
     print(
-        """
-\n
-Welcome to the Dodona CLI, 
-this tutorial will show you everything you need to interact 
-with Dodona from your terminal.
-"""
+        "Welcome to the Dodona CLI,\n"
+        "this tutorial will show you everything you need to interact\n"
+        "with Dodona from your terminal.\n"
     )
+    input(" <Enter to continue>")
+
+    # Clear previously selected configs
     config['serie_id'], config['serie_name'] = None, None
     config['exercise_name'], config['exercise_name'] = None, None
 
     if "TOKEN" not in config:
+        os.system('cls' if os.name == 'nt' else 'clear')
         pretty_console.console.print(
-            """
-\n\n
-Before we begin, we'll need an API-token to authorize your 
-connection with Dodona. 
-You can find it on your profile page on https://dodona.be
-"""
+            "Before we begin, we'll need an API-token to authorize your\n"
+            "connection with Dodona.\n"
+            "You can find it on your profile page on https://dodona.be\n"
         )
         config = dodonacli.source.get_data.get_api_token(config)
 
     connection = http.client.HTTPSConnection("dodona.be")
     headers = {
         "Content-type": "application/json",
         "Accept": "application/json",
@@ -67,34 +65,33 @@
         if status == 401:
             print("Authorization didn't work, "
                   "please re-enter your API-token and make sure it's correct.")
             config = dodonacli.source.get_data.get_api_token(config)
             set_data.dump_config(config)
 
         else:
-            pretty_console.console.print(
-                "Error connecting to Dodona: " + str(status)
-            )
+            pretty_console.console.print("Error connecting to Dodona: " + str(status))
             pretty_console.console.print("Reason: " + res.reason)
 
         pretty_console.console.print(
             "Tutorial will terminate due to error, "
-            "you can start again with `dodona tutorial`")
+            "you can start again with `dodona tutorial`"
+        )
         exit(-1)
 
     data = res.read()
     connection.close()
 
     return json.loads(data)
 
 
 def tutorial_select_course(config: dict, connection: http.client.HTTPSConnection,
                            headers: dict):
+    os.system('cls' if os.name == 'nt' else 'clear')
     pretty_console.console.print(
-        "\n\n\n"
         "Use the command `dodona display` to show the available courses."
     )
 
     command = input("$ ")
 
     while command.rstrip() != "dodona display":
         print("That was not the right command, please try again")
@@ -102,260 +99,226 @@
 
     connection.request("GET", "/courses?tab=featured", headers=headers)
     json_data = tutorial_handle_connection(config, connection)
 
     pretty_print.print_courses_data(json_data, "Featured courses")
 
     pretty_console.console.print(
-        """
-Select now "The Coder's Apprenctice" with `dodona select` + 
-the courses id, or (distinct part of) the courses name
-"""
+        "\nSelect now \"The Coder's Apprenctice\" with `dodona select` + the courses id,"
+        "\nor (distinct part of) the courses name"
     )
     command = input("$ ")
 
-    while not command.rstrip().startswith("dodona select"):
-        print("That was not the right command, please try again")
+    while not command.lstrip().startswith("dodona select"):
+        print("\tThat was not the right command, please try again")
         command = input("$ ")
 
-    if (len(command.split()) < 3
-            or command.split()[2] != "296"
-            and command.split()[2].lower() not in "The Coder's Apprentice".lower()):
+    dod, sel, course = command.split()
+    if (len(command.split()) < 3 or
+            course != "296" and course.lower() not in "The Coder's Apprentice".lower()):
         pretty_console.console.print(
-            """
-Watch out, you used a wrong id or name to select 
-"The Coder's Apprentice"!\n
-The tutorial will continue as if you selected it right, 
-but pay attention next time.
-"""
+            "\t[red]Watch out[/], you used a wrong id or name to select"
+            "\"The Coder's Apprentice\"!\n"
+            "\tThe tutorial will continue as if you selected it right,"
+            "but pay attention next time."
         )
 
     config['course_id'] = 296
     config['course_name'] = "The Coder's Apprentice"
 
     pretty_console.console.print(
-        """
-\n
-The course is now selected, 
-use `dodona status` to view your selection:
-"""
+        "The course is now selected, let's continue with selecting an exercise-series.\n"
     )
-    command = input("$ ")
-
-    while not command.rstrip() == "dodona status":
-        print("That was not the right command, please try again")
-        command = input("$ ")
-
-    pretty_print.print_status(config)
-    print("Fantastic, let's move on to selecting an exercise series.")
+    input(" <Enter to continue>")
 
     return config
 
 
 def tutorial_select_series(config: dict, connection: http.client.HTTPSConnection,
                            headers: dict):
+    os.system('cls' if os.name == 'nt' else 'clear')
     pretty_console.console.print(
-        """
-\n\n\n
-Use the command `dodona display` to show the available 
-exercise-series.
-"""
+        "Use the command `dodona display` to show the available exercise-series."
     )
     command = input("$ ")
 
-    while command.rstrip() != "dodona display":
-        print("That was not the right command, please try again")
+    while command.strip() != "dodona display":
+        print("\nThat was not the right command, please try again")
         command = input("$ ")
 
     connection.request(
         "GET", "/courses/" + str(config['course_id']) + '/series',
         headers=headers)
     json_data = tutorial_handle_connection(config, connection)
 
-    # To prevent the screen being blasted with a lot of text, 
+    # To prevent the screen being blasted with a lot of text,
     # only print out the first 6 exercise series
     pretty_print.print_series_data(json_data[:6])
 
     pretty_console.console.print(
-        """
-Select now "2. Using Python" with `dodona select` + 
-the series' id, or (distinct part of) the series' name.
-"""
+        "Select now \"2. Using Python\" with `dodona select` + the series' id,"
+        "\nor (distinct part of) the series' name."
     )
     command = input("$ ")
 
-    while not command.rstrip().startswith("dodona select"):
-        print("That was not the right command, please try again")
+    while not command.lstrip().startswith("dodona select"):
+        print("\nThat was not the right command, please try again")
         command = input("$ ")
 
+    dod, sel, series = command.split()
     if (len(command.split()) < 3
-            or command.split()[2] != "2592"
-            and command.split()[2].lower() not in "2. Using Python".lower()):
+            or series != "2592" and series.lower() not in "2. Using Python".lower()):
         pretty_console.console.print(
-            """
-Watch out, you used a wrong id or name to select 
-"2. Using Python"!\n
-The tutorial will continue as if you selected it right, 
-but pay attention next time.
-"""
+            "\tWatch out, you used a wrong id or name to select \"2. Using Python\"!\n"
+            "\tThe tutorial will continue as if you selected it right,"
+            "but pay attention next time."
         )
 
     config['serie_id'] = 2592
     config['serie_name'] = "2. Using Python"
 
     pretty_console.console.print(
-        """
-\n
-The exercise-series is now selected, use `dodona status` 
-to view your selection:
-"""
+        "\nWith the exercise-series now selected, it's time to introcude `dodona status`, "
+        "give it a try!"
     )
     command = input("$ ")
 
-    while not command.rstrip() == "dodona status":
-        print("That was not the right command, please try again")
+    while not command.strip() == "dodona status":
+        print("\tThat was not the right command, please try again")
         command = input("$ ")
 
     pretty_print.print_status(config)
-    print("Fantastic, let's move on to selecting an exercise.")
+    print("Fantastic, let's move on to selecting an exercise.\n")
+    input(" <Enter to continue>")
 
     return config
 
 
 def tutorial_select_exercise(config: dict, connection: http.client.HTTPSConnection,
                              headers: dict):
+    os.system('cls' if os.name == 'nt' else 'clear')
     pretty_console.console.print(
-        """
-\n\n\n
-Use the command `dodona display` to show the available exercises.
-"""
+        "Use the command `dodona display` to show the available exercises."
     )
     command = input("$ ")
 
-    while command.rstrip() != "dodona display":
+    while command.strip() != "dodona display":
         print("That was not the right command, please try again")
         command = input("$ ")
 
     connection.request(
-        "GET", "/series/" + str(config['serie_id']) + '/activities',
-        headers=headers)
+        "GET",
+        "/series/" + str(config['serie_id']) + '/activities',
+        headers=headers
+    )
     json_data = tutorial_handle_connection(config, connection)
 
     pretty_print.print_exercise_data(json_data)
 
     pretty_console.console.print(
-        """
-Select now "Hello, World!" with `dodona select` + 
-the series' id, or (distinct part of) the series' name.
-"""
+        "Select now \"Hello, World!\" with `dodona select` + the series' id,\n"
+        "or (distinct part of) the series' name."
     )
     command = input("$ ")
 
-    while not command.rstrip().startswith("dodona select"):
+    while not command.lstrip().startswith("dodona select"):
         print("That was not the right command, please try again")
         command = input("$ ")
 
+    dod, sel, exercise = command.split()
     if (len(command.split()) < 3
-            or command.split()[2] != "1399231809"
-            and command.split()[2].lower() not in "Hello, World!".lower()):
+            or exercise != "1399231809" and exercise.lower() not in "Hello, World!".lower()):
         pretty_console.console.print(
-            """
-Watch out, you used a wrong id or name to select 
-"2. Using Python"!\n
-The tutorial will continue as if you selected it right, 
-but pay attention next time.
-"""
+            "\tWatch out, you used a wrong id or name to select \"2. Using Python\"!\n"
+            "\tThe tutorial will continue as if you selected it right, "
+            "but pay attention next time."
         )
 
     config['exercise_id'] = 1399231809
     config['exercise_name'] = "Hello, World!"
 
     # This exercise has boilerplate code
     with open('boilerplate.py', 'w') as boilerplate:
         boilerplate.write(json_data[5]['boilerplate'])
-    print(
-        """
-This exercise has some boilerplate code attached to it, 
-you can view it in the boilerplate file, or here:\n|\t        
-""" + json_data[5]['boilerplate']
-    )
 
     pretty_console.console.print(
-        """
-\n
-The exercise is now selected, 
-use `dodona status` to view your selection:
-"""
+        "This exercise has some boilerplate code attached to it,\n"
+        "here is its content:\n|\t"
+        + json_data[5]['boilerplate'].strip()
+        + "\nNormally, this file will be saved to your disk, "
+          "with the file-extension of the programming-language of the exercise.\n"
     )
-    command = input("$ ")
 
-    while not command.rstrip() == "dodona status":
-        print("That was not the right command, please try again.")
-        command = input("$ ")
-
-    pretty_print.print_status(config)
-    print("Fantastic, let's move on to viewing an exercise description.")
+    pretty_console.console.print(
+        "The exercise is now selected, let's move on to viewing an exercise description.\n"
+    )
+    input(" <Enter to continue>")
 
     return config
 
 
 def tutorial_view_exercise(config: dict, connection: http.client.HTTPSConnection,
                            headers: dict):
+    os.system('cls' if os.name == 'nt' else 'clear')
     pretty_console.console.print(
-        """
-\n\n\n
-Use the command `dodona display` to show the description of the 
-exercise.
-"""
+        "Use the command `dodona display` to show the description of the exercise."
     )
     command = input("$ ")
 
-    while command.rstrip() != "dodona display":
+    while command.strip() != "dodona display":
         print("That was not the right command, please try again")
         command = input("$ ")
 
-    connection.request("GET", "/courses/" + str(config['course_id'])
-                       + "/series/" + str(config['serie_id'])
-                       + '/activities/' + str(config['exercise_id']),
-                       headers=headers)
-    json_data = tutorial_handle_connection(config, connection)
+    connection.request(
+        "GET",
+        f"/courses/{str(config['course_id'])}"
+        + f"/series/{str(config['serie_id'])}"
+        + f"/activities/{str(config['exercise_id'])}",
+        headers=headers)
 
+    json_data = tutorial_handle_connection(config, connection)
     pretty_print.print_exercise(json_data, config['TOKEN'])
 
+    input(" <Enter to continue>")
+
 
 def tutorial_post_exercise(config: dict, connection: http.client.HTTPSConnection,
                            headers: dict):
+    os.system('cls' if os.name == 'nt' else 'clear')
     pretty_console.console.print(
-        """
-\n\n\n
-Now you can post the solution. You don't need to write any code 
-for it, as it is already writtin in the 'boilerplate'-file. 
-You can post it by writing `dodona post <SOLUTION_FILE_NAME>`.
-Replace <SOLUTION_FILE_NAME> with the correct file-name, 
-in this case 'boilerplate'.
-"""
+        "Now you can post the solution. You don't need to write any code for this exercise, \n"
+        "as it is already writtin in the 'boilerplate.py'-file.\n"
+        "You can post it with the command `dodona post <SOLUTION_FILE_NAME>`.\n"
+        "Replace <SOLUTION_FILE_NAME> with the correct file-name, in this case 'boilerplate.py'."
     )
     command = input("$ ")
 
-    while command.rstrip() != "dodona post boilerplate":
+    while command.strip() != "dodona post boilerplate.py":
         print("That was not the right command, please try again")
         command = input("$ ")
 
-    with open('boilerplate', 'r') as solution_file:
-        set_data.post_solution(solution_file.read(), connection, headers, config['course_id'], config['exercise_id'])
+    set_data.post_solution(
+        "print( \"Hello, world!\" )",
+        connection, headers, config['course_id'], config['exercise_id']
+    )
+
+    pretty_console.console.print(
+        "Nice, programmed that like a pro.\n"
+        "You're nearly done with this tutorial, I want to show you one last thing. \n"
+    )
+    input(" <Enter to continue>")
 
 
 def tutorial_conclude(config: dict) -> dict:
+    os.system('cls' if os.name == 'nt' else 'clear')
     pretty_console.console.print(
-        """
-Almost done, now deselect everything. You can do this with the 
-'up' command + a selection from [1|2|3|all|top]. The numbers specify 
-the amount of levels you'll deselect, while all/top deselects 
-everything at once.
-"""
+        "It's time deselect everything. You can do this with the "
+        "'up' command + a selection from [1|2|3|all|top].\n"
+        "The numbers specify the amount of levels you'll deselect, while all/top deselects "
+        "everything at once."
     )
 
     command = input("$ ")
 
     # Parse input
     while not command.rstrip().startswith("dodona up"):
         print("That wasn't the right command, please try again.")
@@ -366,28 +329,27 @@
     all_configs.remove("TOKEN")
 
     for conf in all_configs:
         config[conf] = None
 
     # Print the right message
     amount = command.replace("dodona up", "").strip()
+    print()
     if amount in ("all", "top", "3"):
         print("Deselected everything")
     elif amount.isnumeric():
         print("Deselected everything to save on time. Normally this would "
-              "deselect " + amount + "levels")
+              "deselect " + amount + " levels")
     else:
         print("You didn't enter a valid amount, but I'll let it slip now.\n"
               "Deselected everything.")
 
     # End of tutorial
     pretty_console.console.print(
-        """
-Remember you can always use `dodona [subcommand] --help` to get 
-help with all the subcommands. Additionally there is a manual-page 
-you can download from [link=https://www.github.com/BWindey/DodonaCLI]
-GitHub[/link]. You can also find a completion script there.
-Installation instructions for both can be found in the README.md.
-"""
+        "\nRemember you can always use `dodona \[subcommand\] --help` to get "
+        "help with all the subcommands.\n"
+        "Additionally there is a manual-page you can download "
+        "from https://www.github.com/BWindey/DodonaCLI .\n"
+        "I would strongly encourage you to read through the README there as well."
     )
 
     return config
```

### Comparing `dodonacli-2024.5.15/dodonacli/source/pretty_print.py` & `dodonacli-2024.5.16/dodonacli/source/pretty_print.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,16 @@
     pretty_console.console.print(f'\n[u bright_blue]{title}[/]')
     for course in display_data:
         pretty_console.console.print(
             (prefixes.get(course[0]) or "\t") +
             f"{course[0].ljust(max_course_id_length)}: "
             f"[bold]{course[1].ljust(max_course_name_length)}[/]\tby {course[2]}"
         )
+    # Newline for clarity
+    print()
 
 
 def print_series_data(json_data: dict, force: bool = False, prefixes: dict = None):
     """
     Print out the exercise-series in json_data in a neat way.
     :param json_data: Json object with data about Dodona exercise-series
     :param force: Boolean to decide if the series description has to be printed, or only a link to it
@@ -189,14 +191,15 @@
 
         pretty_console.console.print(
             (prefixes.get(exercise['id']) or "\t")
             + f"{exercise['id'].ljust(max_exercise_id_length)}: "
             + f"[bold]{exercise['name'].ljust(max_exercise_name_length)}[/]\t"
             + solve_status
         )
+    # Newline for clarity
     print()
 
 
 def print_exercise(json_data: dict, token: str, force: bool = False):
     """
     Print out the exercise-description.
     Needs to call the Dodona sandbox and convert HTML to text.
@@ -208,15 +211,17 @@
     if json_data['type'] == 'ContentPage':
         pretty_console.console.print(
             "\nNo need to program anything this time, but you'll have to go read this and mark it as read:\n"
             + json_data['url'].replace(".json", "") + '\n'
         )
 
     elif not force:
-        pretty_console.console.print("\nYou can find the description at \n" + json_data['description_url'] + '\n')
+        pretty_console.console.print(
+            f"\nYou can find the exercise description at \n{json_data['description_url']}\n"
+        )
 
     else:
         # Print the HTML with warnings
         warning = (
                 "\n[u bold bright_red]WARNING:[/] the description may be incorrect, "
                 "DO NOT rely on this for exams and tests!\n"
                 "View in browser: " + json_data['description_url'] + '\n'
@@ -254,27 +259,33 @@
 def print_result(json_results: dict):
     """
     Print out the results of a submission in a neat way
     :param json_results: json object with data about a submission
     """
     if json_results['accepted']:
         # Everything passed, well done!
-        pretty_console.console.print("[bold bright_green]All tests passed![/] You can continue to next exercise.")
+        pretty_console.console.print(
+            "[bold bright_green]All tests passed![/] You can continue to next exercise."
+        )
     else:
         pretty_console.console.print(submission_data_handler.submission_data_handler(json_results))
 
 
 def print_status(config: dict):
     """
     Print out the current selection of course, exercise-series and exercise.
     :param config: Dictionary with the configs
     """
+    course_string = config['course_name']
+    if config['course_id'] is not None:
+        course_string += f" ({config['course_id']})"
+
     pretty_console.console.print(
         f"\n[u bright_blue]Status:[/]\n"
-        f"\t{'Course: '.ljust(10)}{config['course_name']}\n"
+        f"\t{'Course: '.ljust(10)}{course_string}\n"
         f"\t{'Series: '.ljust(10)}{config['serie_name']}\n"
         f"\t{'Exercise: '.ljust(10)}{config['exercise_name']}\n"
     )
 
 
 def print_exercise_submissions(json_data: dict):
     """
@@ -294,15 +305,15 @@
         if submission['status'] in ("memory limit exceeded", "geheugenlimiet overschreden"):
             status += "\n\t\t\tWow, how did you do that?"
 
         pretty_console.console.print(
             f"\t{accepted_emoji}  [link={submission['url'].rstrip('.json')}]#{len(json_data) - i: <2}[/link]"
             f"\t{status}\t"
         )
-
+    # Newline for clarity
     print()
 
 
 def print_all_submissions(connection: http.client.HTTPSConnection, headers: dict, json_data: dict):
     """
     Print out a list of the latest 30 submissions for the user, userwide (not tied to an exercise).
     Makes extra requests to Dodona to get the name of the exercises of the submissions
@@ -339,8 +350,9 @@
         pretty_console.console.print(
             f"\t{accepted_emoji}  [link={submission['url'].rstrip('.json')}]#{len(json_data) - i: <2}[/link]"
             f"\t{status: <25}"
             f"\t{exercise_name}"
         )
 
     connection.close()
+    # Newline for clarity
     print()
```

### Comparing `dodonacli-2024.5.15/dodonacli/source/set_data.py` & `dodonacli-2024.5.16/dodonacli/source/set_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,24 +125,24 @@
 
     if is_christmas_season:
         return christmas_spinner
 
     return random.choice(selection_spinners)
 
 
-def save_to_file(name: str, id: int, content: str, extension: str = ""):
+def save_to_file(name: str, submission_id: int, content: str, extension: str = ""):
     """
     Save code to a file in the users current working directory.
     The resulting file name: {name}_{id}{extension}
     :param name: Name of the file
-    :param id: ID to add to the name of file
+    :param submission_id: ID to add to the name of file
     :param content: Content to save in the file
     :param extension: Optional file-extension, has to include the '.'
     """
     name = name.replace(' ', '-')
-    file_name = f"{name}_{id}{extension}"
+    file_name = f"{name}_{submission_id}{extension}"
 
     with open(file_name, "w") as code_file:
         code_file.write(content)
 
     print(f"\nCode from your submission for {name} is now saved in:\n"
-          f"\t{name}_{id}{extension}\n")
+          f"\t{name}_{submission_id}{extension}\n")
```

### Comparing `dodonacli-2024.5.15/dodonacli/source/submission_data_handler.py` & `dodonacli-2024.5.16/dodonacli/source/submission_data_handler.py`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.5.15/dodonacli/source/syntax_checker.py` & `dodonacli-2024.5.16/dodonacli/source/syntax_checker.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,92 +31,104 @@
         return True
     except subprocess.CalledProcessError as cpe:
         print(f"Syntax Error in Bash script: {str(cpe)}")
         return False
     except FileNotFoundError:
         # This will only occur if shellcheck isn't installed.
         # Click will detect that the user gave an invalid file before this function is called
-        print("\nTo check the syntax, 'shellcheck' is called with your file. It appears however, that "
-              "shellcheck isn't installed on your system. Please install it: https://www.shellcheck.net/")
+        print(
+            "\nTo check the syntax, 'shellcheck' is called with your file. "
+            "It appears however, that shellcheck isn't installed on your system. \n"
+            "Please install it: https://www.shellcheck.net/\n"
+        )
         return False
     except Exception as e:
         print("\nNo idea what's going wrong, but something definitly is going wrong:\n" + str(e))
         return False
 
 
 def check_python_syntax(file: str) -> bool:
     try:
         with open(file, 'r') as content:
             compile(content.read(), file, 'exec')
         return True
     except SyntaxError as se:
-        print(f"\nSyntax error in Python file:\n{se}")
+        print(f"\nSyntax error in Python file:\n{se}\n")
     except Exception as e:
         print("\nNo idea what's going wrong, but something definitly is going wrong:\n" + str(e))
         return False
 
 
 def check_java_syntax(file: str) -> bool:
     temp_dir = tempfile.mkdtemp()
     try:
         directory = os.path.dirname(file)
-        java_files = [file for file in os.listdir(directory) if file.endswith('.java') and not "test" in file.lower()]
+        java_files = [file for file in os.listdir(directory) if file.endswith('.java') and "test" not in file.lower()]
         if not java_files:
             return False  # No Java files found in the directory
 
         # Construct the list of Java files with their full paths
         java_files_with_paths = [os.path.join(directory, file) for file in java_files]
 
         subprocess.run(['javac', '-d', temp_dir] + java_files_with_paths, check=True)
 
         # Remove temporary directory
         shutil.rmtree(temp_dir, ignore_errors=True)
         return True
 
-    except subprocess.CalledProcessError as cpe:
+    except subprocess.CalledProcessError:
         # This error will happen if there was something wrong with the Java syntax
         return False
 
     except FileNotFoundError:
         # This will only occur if javac isn't installed.
         # Click will detect that the user gave an invalid file before this function is called
-        print("\nTo check the syntax, 'javac' is called with your file. It appears however, that "
-              "the Java compiler isn't installed on your system. Please install it: https://openjdk.org/install/")
+        print(
+            "\nTo check the syntax, 'javac' is called with your file. "
+            "It appears however, that the Java compiler isn't installed on your system.\n"
+            "Please install it: https://openjdk.org/install/\n"
+        )
         return False
     except Exception as e:
         print("\nNo idea what's going wrong, but something definitly is going wrong:\n" + str(e))
         return False
     finally:
         shutil.rmtree(temp_dir, ignore_errors=True)
 
 
 def check_javascript_syntax(file: str) -> bool:
     try:
         subprocess.run(['node', '-c', file], check=True)
         return True
-    except subprocess.CalledProcessError as cpe:
+    except subprocess.CalledProcessError:
         return False
     except FileNotFoundError:
         # This will only occur if jshint isn't installed.
         # Click will detect that the user gave an invalid file before this function is called
-        print("\nTo check the syntax, 'node' is called with your file. It appears however, that "
-              "this program isn't installed on your system. Please install it: https://nodejs.org/en/learn/getting-started/how-to-install-nodejs")
+        print(
+            "\nTo check the syntax, 'node' is called with your file. "
+            "It appears however, that this program isn't installed on your system.\n"
+            "Please install it: https://nodejs.org/en/learn/getting-started/how-to-install-nodejs\n"
+        )
         return False
     except Exception as e:
         print("\nNo idea what's going wrong, but something definitly is going wrong:\n" + str(e))
         return False
 
 
 def check_haskell_syntax(file: str) -> bool:
     try:
         # TODO: enable compiling without main function present
         subprocess.run(['ghc', '-fno-code', '-v0', file], check=True)
         return True
-    except subprocess.CalledProcessError as cpe:
+    except subprocess.CalledProcessError:
         return False
     except FileNotFoundError:
-        print("\nTo check the syntax, 'ghc' is called with your file. It appears however, that "
-              "this program isn't installed on your system. Please install it: https://www.haskell.org/ghcup/")
+        print(
+            "\nTo check the syntax, 'ghc' is called with your file. "
+            "It appears however, that this program isn't installed on your system.\n"
+            "Please install it: https://www.haskell.org/ghcup/\n"
+        )
         return False
     except Exception as e:
         print("\nNo idea what's going wrong, but something definitly is going wrong:\n" + str(e))
         return False
```

### Comparing `dodonacli-2024.5.15/man-page/dodonacli.1` & `dodonacli-2024.5.16/man-page/dodonacli.1`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.5.15/man-page/dodonacli.1.gz` & `dodonacli-2024.5.16/man-page/dodonacli.1.gz`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.5.15/pyproject.toml` & `dodonacli-2024.5.16/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "DodonaCLI"
-version = '2024.5.15'
+version = '2024.5.16'
 authors = [
     { name = "Bram Windey", email = "windey.bram@gmail.com" },
 ]
 description = "A CLI tool for Dodona"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
@@ -19,15 +19,15 @@
 ]
 dependencies = [
     "bs4",
     "click",
     "click-default-group",
     "markdownify",
     "packaging",
-    "pkg_info",
+    "pkg-info",
     "rich"
 ]
 keywords = ["dodona", "cli"]
 
 
 [project.scripts]
 dodona = "dodonacli.main:main"
```

