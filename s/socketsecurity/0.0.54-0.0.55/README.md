# Comparing `tmp/socketsecurity-0.0.54-py3-none-any.whl.zip` & `tmp/socketsecurity-0.0.55-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 2704464 bytes, number of entries: 15
--rw-r--r--  2.0 unx       49 b- defN 24-May-15 05:16 socketsecurity/__init__.py
--rw-r--r--  2.0 unx     5517 b- defN 24-May-15 05:15 socketsecurity/socketcli.py
--rw-r--r--  2.0 unx    26005 b- defN 24-May-15 05:16 socketsecurity/core/__init__.py
--rw-r--r--  2.0 unx     8606 b- defN 24-May-13 22:21 socketsecurity/core/classes.py
+Zip file size: 2704511 bytes, number of entries: 15
+-rw-r--r--  2.0 unx       49 b- defN 24-May-16 08:35 socketsecurity/__init__.py
+-rw-r--r--  2.0 unx     5636 b- defN 24-May-16 08:49 socketsecurity/socketcli.py
+-rw-r--r--  2.0 unx    26015 b- defN 24-May-16 08:35 socketsecurity/core/__init__.py
+-rw-r--r--  2.0 unx     9282 b- defN 24-May-16 08:29 socketsecurity/core/classes.py
 -rw-r--r--  2.0 unx      626 b- defN 24-Apr-29 13:52 socketsecurity/core/exceptions.py
--rw-r--r--  2.0 unx    11296 b- defN 24-May-15 05:15 socketsecurity/core/github.py
--rw-r--r--  2.0 unx    11253 b- defN 24-May-15 05:15 socketsecurity/core/glitlab.py
+-rw-r--r--  2.0 unx    11342 b- defN 24-May-16 07:53 socketsecurity/core/github.py
+-rw-r--r--  2.0 unx    10906 b- defN 24-May-16 08:32 socketsecurity/core/glitlab.py
 -rw-r--r--  2.0 unx    67547 b- defN 24-May-05 17:36 socketsecurity/core/issues.py
 -rw-r--r--  2.0 unx 17442610 b- defN 24-May-06 19:45 socketsecurity/core/licenses.py
 -rw-r--r--  2.0 unx    11849 b- defN 24-May-15 05:15 socketsecurity/core/messages.py
--rw-r--r--  2.0 unx      771 b- defN 24-May-15 05:17 socketsecurity-0.0.54.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-15 05:17 socketsecurity-0.0.54.dist-info/WHEEL
--rw-r--r--  2.0 unx       59 b- defN 24-May-15 05:17 socketsecurity-0.0.54.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       15 b- defN 24-May-15 05:17 socketsecurity-0.0.54.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1305 b- defN 24-May-15 05:17 socketsecurity-0.0.54.dist-info/RECORD
-15 files, 17587600 bytes uncompressed, 2702292 bytes compressed:  84.6%
+-rw-r--r--  2.0 unx      771 b- defN 24-May-16 08:54 socketsecurity-0.0.55.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-16 08:54 socketsecurity-0.0.55.dist-info/WHEEL
+-rw-r--r--  2.0 unx       59 b- defN 24-May-16 08:54 socketsecurity-0.0.55.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       15 b- defN 24-May-16 08:54 socketsecurity-0.0.55.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1305 b- defN 24-May-16 08:54 socketsecurity-0.0.55.dist-info/RECORD
+15 files, 17588104 bytes uncompressed, 2702339 bytes compressed:  84.6%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: socketsecurity/core/licenses.py
 Comment: 
 
 Filename: socketsecurity/core/messages.py
 Comment: 
 
-Filename: socketsecurity-0.0.54.dist-info/METADATA
+Filename: socketsecurity-0.0.55.dist-info/METADATA
 Comment: 
 
-Filename: socketsecurity-0.0.54.dist-info/WHEEL
+Filename: socketsecurity-0.0.55.dist-info/WHEEL
 Comment: 
 
-Filename: socketsecurity-0.0.54.dist-info/entry_points.txt
+Filename: socketsecurity-0.0.55.dist-info/entry_points.txt
 Comment: 
 
-Filename: socketsecurity-0.0.54.dist-info/top_level.txt
+Filename: socketsecurity-0.0.55.dist-info/top_level.txt
 Comment: 
 
-Filename: socketsecurity-0.0.54.dist-info/RECORD
+Filename: socketsecurity-0.0.55.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## socketsecurity/__init__.py

```diff
@@ -1,2 +1,2 @@
 __author__ = 'socket.dev'
-__version__ = '0.0.54'
+__version__ = '0.0.55'
```

## socketsecurity/socketcli.py

```diff
@@ -64,15 +64,15 @@
     choices=["diff", "new", "license"],
     required=False
 )
 parser.add_argument(
     '--scm',
     default='api',
     help='Integration mode choices are api, github, gitlab, and bitbucket',
-    choices=["api", "github"],
+    choices=["api", "github", "gitlab"],
     required=False
 )
 
 parser.add_argument(
     '--generate-license',
     default=False,
     help='Run in license mode to generate license output',
@@ -117,14 +117,17 @@
         print("Repo name needs to be set")
         sys.exit(2)
     print(f"Starting Socket Security Scan version {version}")
     scm = None
     if scm_type == "github":
         from socketsecurity.core.github import Github
         scm = Github()
+    elif scm_type == 'gitlab':
+        from socketsecurity.core.glitlab import Gitlab
+        scm = Gitlab()
     base_api_url = os.getenv("BASE_API_URL") or None
     core = Core(token=api_token, request_timeout=6000, base_api_url=base_api_url)
     set_as_pending_head = False
     if default_branch:
         set_as_pending_head = True
     params = FullScanParams(
         repo=repo,
```

## socketsecurity/core/__init__.py

```diff
@@ -19,15 +19,15 @@
 )
 import platform
 from glob import glob
 import time
 
 
 __author__ = 'socket.dev'
-__version__ = '0.0.54'
+__version__ = '0.0.55'
 __all__ = [
     "Core",
     "log"
 ]
 
 
 global encoded_key
@@ -425,24 +425,24 @@
             if head_full_scan_id is None or head_full_scan_id == "":
                 head_full_scan = []
             else:
                 head_start = time.time()
                 head_full_scan = Core.get_sbom_data(head_full_scan_id)
                 head_end = time.time()
                 total_head_time = head_end - head_start
-                print(f"Total time to get head sbom {total_head_time: .2f}")
+                print(f"Total time to get head full-scan {total_head_time: .2f}")
         except APIResourceNotFound:
             head_full_scan = []
         if files is not None and len(files) > 0:
             new_scan_start = time.time()
             new_full_scan = Core.create_full_scan(files, params, workspace)
             new_full_scan.packages = Core.create_sbom_dict(new_full_scan.sbom_artifacts)
             new_scan_end = time.time()
             total_new_time = new_scan_end - new_scan_start
-            print(f"Total time to get new sbom {total_new_time: .2f}")
+            print(f"Total time to get new full-scan {total_new_time: .2f}")
             diff_report = Core.compare_sboms(new_full_scan.sbom_artifacts, head_full_scan)
             diff_report.packages = new_full_scan.packages
         else:
             diff_report = Diff()
         return diff_report
 
     @staticmethod
```

## socketsecurity/core/classes.py

```diff
@@ -363,7 +363,39 @@
                 setattr(self, key, value)
         if not hasattr(self, "body_list"):
             self.body_list = []
 
     def __str__(self):
         return json.dumps(self.__dict__)
 
+
+class GitlabComment:
+    id: int
+    type: str
+    body: str
+    attachment: str
+    author: dict
+    created_at: str
+    updated_at: str
+    system: bool
+    notable_id: int
+    noteable_type: str
+    project_id: int
+    resolvable: bool
+    confidential: bool
+    internal: bool
+    imported: bool
+    imported_from: str
+    noteable_iid: int
+    commands_changes: dict
+    body_list: list
+
+    def __init__(self, **kwargs):
+        if kwargs:
+            for key, value in kwargs.items():
+                setattr(self, key, value)
+        if not hasattr(self, "body_list"):
+            self.body_list = []
+
+    def __str__(self):
+        return json.dumps(self.__dict__)
+
```

## socketsecurity/core/github.py

```diff
@@ -118,33 +118,35 @@
     is_default_branch: bool
     pr_number: int
     pr_name: str
     commit_message: str
     committer: str
     github_env: str
     api_token: str
+    project_id: int
 
     def __init__(self):
         self.commit_sha = github_sha
         self.api_url = github_api_url
         self.ref_type = github_ref_type
         self.event_name = github_event_name
         self.workspace = github_workspace
         self.repository = github_repository
         if "/" in self.repository:
             self.repository = self.repository.rsplit("/")[1]
-        self.ref_name = github_ref_name
+        self.branch = github_ref_name
         self.default_branch = default_branch
         self.is_default_branch = is_default_branch
         self.pr_number = pr_number
         self.pr_name = pr_name
         self.commit_message = commit_message
         self.committer = github_actor
         self.github_env = github_env
         self.api_token = gh_api_token
+        self.project_id = 0
         if self.api_token is None:
             print("Unable to get Github API Token from GH_API_TOKEN")
             sys.exit(2)
 
     @staticmethod
     def check_event_type() -> str:
         if github_event_name.lower() == "push":
```

## socketsecurity/core/glitlab.py

```diff
@@ -1,62 +1,57 @@
 import json
 import os
 from socketsecurity.core import log
 import requests
 from socketsecurity.core.exceptions import *
-from socketsecurity.core.classes import GithubComment, Diff, Issue
+from socketsecurity.core.classes import GitlabComment, Diff, Issue
+import sys
 
 
-global github_sha
-global github_api_url
-global github_ref_type
-global github_event_name
-global github_workspace
-global github_repository
-global github_ref_name
-global github_actor
-global default_branch
-global github_env
-global pr_number
+global ci_commit_sha
+global ci_api_v4_url
+global ci_project_dir
+global ci_commit_branch
+global ci_merge_request_iid
+global ci_merge_request_project_id
+global ci_commit_message
+global ci_default_branch
+global ci_project_name
+global ci_pipeline_source
+global ci_commit_author
+global project_dir
 global pr_name
 global is_default_branch
-global commit_message
 global committer
-global gh_api_token
-global github_repository_owner
+global gitlab_token
 
 
-github_variables = [
+
+gitlab_variables = [
     "CI_COMMIT_SHA",
-    "GITHUB_API_URL",
-    "GITHUB_REF_TYPE",
-    "GITHUB_EVENT_NAME",
-    "GITHUB_WORKSPACE",
-    "GITHUB_REPOSITORY",
+    "CI_API_V4_URL",
+    "CI_PROJECT_DIR",
     "CI_COMMIT_BRANCH",
+    "CI_MERGE_REQUEST_IID",
+    "CI_MERGE_REQUEST_PROJECT_ID",
+    "CI_COMMIT_MESSAGE",
+    "CI_DEFAULT_BRANCH",
+    "CI_PROJECT_NAME",
+    "CI_PIPELINE_SOURCE",
+    "CI_COMMIT_AUTHOR",
+    "PROJECT_DIR",
     "DEFAULT_BRANCH",
-    "PR_NUMBER",
     "PR_NAME",
-    "COMMIT_MESSAGE",
-    "GITHUB_ACTOR",
-    "GITHUB_ENV",
-    "GH_API_TOKEN",
-    "GITHUB_REPOSITORY_OWNER"
+    "GITLAB_TOKEN",
 ]
 
 
-for env in github_variables:
+for env in gitlab_variables:
     var_name = env.lower()
     globals()[var_name] = os.getenv(env) or None
-    if var_name == "default_branch":
-        global is_default_branch
-        if default_branch is None or default_branch.lower() == "false":
-            is_default_branch = False
-        else:
-            is_default_branch = True
 
 
 def do_request(
         path: str,
         headers: dict = None,
         payload: [dict, str] = None,
         files: list = None,
@@ -68,24 +63,24 @@
     :param path: Required path for the request
     :param headers: Optional dictionary of headers. If not set will use a default set
     :param payload: Optional dictionary or string of the payload to pass
     :param files: Optional list of files to upload
     :param method: Optional method to use, defaults to GET
     :return:
     """
-    if gh_api_token is None or gh_api_token == "":
+    if gitlab_token is None or gitlab_token == "":
         raise APIKeyMissing
 
     if headers is None:
         headers = {
-            'Authorization': f"Bearer {gh_api_token}",
+            'Authorization': f"Bearer {gitlab_token}",
             'User-Agent': 'SocketPythonScript/0.0.1',
             "accept": "application/json"
         }
-    url = f"{github_api_url}/{path}"
+    url = f"{ci_api_v4_url}/{path}"
     response = requests.request(
         method.upper(),
         url,
         headers=headers,
         data=payload,
         files=files
     )
@@ -110,124 +105,118 @@
 class Gitlab:
     commit_sha: str
     api_url: str
     ref_type: str
     event_name: str
     workspace: str
     repository: str
-    ref_name: str
+    branch: str
     default_branch: str
     is_default_branch: bool
     pr_number: int
     pr_name: str
     commit_message: str
     committer: str
-    github_env: str
     api_token: str
+    project_id: int
 
     def __init__(self):
-        self.commit_sha = github_sha
-        self.api_url = github_api_url
-        self.ref_type = github_ref_type
-        self.event_name = github_event_name
-        self.workspace = github_workspace
-        self.repository = github_repository
+        self.commit_sha = ci_commit_sha
+        self.api_url = ci_api_v4_url
+        self.ref_type = ""
+        self.event_name = ci_pipeline_source
+        self.workspace = project_dir
+        self.repository = ci_project_name
         if "/" in self.repository:
             self.repository = self.repository.rsplit("/")[1]
-        self.ref_name = github_ref_name
-        self.default_branch = default_branch
-        self.is_default_branch = is_default_branch
-        self.pr_number = pr_number
+        self.branch = ci_commit_branch
+        self.default_branch = ci_default_branch
+        if self.branch == self.default_branch:
+            self.is_default_branch = True
+        else:
+            self.is_default_branch = False
+        self.pr_number = ci_merge_request_iid
         self.pr_name = pr_name
-        self.commit_message = commit_message
-        self.committer = github_actor
-        self.github_env = github_env
-        self.api_token = gh_api_token
+        self.commit_message = ci_commit_message
+        self.committer = ci_commit_author
+        self.api_token = gitlab_token
+        self.project_id = ci_merge_request_project_id
         if self.api_token is None:
-            print("Unable to get Github API Token from GH_API_TOKEN")
+            print("Unable to get gitlab API Token from GH_API_TOKEN")
             sys.exit(2)
 
     @staticmethod
     def check_event_type() -> str:
-        if github_event_name.lower() == "push":
-            if pr_number is None or pr_number == "":
+        if ci_pipeline_source.lower() == "push":
+            if ci_merge_request_iid is None or ci_merge_request_iid == "":
                 event_type = "main"
             else:
                 event_type = "diff"
-        elif github_event_name.lower() == "issue_comment":
+        elif ci_pipeline_source.lower() == "issue_comment":
             event_type = "comment"
         else:
-            log.error(f"Unknown event type {github_event_name}")
+            log.error(f"Unknown event type {ci_pipeline_source}")
             sys.exit(1)
         return event_type
 
     @staticmethod
     def add_socket_comments(security_comment: str, overview_comment: str, comments: dict) -> None:
         existing_overview_comment = comments.get("overview")
         existing_security_comment = comments.get("security")
         if existing_overview_comment is not None:
-            existing_overview_comment: GithubComment
-            Github.update_comment(overview_comment, str(existing_overview_comment.id))
+            existing_overview_comment: GitlabComment
+            Gitlab.update_comment(overview_comment, str(existing_overview_comment.id))
         else:
-            Github.post_comment(overview_comment)
+            Gitlab.post_comment(overview_comment)
         if existing_security_comment is not None:
-            existing_security_comment: GithubComment
-            Github.update_comment(security_comment, str(existing_security_comment.id))
+            existing_security_comment: GitlabComment
+            Gitlab.update_comment(security_comment, str(existing_security_comment.id))
         else:
-            Github.post_comment(security_comment)
+            Gitlab.post_comment(security_comment)
 
     @staticmethod
     def post_comment(body: str) -> None:
-        repo = github_repository.rsplit("/", 1)[1]
-        path = f"repos/{github_repository_owner}/{repo}/issues/{pr_number}/comments"
+        path = f"projects/{ci_merge_request_project_id}/merge_requests/{ci_merge_request_iid}/notes"
         payload = {
             "body": body
         }
         payload = json.dumps(payload)
         do_request(path, payload=payload, method="POST")
 
     @staticmethod
     def update_comment(body: str, comment_id: str) -> None:
-        repo = github_repository.rsplit("/", 1)[1]
-        path = f"repos/{github_repository_owner}/{repo}/issues/comments/{comment_id}"
+        path = f"projects/{ci_merge_request_project_id}/merge_requests/{ci_merge_request_iid}/notes/{comment_id}"
         payload = {
             "body": body
         }
         payload = json.dumps(payload)
         do_request(path, payload=payload, method="PATCH")
 
     @staticmethod
-    def write_new_env(name: str, content: str) -> None:
-        file = open(github_env, "a")
-        new_content = content.replace("\n", "\\n")
-        env_output = f"{name}={new_content}"
-        file.write(env_output)
-
-    @staticmethod
-    def get_comments_for_pr(repo: str, pr: str) -> dict:
-        path = f"repos/{github_repository_owner}/{repo}/issues/{pr}/comments"
+    def get_comments_for_pr() -> dict:
+        path = f"projects/{ci_merge_request_project_id}/merge_requests/{ci_merge_request_iid}/notes"
         raw_comments = do_request(path)
         comments = {}
-        if "error" not in raw_comments:
+        if "message" not in raw_comments:
             for item in raw_comments:
-                comment = GithubComment(**item)
+                comment = GitlabComment(**item)
                 comments[comment.id] = comment
                 for line in comment.body.split("\n"):
                     comment.body_list.append(line)
         else:
             log.error(raw_comments)
-        socket_comments = Github.check_for_socket_comments(comments)
+        socket_comments = Gitlab.check_for_socket_comments(comments)
         return socket_comments
 
     @staticmethod
     def check_for_socket_comments(comments: dict):
         socket_comments = {}
         for comment_id in comments:
             comment = comments[comment_id]
-            comment: GithubComment
+            comment: GitlabComment
             if "socket-security-comment-actions" in comment.body:
                 socket_comments["security"] = comment
             elif "socket-overview-comment-actions" in comment.body:
                 socket_comments["overview"] = comment
             elif "SocketSecurity ignore" in comment.body:
                 if "ignore" not in socket_comments:
                     socket_comments["ignore"] = []
@@ -235,15 +224,15 @@
         return socket_comments
 
     @staticmethod
     def remove_alerts(comments: dict, new_alerts: list) -> list:
         alerts = []
         if "ignore" not in comments:
             return new_alerts
-        ignore_all, ignore_commands = Github.get_ignore_options(comments)
+        ignore_all, ignore_commands = Gitlab.get_ignore_options(comments)
         for alert in new_alerts:
             alert: Issue
             if ignore_all:
                 break
             else:
                 purl = f"{alert.pkg_name}, {alert.pkg_version}"
                 purl_star = f"{alert.pkg_name}, *"
@@ -256,15 +245,15 @@
 
     @staticmethod
     def get_ignore_options(comments: dict) -> [bool, list]:
         ignore_commands = []
         ignore_all = False
 
         for comment in comments["ignore"]:
-            comment: GithubComment
+            comment: GitlabComment
             first_line = comment.body_list[0]
             if not ignore_all and "SocketSecurity ignore" in first_line:
                 first_line = first_line.lstrip("@")
                 _, command = first_line.split("SocketSecurity ")
                 command = command.strip()
                 if command == "ignore-all":
                     ignore_all = True
@@ -282,42 +271,42 @@
             result = True
         return result
 
     @staticmethod
     def remove_comment_alerts(comments: dict):
         security_alert = comments.get("security")
         if security_alert is not None:
-            security_alert: GithubComment
-            new_body = Github.process_security_comment(security_alert, comments)
-            Github.update_comment(new_body, str(security_alert.id))
+            security_alert: GitlabComment
+            new_body = Gitlab.process_security_comment(security_alert, comments)
+            Gitlab.update_comment(new_body, str(security_alert.id))
 
     @staticmethod
     def is_heading_line(line) -> bool:
         is_heading_line = True
         if line != "|Alert|Package|Introduced by|Manifest File|" and ":---" not in line:
             is_heading_line = False
         return is_heading_line
 
     @staticmethod
-    def process_security_comment(comment: GithubComment, comments) -> str:
+    def process_security_comment(comment: GitlabComment, comments) -> str:
         lines = []
         start = False
-        ignore_all, ignore_commands = Github.get_ignore_options(comments)
+        ignore_all, ignore_commands = Gitlab.get_ignore_options(comments)
         for line in comment.body_list:
             line = line.strip()
             if "start-socket-alerts-table" in line:
                 start = True
-            elif start and "end-socket-alerts-table" not in line and not Github.is_heading_line(line) and line != '':
+            elif start and "end-socket-alerts-table" not in line and not Gitlab.is_heading_line(line) and line != '':
                 title, package, introduced_by, manifest = line.lstrip("|").rstrip("|").split("|")
                 details, _ = package.split("](")
                 ecosystem, details = details.split("/", 1)
                 pkg_name, pkg_version = details.split("@")
                 ignore = False
                 for name, version in ignore_commands:
-                    if ignore_all or Github.is_ignore(pkg_name, pkg_version, name, version):
+                    if ignore_all or Gitlab.is_ignore(pkg_name, pkg_version, name, version):
                         ignore = True
                 if not ignore:
                     lines.append(line)
             elif "end-socket-alerts-table" in line:
                 start = False
                 lines.append(line)
             else:
```

## Comparing `socketsecurity-0.0.54.dist-info/METADATA` & `socketsecurity-0.0.55.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketsecurity
-Version: 0.0.54
+Version: 0.0.55
 Summary: Socket Security CLI for CI/CD
 Author-email: Douglas Coburn <douglas@socket.dev>
 Maintainer-email: Douglas Coburn <douglas@socket.dev>
 Project-URL: Homepage, https://socket.dev
 Keywords: socketsecurity,socket.dev,sca,oss,security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

## Comparing `socketsecurity-0.0.54.dist-info/RECORD` & `socketsecurity-0.0.55.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-socketsecurity/__init__.py,sha256=NrE5YsOkHORpE-QcSHtaX9GrU7klhGqlSu7771PFU9I,49
-socketsecurity/socketcli.py,sha256=-ZctqrFQ0BF4ztux2hbrTtNfd2Cr3nCUsGUbj-q2Q1k,5517
-socketsecurity/core/__init__.py,sha256=1RW1IUP5LK524v2DbwZLToP21Qapoo6LqA-kVnQotCw,26005
-socketsecurity/core/classes.py,sha256=VlIzLOhG9Z5K-95ovblrCR9wDgGBs0N3mFSa6d9qbw8,8606
+socketsecurity/__init__.py,sha256=ACrfRKvrxRVxwNeWp8Xoc7CWrNMdlZrlfgXjA9ou_yk,49
+socketsecurity/socketcli.py,sha256=d0IgXL9M4zupXHkrbSzdsXGp0Y3AFSWhq1NF7Ff2MXk,5636
+socketsecurity/core/__init__.py,sha256=G-i7TnYuh-lZmg_NIZYJEKYELC6L0kY05C6oHvz5iAw,26015
+socketsecurity/core/classes.py,sha256=PXmVuTOmuK1H8F5UxyostYS-caAWZWdz-4_yNwBnQUM,9282
 socketsecurity/core/exceptions.py,sha256=C7q0D3KlnE3ff4FyTnlY9TxU3G-7xaRZcxpanUPvCzc,626
-socketsecurity/core/github.py,sha256=Hs8aPRsO-5-K_0GCVdRrNCFjvg1sc2ipRwVLC9lPyp0,11296
-socketsecurity/core/glitlab.py,sha256=YMVvk52mrQuNbX2ls0_n4RfdPi2K_6oJUAtXN2IuI90,11253
+socketsecurity/core/github.py,sha256=lGhHIMO1V6ZW5Jajct-Bc5ig_0zhjd68-rnNnMqyq7k,11342
+socketsecurity/core/glitlab.py,sha256=SZvDf6pYS298u8DTeKggS1bymqMgy12v0V7JVenoems,10906
 socketsecurity/core/issues.py,sha256=_AsYSTV-Fu4_o0fmxRV7JMZGQKyyaeN8mIvv64szwQ8,67547
 socketsecurity/core/licenses.py,sha256=VIpK01sRmKy_94ulojgWJHS2K8xo9YnW5KoJYhn8aaI,17442610
 socketsecurity/core/messages.py,sha256=0fqZ9Tp4Ykhf4jY99CP8s8v6y9A1q8cMR46Nj-X3pBg,11849
-socketsecurity-0.0.54.dist-info/METADATA,sha256=HHlH6H7AdVb487gEP5unk2S1aqFgZAZIagdWjKi_adU,771
-socketsecurity-0.0.54.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-socketsecurity-0.0.54.dist-info/entry_points.txt,sha256=6RvItr40ejlapwQ9_dS5U5iuaBDvp8lIL2NZOn1xSPM,59
-socketsecurity-0.0.54.dist-info/top_level.txt,sha256=ukMzHpGy5wQ9XCd7OzP2Y2iBz3zd9mB7RtNzj5wf6c4,15
-socketsecurity-0.0.54.dist-info/RECORD,,
+socketsecurity-0.0.55.dist-info/METADATA,sha256=Da5hkQDLfEscmnHvE-VBLY_N38CPvFezZL3Fr4SvZkE,771
+socketsecurity-0.0.55.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+socketsecurity-0.0.55.dist-info/entry_points.txt,sha256=6RvItr40ejlapwQ9_dS5U5iuaBDvp8lIL2NZOn1xSPM,59
+socketsecurity-0.0.55.dist-info/top_level.txt,sha256=ukMzHpGy5wQ9XCd7OzP2Y2iBz3zd9mB7RtNzj5wf6c4,15
+socketsecurity-0.0.55.dist-info/RECORD,,
```

