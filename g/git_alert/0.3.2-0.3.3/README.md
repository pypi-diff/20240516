# Comparing `tmp/git_alert-0.3.2.tar.gz` & `tmp/git_alert-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_alert-0.3.2.tar", max compression
+gzip compressed data, was "git_alert-0.3.3.tar", max compression
```

## Comparing `git_alert-0.3.2.tar` & `git_alert-0.3.3.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1077 2024-05-14 10:21:51.084584 git_alert-0.3.2/LICENSE
--rw-r--r--   0        0        0     4908 2024-05-14 10:21:51.084584 git_alert-0.3.2/README.md
--rw-r--r--   0        0        0      142 2024-05-14 10:21:51.084584 git_alert-0.3.2/git_alert/__init__.py
--rw-r--r--   0        0        0      883 2024-05-14 10:21:51.084584 git_alert-0.3.2/git_alert/__main__.py
--rw-r--r--   0        0        0     1348 2024-05-14 10:21:51.084584 git_alert-0.3.2/git_alert/argument_parser.py
--rw-r--r--   0        0        0     1619 2024-05-14 10:21:51.088584 git_alert-0.3.2/git_alert/configuration.py
--rw-r--r--   0        0        0     1285 2024-05-14 10:21:51.088584 git_alert-0.3.2/git_alert/repositories.py
--rw-r--r--   0        0        0      983 2024-05-14 10:21:51.088584 git_alert-0.3.2/git_alert/scripts/git_alert.py
--rw-r--r--   0        0        0     1552 2024-05-14 10:21:51.088584 git_alert-0.3.2/git_alert/traverse.py
--rw-r--r--   0        0        0      658 2024-05-14 10:21:51.088584 git_alert-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     5392 1970-01-01 00:00:00.000000 git_alert-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-05-16 13:49:05.208022 git_alert-0.3.3/LICENSE
+-rw-r--r--   0        0        0     4908 2024-05-16 13:49:05.208022 git_alert-0.3.3/README.md
+-rw-r--r--   0        0        0      142 2024-05-16 13:49:05.208022 git_alert-0.3.3/git_alert/__init__.py
+-rw-r--r--   0        0        0     1341 2024-05-16 13:49:05.208022 git_alert-0.3.3/git_alert/__main__.py
+-rw-r--r--   0        0        0     1348 2024-05-16 13:49:05.208022 git_alert-0.3.3/git_alert/argument_parser.py
+-rw-r--r--   0        0        0     1619 2024-05-16 13:49:05.208022 git_alert-0.3.3/git_alert/configuration.py
+-rw-r--r--   0        0        0     2098 2024-05-16 13:49:05.208022 git_alert-0.3.3/git_alert/display.py
+-rw-r--r--   0        0        0      641 2024-05-16 13:49:05.208022 git_alert-0.3.3/git_alert/repositories.py
+-rw-r--r--   0        0        0     1477 2024-05-16 13:49:05.208022 git_alert-0.3.3/git_alert/scripts/git_alert.py
+-rw-r--r--   0        0        0     1552 2024-05-16 13:49:05.208022 git_alert-0.3.3/git_alert/traverse.py
+-rw-r--r--   0        0        0      675 2024-05-16 13:49:05.208022 git_alert-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     5431 1970-01-01 00:00:00.000000 git_alert-0.3.3/PKG-INFO
```

### Comparing `git_alert-0.3.2/LICENSE` & `git_alert-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `git_alert-0.3.2/README.md` & `git_alert-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `git_alert-0.3.2/git_alert/__main__.py` & `git_alert-0.3.3/git_alert/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,50 @@
 import sys
 
 from git_alert.argument_parser import argument_parser
 from git_alert.configuration import ReadConfig, System
+from git_alert.display import Report
 from git_alert.repositories import Repositories
 from git_alert.traverse import GitAlert
 
 args = argument_parser(sys.argv[1:])
 repos = Repositories()
 
 # Create System class
 system = System()
 
 # Read configuration file:
 config = ReadConfig(system, config=args.config)
 
+
 # Get the path, only_dirty and ignore from the configuration class:
 path = config.path
 only_dirty = config.only_dirty
 ignore = config.ignore
 
 # Override the configuration file with the command line arguments:
 if args.path:
     path = args.path
 if args.only_dirty:
     only_dirty = args.only_dirty
 if args.ignore:
     ignore = args.ignore
 
+report = Report(repos=repos, only_dirty=only_dirty)
+
 alert = GitAlert(pth=path, ignore=ignore, repos=repos)
 
-alert.traverse(path)
-alert.check()
-alert.repos.display(only_dirty=only_dirty)
-alert.repos.summary()
+with report.console.status("Indexing repositories...", spinner="bouncingBall"):
+    alert.traverse(path)
+print("✅ Successfully indexed.")
+
+with report.console.status("Checking repositories...", spinner="bouncingBall"):
+    alert.check()
+print("✅ Successfully checked.")
+
+report.create_long_report_table()
+report.populate_long_report_table()
+report.display_long_report()
+
+report.create_summary_table()
+report.populate_short_table()
+report.display_summary_report()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `git_alert-0.3.2/git_alert/argument_parser.py` & `git_alert-0.3.3/git_alert/argument_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         "-i",
         "--ignore",
         type=ignore_paths,
         default=[],
         help="colon separated list of paths to ignore",
     )
 
-    parser.add_argument("-v", "--version", action="version", version="%(prog)s 0.3.1")
+    parser.add_argument("-v", "--version", action="version", version="%(prog)s 0.3.3")
 
     parser.add_argument(
         "-c",
         "--config",
         type=Path,
         help="path to the configuration file",
     )
```

### Comparing `git_alert-0.3.2/git_alert/configuration.py` & `git_alert-0.3.3/git_alert/configuration.py`

 * *Files identical despite different names*

### Comparing `git_alert-0.3.2/git_alert/traverse.py` & `git_alert-0.3.3/git_alert/traverse.py`

 * *Files identical despite different names*

### Comparing `git_alert-0.3.2/pyproject.toml` & `git_alert-0.3.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [tool.poetry]
 name = "git_alert"
-version = "0.3.2"
+version = "0.3.3"
 
 description = "Checks a given path and its sub-directories for dirty git repositories."
 authors = ["Simon Antonius Lauer <simon.lauer@posteo.de>"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "git_alert"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
+rich = "^13.7.1"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.1.1"
 pytest-cov = "^5.0.0"
```

### Comparing `git_alert-0.3.2/PKG-INFO` & `git_alert-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: git_alert
-Version: 0.3.2
+Version: 0.3.3
 Summary: Checks a given path and its sub-directories for dirty git repositories.
 License: MIT
 Author: Simon Antonius Lauer
 Author-email: simon.lauer@posteo.de
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: rich (>=13.7.1,<14.0.0)
 Description-Content-Type: text/markdown
 
 # Git Alert
 
 <hr>
 
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
```

