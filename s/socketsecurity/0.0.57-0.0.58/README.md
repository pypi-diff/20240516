# Comparing `tmp/socketsecurity-0.0.57.tar.gz` & `tmp/socketsecurity-0.0.58.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socketsecurity-0.0.57.tar", last modified: Thu May 16 09:20:28 2024, max compression
+gzip compressed data, was "socketsecurity-0.0.58.tar", last modified: Thu May 16 09:30:19 2024, max compression
```

## Comparing `socketsecurity-0.0.57.tar` & `socketsecurity-0.0.58.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 09:20:28.587131 socketsecurity-0.0.57/
--rw-r--r--   0 douglascoburn   (501) staff       (20)      771 2024-05-16 09:20:28.586958 socketsecurity-0.0.57/PKG-INFO
--rw-r--r--   0 douglascoburn   (501) staff       (20)       21 2024-05-15 04:22:36.000000 socketsecurity-0.0.57/README.md
--rw-r--r--   0 douglascoburn   (501) staff       (20)     1025 2024-05-16 09:18:18.000000 socketsecurity-0.0.57/pyproject.toml
--rw-r--r--   0 douglascoburn   (501) staff       (20)       38 2024-05-16 09:20:28.587184 socketsecurity-0.0.57/setup.cfg
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 09:20:28.571095 socketsecurity-0.0.57/socketsecurity/
--rw-r--r--   0 douglascoburn   (501) staff       (20)       49 2024-05-16 09:18:28.000000 socketsecurity-0.0.57/socketsecurity/__init__.py
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 09:20:28.581506 socketsecurity-0.0.57/socketsecurity/core/
--rw-r--r--   0 douglascoburn   (501) staff       (20)    26034 2024-05-16 09:18:22.000000 socketsecurity-0.0.57/socketsecurity/core/__init__.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)     9282 2024-05-16 08:29:16.000000 socketsecurity-0.0.57/socketsecurity/core/classes.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)      626 2024-04-29 13:52:20.000000 socketsecurity-0.0.57/socketsecurity/core/exceptions.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)    11342 2024-05-16 07:53:25.000000 socketsecurity-0.0.57/socketsecurity/core/github.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)    10906 2024-05-16 08:32:33.000000 socketsecurity-0.0.57/socketsecurity/core/glitlab.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)    67547 2024-05-05 17:36:53.000000 socketsecurity-0.0.57/socketsecurity/core/issues.py
--rw-r--r--   0 douglascoburn   (501) staff       (20) 17442610 2024-05-06 19:45:31.000000 socketsecurity-0.0.57/socketsecurity/core/licenses.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)    11849 2024-05-15 05:15:37.000000 socketsecurity-0.0.57/socketsecurity/core/messages.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)     5787 2024-05-16 09:18:13.000000 socketsecurity-0.0.57/socketsecurity/socketcli.py
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 09:20:28.586772 socketsecurity-0.0.57/socketsecurity.egg-info/
--rw-r--r--   0 douglascoburn   (501) staff       (20)      771 2024-05-16 09:20:28.000000 socketsecurity-0.0.57/socketsecurity.egg-info/PKG-INFO
--rw-r--r--   0 douglascoburn   (501) staff       (20)      561 2024-05-16 09:20:28.000000 socketsecurity-0.0.57/socketsecurity.egg-info/SOURCES.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)        1 2024-05-16 09:20:28.000000 socketsecurity-0.0.57/socketsecurity.egg-info/dependency_links.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)       59 2024-05-16 09:20:28.000000 socketsecurity-0.0.57/socketsecurity.egg-info/entry_points.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)       38 2024-05-16 09:20:28.000000 socketsecurity-0.0.57/socketsecurity.egg-info/requires.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)       15 2024-05-16 09:20:28.000000 socketsecurity-0.0.57/socketsecurity.egg-info/top_level.txt
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 09:30:19.266027 socketsecurity-0.0.58/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      771 2024-05-16 09:30:19.265853 socketsecurity-0.0.58/PKG-INFO
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       21 2024-05-15 04:22:36.000000 socketsecurity-0.0.58/README.md
+-rw-r--r--   0 douglascoburn   (501) staff       (20)     1025 2024-05-16 09:30:10.000000 socketsecurity-0.0.58/pyproject.toml
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       38 2024-05-16 09:30:19.266067 socketsecurity-0.0.58/setup.cfg
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 09:30:19.250979 socketsecurity-0.0.58/socketsecurity/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       49 2024-05-16 09:30:07.000000 socketsecurity-0.0.58/socketsecurity/__init__.py
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 09:30:19.260981 socketsecurity-0.0.58/socketsecurity/core/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    26034 2024-05-16 09:30:05.000000 socketsecurity-0.0.58/socketsecurity/core/__init__.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)     9282 2024-05-16 08:29:16.000000 socketsecurity-0.0.58/socketsecurity/core/classes.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      626 2024-04-29 13:52:20.000000 socketsecurity-0.0.58/socketsecurity/core/exceptions.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    11342 2024-05-16 07:53:25.000000 socketsecurity-0.0.58/socketsecurity/core/github.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    10963 2024-05-16 09:28:06.000000 socketsecurity-0.0.58/socketsecurity/core/glitlab.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    67547 2024-05-05 17:36:53.000000 socketsecurity-0.0.58/socketsecurity/core/issues.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20) 17442610 2024-05-06 19:45:31.000000 socketsecurity-0.0.58/socketsecurity/core/licenses.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    11849 2024-05-15 05:15:37.000000 socketsecurity-0.0.58/socketsecurity/core/messages.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)     5641 2024-05-16 09:29:23.000000 socketsecurity-0.0.58/socketsecurity/socketcli.py
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 09:30:19.263893 socketsecurity-0.0.58/socketsecurity.egg-info/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      771 2024-05-16 09:30:19.000000 socketsecurity-0.0.58/socketsecurity.egg-info/PKG-INFO
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      561 2024-05-16 09:30:19.000000 socketsecurity-0.0.58/socketsecurity.egg-info/SOURCES.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)        1 2024-05-16 09:30:19.000000 socketsecurity-0.0.58/socketsecurity.egg-info/dependency_links.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       59 2024-05-16 09:30:19.000000 socketsecurity-0.0.58/socketsecurity.egg-info/entry_points.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       38 2024-05-16 09:30:19.000000 socketsecurity-0.0.58/socketsecurity.egg-info/requires.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       15 2024-05-16 09:30:19.000000 socketsecurity-0.0.58/socketsecurity.egg-info/top_level.txt
```

### Comparing `socketsecurity-0.0.57/PKG-INFO` & `socketsecurity-0.0.58/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketsecurity
-Version: 0.0.57
+Version: 0.0.58
 Summary: Socket Security CLI for CI/CD
 Author-email: Douglas Coburn <douglas@socket.dev>
 Maintainer-email: Douglas Coburn <douglas@socket.dev>
 Project-URL: Homepage, https://socket.dev
 Keywords: socketsecurity,socket.dev,sca,oss,security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `socketsecurity-0.0.57/pyproject.toml` & `socketsecurity-0.0.58/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "socketsecurity"
-version = "0.0.57"
+version = "0.0.58"
 requires-python = ">= 3.9"
 dependencies = [
     'requests',
     'mdutils',
     'prettytable',
     'argparse'
 ]
```

### Comparing `socketsecurity-0.0.57/socketsecurity/core/__init__.py` & `socketsecurity-0.0.58/socketsecurity/core/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 )
 import platform
 from glob import glob
 import time
 
 
 __author__ = 'socket.dev'
-__version__ = '0.0.57'
+__version__ = '0.0.58'
 __all__ = [
     "Core",
     "log",
     "__version__"
 ]
```

### Comparing `socketsecurity-0.0.57/socketsecurity/core/classes.py` & `socketsecurity-0.0.58/socketsecurity/core/classes.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.57/socketsecurity/core/exceptions.py` & `socketsecurity-0.0.58/socketsecurity/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.57/socketsecurity/core/github.py` & `socketsecurity-0.0.58/socketsecurity/core/github.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.57/socketsecurity/core/glitlab.py` & `socketsecurity-0.0.58/socketsecurity/core/glitlab.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from socketsecurity.core.classes import GitlabComment, Diff, Issue
 import sys
 
 
 global ci_commit_sha
 global ci_api_v4_url
 global ci_project_dir
-global ci_commit_branch
+global ci_merge_request_source_branch_name
 global ci_merge_request_iid
 global ci_merge_request_project_id
 global ci_commit_message
 global ci_default_branch
 global ci_project_name
 global ci_pipeline_source
 global ci_commit_author
@@ -26,15 +26,15 @@
 
 
 
 gitlab_variables = [
     "CI_COMMIT_SHA",
     "CI_API_V4_URL",
     "CI_PROJECT_DIR",
-    "CI_COMMIT_BRANCH",
+    "CI_MERGE_REQUEST_SOURCE_BRANCH_NAME",
     "CI_MERGE_REQUEST_IID",
     "CI_MERGE_REQUEST_PROJECT_ID",
     "CI_COMMIT_MESSAGE",
     "CI_DEFAULT_BRANCH",
     "CI_PROJECT_NAME",
     "CI_PIPELINE_SOURCE",
     "CI_COMMIT_AUTHOR",
@@ -124,15 +124,15 @@
         self.api_url = ci_api_v4_url
         self.ref_type = ""
         self.event_name = ci_pipeline_source
         self.workspace = project_dir
         self.repository = ci_project_name
         if "/" in self.repository:
             self.repository = self.repository.rsplit("/")[1]
-        self.branch = ci_commit_branch
+        self.branch = ci_merge_request_source_branch_name
         self.default_branch = ci_default_branch
         if self.branch == self.default_branch:
             self.is_default_branch = True
         else:
             self.is_default_branch = False
         self.pr_number = ci_merge_request_iid
         self.pr_name = pr_name
```

### Comparing `socketsecurity-0.0.57/socketsecurity/core/issues.py` & `socketsecurity-0.0.58/socketsecurity/core/issues.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.57/socketsecurity/core/licenses.py` & `socketsecurity-0.0.58/socketsecurity/core/licenses.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.57/socketsecurity/core/messages.py` & `socketsecurity-0.0.58/socketsecurity/core/messages.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.57/socketsecurity/socketcli.py` & `socketsecurity-0.0.58/socketsecurity/socketcli.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,21 +52,15 @@
 )
 parser.add_argument(
     '--target_path',
     default='./',
     help='Path to look for manifest files',
     required=False
 )
-parser.add_argument(
-    '--mode',
-    default='diff',
-    help='Integration mode choices are api, github, gitlab, and bitbucket',
-    choices=["diff", "new", "license"],
-    required=False
-)
+
 parser.add_argument(
     '--scm',
     default='api',
     help='Integration mode choices are api, github, gitlab, and bitbucket',
     choices=["api", "github", "gitlab"],
     required=False
 )
@@ -103,15 +97,14 @@
     branch = arguments.branch
     commit_message = arguments.commit_message
     committer = arguments.committer
     default_branch_int = arguments.default_branch
     default_branch = False
     if default_branch_int == 1:
         default_branch = True
-    mode = arguments.mode
     pr_number = arguments.pr_number
     target_path = arguments.target_path
     scm_type = arguments.scm
     license_mode = arguments.generate_license
     license_file = f"{repo}"
     if branch is not None:
         license_file += f"_{branch}"
@@ -127,14 +120,16 @@
     scm = None
     if scm_type == "github":
         from socketsecurity.core.github import Github
         scm = Github()
     elif scm_type == 'gitlab':
         from socketsecurity.core.glitlab import Gitlab
         scm = Gitlab()
+    if scm is not None:
+        default_branch = scm.is_default_branch
     base_api_url = os.getenv("BASE_API_URL") or None
     core = Core(token=api_token, request_timeout=6000, base_api_url=base_api_url)
     set_as_pending_head = False
     if default_branch:
         set_as_pending_head = True
     params = FullScanParams(
         repo=repo,
```

### Comparing `socketsecurity-0.0.57/socketsecurity.egg-info/PKG-INFO` & `socketsecurity-0.0.58/socketsecurity.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketsecurity
-Version: 0.0.57
+Version: 0.0.58
 Summary: Socket Security CLI for CI/CD
 Author-email: Douglas Coburn <douglas@socket.dev>
 Maintainer-email: Douglas Coburn <douglas@socket.dev>
 Project-URL: Homepage, https://socket.dev
 Keywords: socketsecurity,socket.dev,sca,oss,security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `socketsecurity-0.0.57/socketsecurity.egg-info/SOURCES.txt` & `socketsecurity-0.0.58/socketsecurity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

