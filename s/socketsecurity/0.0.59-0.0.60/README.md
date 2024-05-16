# Comparing `tmp/socketsecurity-0.0.59.tar.gz` & `tmp/socketsecurity-0.0.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socketsecurity-0.0.59.tar", last modified: Thu May 16 10:05:13 2024, max compression
+gzip compressed data, was "socketsecurity-0.0.60.tar", last modified: Thu May 16 10:14:37 2024, max compression
```

## Comparing `socketsecurity-0.0.59.tar` & `socketsecurity-0.0.60.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 10:05:13.629278 socketsecurity-0.0.59/
--rw-r--r--   0 douglascoburn   (501) staff       (20)      771 2024-05-16 10:05:13.629091 socketsecurity-0.0.59/PKG-INFO
--rw-r--r--   0 douglascoburn   (501) staff       (20)       21 2024-05-15 04:22:36.000000 socketsecurity-0.0.59/README.md
--rw-r--r--   0 douglascoburn   (501) staff       (20)     1025 2024-05-16 10:03:45.000000 socketsecurity-0.0.59/pyproject.toml
--rw-r--r--   0 douglascoburn   (501) staff       (20)       38 2024-05-16 10:05:13.629317 socketsecurity-0.0.59/setup.cfg
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 10:05:13.618192 socketsecurity-0.0.59/socketsecurity/
--rw-r--r--   0 douglascoburn   (501) staff       (20)       98 2024-05-16 10:04:37.000000 socketsecurity-0.0.59/socketsecurity/__init__.py
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 10:05:13.628281 socketsecurity-0.0.59/socketsecurity/core/
--rw-r--r--   0 douglascoburn   (501) staff       (20)    26034 2024-05-16 10:03:39.000000 socketsecurity-0.0.59/socketsecurity/core/__init__.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)     9282 2024-05-16 08:29:16.000000 socketsecurity-0.0.59/socketsecurity/core/classes.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)      626 2024-04-29 13:52:20.000000 socketsecurity-0.0.59/socketsecurity/core/exceptions.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)    11342 2024-05-16 07:53:25.000000 socketsecurity-0.0.59/socketsecurity/core/github.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)    11019 2024-05-16 09:57:17.000000 socketsecurity-0.0.59/socketsecurity/core/glitlab.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)    68147 2024-05-16 10:03:15.000000 socketsecurity-0.0.59/socketsecurity/core/issues.py
--rw-r--r--   0 douglascoburn   (501) staff       (20) 17442610 2024-05-06 19:45:31.000000 socketsecurity-0.0.59/socketsecurity/core/licenses.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)    11849 2024-05-15 05:15:37.000000 socketsecurity-0.0.59/socketsecurity/core/messages.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)     5641 2024-05-16 09:29:23.000000 socketsecurity-0.0.59/socketsecurity/socketcli.py
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 10:05:13.628873 socketsecurity-0.0.59/socketsecurity.egg-info/
--rw-r--r--   0 douglascoburn   (501) staff       (20)      771 2024-05-16 10:05:13.000000 socketsecurity-0.0.59/socketsecurity.egg-info/PKG-INFO
--rw-r--r--   0 douglascoburn   (501) staff       (20)      561 2024-05-16 10:05:13.000000 socketsecurity-0.0.59/socketsecurity.egg-info/SOURCES.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)        1 2024-05-16 10:05:13.000000 socketsecurity-0.0.59/socketsecurity.egg-info/dependency_links.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)       59 2024-05-16 10:05:13.000000 socketsecurity-0.0.59/socketsecurity.egg-info/entry_points.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)       38 2024-05-16 10:05:13.000000 socketsecurity-0.0.59/socketsecurity.egg-info/requires.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)       15 2024-05-16 10:05:13.000000 socketsecurity-0.0.59/socketsecurity.egg-info/top_level.txt
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 10:14:37.832550 socketsecurity-0.0.60/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      771 2024-05-16 10:14:37.832305 socketsecurity-0.0.60/PKG-INFO
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       21 2024-05-15 04:22:36.000000 socketsecurity-0.0.60/README.md
+-rw-r--r--   0 douglascoburn   (501) staff       (20)     1025 2024-05-16 10:14:30.000000 socketsecurity-0.0.60/pyproject.toml
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       38 2024-05-16 10:14:37.832720 socketsecurity-0.0.60/setup.cfg
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 10:14:37.814880 socketsecurity-0.0.60/socketsecurity/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       98 2024-05-16 10:04:37.000000 socketsecurity-0.0.60/socketsecurity/__init__.py
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 10:14:37.831004 socketsecurity-0.0.60/socketsecurity/core/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    26034 2024-05-16 10:14:30.000000 socketsecurity-0.0.60/socketsecurity/core/__init__.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)     9282 2024-05-16 08:29:16.000000 socketsecurity-0.0.60/socketsecurity/core/classes.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      626 2024-04-29 13:52:20.000000 socketsecurity-0.0.60/socketsecurity/core/exceptions.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    11342 2024-05-16 07:53:25.000000 socketsecurity-0.0.60/socketsecurity/core/github.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    11019 2024-05-16 09:57:17.000000 socketsecurity-0.0.60/socketsecurity/core/glitlab.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    68147 2024-05-16 10:03:15.000000 socketsecurity-0.0.60/socketsecurity/core/issues.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20) 17442610 2024-05-06 19:45:31.000000 socketsecurity-0.0.60/socketsecurity/core/licenses.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    11849 2024-05-15 05:15:37.000000 socketsecurity-0.0.60/socketsecurity/core/messages.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)     5976 2024-05-16 10:13:50.000000 socketsecurity-0.0.60/socketsecurity/socketcli.py
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 10:14:37.831235 socketsecurity-0.0.60/socketsecurity.egg-info/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      771 2024-05-16 10:14:37.000000 socketsecurity-0.0.60/socketsecurity.egg-info/PKG-INFO
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      561 2024-05-16 10:14:37.000000 socketsecurity-0.0.60/socketsecurity.egg-info/SOURCES.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)        1 2024-05-16 10:14:37.000000 socketsecurity-0.0.60/socketsecurity.egg-info/dependency_links.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       59 2024-05-16 10:14:37.000000 socketsecurity-0.0.60/socketsecurity.egg-info/entry_points.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       38 2024-05-16 10:14:37.000000 socketsecurity-0.0.60/socketsecurity.egg-info/requires.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       15 2024-05-16 10:14:37.000000 socketsecurity-0.0.60/socketsecurity.egg-info/top_level.txt
```

### Comparing `socketsecurity-0.0.59/PKG-INFO` & `socketsecurity-0.0.60/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketsecurity
-Version: 0.0.59
+Version: 0.0.60
 Summary: Socket Security CLI for CI/CD
 Author-email: Douglas Coburn <douglas@socket.dev>
 Maintainer-email: Douglas Coburn <douglas@socket.dev>
 Project-URL: Homepage, https://socket.dev
 Keywords: socketsecurity,socket.dev,sca,oss,security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `socketsecurity-0.0.59/pyproject.toml` & `socketsecurity-0.0.60/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "socketsecurity"
-version = "0.0.59"
+version = "0.0.60"
 requires-python = ">= 3.9"
 dependencies = [
     'requests',
     'mdutils',
     'prettytable',
     'argparse'
 ]
```

### Comparing `socketsecurity-0.0.59/socketsecurity/core/__init__.py` & `socketsecurity-0.0.60/socketsecurity/core/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 )
 import platform
 from glob import glob
 import time
 
 
 __author__ = 'socket.dev'
-__version__ = '0.0.59'
+__version__ = '0.0.60'
 __all__ = [
     "Core",
     "log",
     "__version__"
 ]
```

### Comparing `socketsecurity-0.0.59/socketsecurity/core/classes.py` & `socketsecurity-0.0.60/socketsecurity/core/classes.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.59/socketsecurity/core/exceptions.py` & `socketsecurity-0.0.60/socketsecurity/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.59/socketsecurity/core/github.py` & `socketsecurity-0.0.60/socketsecurity/core/github.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.59/socketsecurity/core/glitlab.py` & `socketsecurity-0.0.60/socketsecurity/core/glitlab.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.59/socketsecurity/core/issues.py` & `socketsecurity-0.0.60/socketsecurity/core/issues.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.59/socketsecurity/core/licenses.py` & `socketsecurity-0.0.60/socketsecurity/core/licenses.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.59/socketsecurity/core/messages.py` & `socketsecurity-0.0.60/socketsecurity/core/messages.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.59/socketsecurity/socketcli.py` & `socketsecurity-0.0.60/socketsecurity/socketcli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import argparse
 import json
 from socketsecurity.core import Core, __version__
 from socketsecurity.core.classes import FullScanParams, Diff, Package
 from socketsecurity.core.messages import Messages
 import os
 import sys
+import logging
 
+logging.basicConfig(level=logging.INFO)
+log = logging.getLogger("socketcli")
 
 parser = argparse.ArgumentParser(
     prog="socketcli",
     description="Socket Security CLI"
 )
 parser.add_argument(
     '--api_token',
@@ -76,27 +79,36 @@
     '-v',
     '--version',
     action="version",
     version=f'%(prog)s {__version__}',
     help='Display the version',
 )
 
+parser.add_argument(
+    '--enable-debug',
+    help='Enable debug mode',
+    action='store_true',
+    default=False
+)
 
 def output_console_comments(diff_report) -> None:
     console_security_comment = Messages.create_console_security_alert_table(diff_report)
     if len(diff_report.new_alerts) > 0:
-        print("Security issues detected by Socket Security")
-        print(console_security_comment)
+        log.info("Security issues detected by Socket Security")
+        log.info(console_security_comment)
         sys.exit(1)
     else:
-        print("No New Security issues detected by Socket Security")
+        log.info("No New Security issues detected by Socket Security")
 
 
 def cli():
     arguments = parser.parse_args()
+    debug = arguments.enable_debug
+    if debug:
+        logging.basicConfig(level=logging.DEBUG)
     repo = arguments.repo
     branch = arguments.branch
     commit_message = arguments.commit_message
     committer = arguments.committer
     default_branch_int = arguments.default_branch
     default_branch = False
     if default_branch_int == 1:
@@ -107,20 +119,20 @@
     license_mode = arguments.generate_license
     license_file = f"{repo}"
     if branch is not None:
         license_file += f"_{branch}"
     license_file += ".json"
     api_token = os.getenv("SOCKET_SECURITY_API_KEY") or arguments.api_token
     if api_token is None:
-        print("Unable to find Socket API Token")
+        log.info("Unable to find Socket API Token")
         sys.exit(3)
     if repo is None:
-        print("Repo name needs to be set")
+        log.info("Repo name needs to be set")
         sys.exit(2)
-    print(f"Starting Socket Security Scan version {__version__}")
+    log.info(f"Starting Socket Security Scan version {__version__}")
     scm = None
     if scm_type == "github":
         from socketsecurity.core.github import Github
         scm = Github()
     elif scm_type == 'gitlab':
         from socketsecurity.core.glitlab import Gitlab
         scm = Gitlab()
@@ -139,30 +151,30 @@
         pull_request=pr_number,
         committers=committer,
         make_default_branch=default_branch,
         set_as_pending_head=set_as_pending_head
     )
     diff = None
     if scm is not None and scm.check_event_type() == "comment":
-        print("Comment initiated flow")
+        log.info("Comment initiated flow")
         comments = scm.get_comments_for_pr(scm.repository, str(scm.pr_number))
         scm.remove_comment_alerts(comments)
     elif scm is not None and scm.check_event_type() != "comment":
-        print("Push initiated flow")
+        log.info("Push initiated flow")
         diff: Diff
         diff = core.create_new_diff(target_path, params, workspace=target_path)
         if scm.check_event_type() == "diff":
             comments = scm.get_comments_for_pr(repo, str(pr_number))
             diff.new_alerts = scm.remove_alerts(comments, diff.new_alerts)
             overview_comment = Messages.dependency_overview_template(diff)
             security_comment = Messages.security_comment_template(diff)
             scm.add_socket_comments(security_comment, overview_comment, comments)
         output_console_comments(diff)
     else:
-        print("API Mode")
+        log.info("API Mode")
         diff: Diff
         diff = core.create_new_diff(target_path, params, workspace=target_path)
         output_console_comments(diff)
     if diff is not None and license_mode:
         all_packages = {}
         for package_id in diff.packages:
             package: Package
```

### Comparing `socketsecurity-0.0.59/socketsecurity.egg-info/PKG-INFO` & `socketsecurity-0.0.60/socketsecurity.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketsecurity
-Version: 0.0.59
+Version: 0.0.60
 Summary: Socket Security CLI for CI/CD
 Author-email: Douglas Coburn <douglas@socket.dev>
 Maintainer-email: Douglas Coburn <douglas@socket.dev>
 Project-URL: Homepage, https://socket.dev
 Keywords: socketsecurity,socket.dev,sca,oss,security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `socketsecurity-0.0.59/socketsecurity.egg-info/SOURCES.txt` & `socketsecurity-0.0.60/socketsecurity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

