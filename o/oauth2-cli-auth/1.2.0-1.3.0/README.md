# Comparing `tmp/oauth2_cli_auth-1.2.0.tar.gz` & `tmp/oauth2_cli_auth-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oauth2_cli_auth-1.2.0.tar", max compression
+gzip compressed data, was "oauth2_cli_auth-1.3.0.tar", max compression
```

## Comparing `oauth2_cli_auth-1.2.0.tar` & `oauth2_cli_auth-1.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1068 2023-12-10 13:00:12.300512 oauth2_cli_auth-1.2.0/LICENSE
--rw-r--r--   0        0        0     7510 2023-12-10 13:00:12.300512 oauth2_cli_auth-1.2.0/README.md
--rw-r--r--   0        0        0      338 2023-12-10 13:00:12.300512 oauth2_cli_auth-1.2.0/oauth2_cli_auth/__init__.py
--rw-r--r--   0        0        0      494 2023-12-10 13:00:12.300512 oauth2_cli_auth-1.2.0/oauth2_cli_auth/_timeout.py
--rw-r--r--   0        0        0      736 2023-12-10 13:00:12.300512 oauth2_cli_auth-1.2.0/oauth2_cli_auth/_urllib_util.py
--rw-r--r--   0        0        0     2998 2023-12-10 13:00:12.300512 oauth2_cli_auth-1.2.0/oauth2_cli_auth/code_grant.py
--rw-r--r--   0        0        0      221 2023-12-10 13:00:12.300512 oauth2_cli_auth-1.2.0/oauth2_cli_auth/conftest.py
--rw-r--r--   0        0        0     7512 2023-12-10 13:00:12.300512 oauth2_cli_auth-1.2.0/oauth2_cli_auth/http_server.py
--rw-r--r--   0        0        0      985 2023-12-10 13:00:12.300512 oauth2_cli_auth-1.2.0/oauth2_cli_auth/simplified_flow.py
--rw-r--r--   0        0        0     1249 2023-12-10 13:00:12.300512 oauth2_cli_auth-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     8554 1970-01-01 00:00:00.000000 oauth2_cli_auth-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-16 08:37:14.046018 oauth2_cli_auth-1.3.0/LICENSE
+-rw-r--r--   0        0        0     7510 2024-05-16 08:37:14.046018 oauth2_cli_auth-1.3.0/README.md
+-rw-r--r--   0        0        0      338 2024-05-16 08:37:14.046018 oauth2_cli_auth-1.3.0/oauth2_cli_auth/__init__.py
+-rw-r--r--   0        0        0      495 2024-05-16 08:37:14.046018 oauth2_cli_auth-1.3.0/oauth2_cli_auth/_timeout.py
+-rw-r--r--   0        0        0      769 2024-05-16 08:37:14.046018 oauth2_cli_auth-1.3.0/oauth2_cli_auth/_urllib_util.py
+-rw-r--r--   0        0        0     4080 2024-05-16 08:37:14.046018 oauth2_cli_auth-1.3.0/oauth2_cli_auth/code_grant.py
+-rw-r--r--   0        0        0      221 2024-05-16 08:37:14.046018 oauth2_cli_auth-1.3.0/oauth2_cli_auth/conftest.py
+-rw-r--r--   0        0        0     7512 2024-05-16 08:37:14.046018 oauth2_cli_auth-1.3.0/oauth2_cli_auth/http_server.py
+-rw-r--r--   0        0        0      985 2024-05-16 08:37:14.046018 oauth2_cli_auth-1.3.0/oauth2_cli_auth/simplified_flow.py
+-rw-r--r--   0        0        0     1235 2024-05-16 08:37:14.046018 oauth2_cli_auth-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     8605 1970-01-01 00:00:00.000000 oauth2_cli_auth-1.3.0/PKG-INFO
```

### Comparing `oauth2_cli_auth-1.2.0/LICENSE` & `oauth2_cli_auth-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oauth2_cli_auth-1.2.0/README.md` & `oauth2_cli_auth-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `oauth2_cli_auth-1.2.0/oauth2_cli_auth/code_grant.py` & `oauth2_cli_auth-1.3.0/oauth2_cli_auth/code_grant.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+import base64
+import urllib.parse
+import urllib.request
 import webbrowser
+from collections.abc import Callable
 from dataclasses import dataclass
-import urllib.request
-import urllib.parse
-import base64
+
 from oauth2_cli_auth._urllib_util import _load_json
 
 
 @dataclass
 class OAuth2ClientInfo:
     """
     Metadata for Oauth2 client
@@ -32,21 +34,23 @@
 
 
 def load_oidc_config(odic_well_known_endpoint: str) -> dict:
     config = _load_json(odic_well_known_endpoint)
     return config
 
 
-def open_browser(url: str) -> None:
+def open_browser(url: str, print_open_browser_instruction: Callable[[str], None] | None = print) -> None:
     """
     Open browser using webbrowser module and show message about URL open
+    :param print_open_browser_instruction: Callback to print the instructions to open the browser. Set to None in order to supress the output.
     :param url: URL to open and display
     :return: None
     """
-    print(f"Open your browser at\n{url}")
+    if print_open_browser_instruction is not None:
+        print_open_browser_instruction(f"Open your browser at\n{url}")
     webbrowser.open(url)
 
 
 def get_auth_url(client_info: OAuth2ClientInfo, redirect_uri: str) -> str:
     """
     Build authorization url for browser
 
@@ -57,25 +61,28 @@
     return (f"{client_info.authorization_url}"
             f"?client_id={client_info.client_id}"
             f"&redirect_uri={redirect_uri}"
             f"&scope={' '.join(client_info.scopes)}"
             f"&response_type=code")
 
 
-def exchange_code_for_access_token(client_info: OAuth2ClientInfo, redirect_uri: str, code: str,
-                                   access_token_field: str = "access_token") -> str:
+def exchange_code_for_response(
+        client_info: OAuth2ClientInfo,
+        redirect_uri: str,
+        code: str,
+) -> dict:
     """
-    Exchange a code for an access token using the endpoints from client info
+    Exchange a code for an access token using the endpoints from client info and return the entire response
 
     :param client_info: Info about oauth2 client
     :param redirect_uri: Callback URL
     :param code: Code to redeem
     :param access_token_field: Name of the field containing the access token to use. This might differ depending on
-                               the provider you are using. For example for Auth0 you have to set this to id_token
-    :return: Extracted access token from response
+                              the provider you are using. For example for Auth0 you have to set this to id_token
+    :return: Response from OAuth2 endpoint
     """
     headers = {
         "Content-Type": "application/x-www-form-urlencoded",
         "Authorization": "Basic " + base64.b64encode(f"{client_info.client_id}:".encode()).decode(),
     }
 
     data = {
@@ -84,8 +91,29 @@
         "grant_type": "authorization_code",
     }
     encoded_data = urllib.parse.urlencode(data).encode('utf-8')
 
     request = urllib.request.Request(client_info.token_url, data=encoded_data, headers=headers)
     json_response = _load_json(request)
 
+    return json_response
+
+
+def exchange_code_for_access_token(
+        client_info: OAuth2ClientInfo,
+        redirect_uri: str,
+        code: str,
+        access_token_field: str = "access_token"
+) -> str:
+    """
+    Exchange a code for an access token using the endpoints from client info
+
+    :param client_info: Info about oauth2 client
+    :param redirect_uri: Callback URL
+    :param code: Code to redeem
+    :param access_token_field: Name of the field containing the access token to use. This might differ depending on
+                               the provider you are using. For example for Auth0 you have to set this to id_token
+    :return: Extracted access token from response
+    """
+    json_response = exchange_code_for_response(client_info, redirect_uri, code)
+
     return json_response.get(access_token_field)
```

### Comparing `oauth2_cli_auth-1.2.0/oauth2_cli_auth/http_server.py` & `oauth2_cli_auth-1.3.0/oauth2_cli_auth/http_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,15 +197,15 @@
     def get_code(self):
         return self._code
 
     @property
     def callback_url(self):
         return f"http://localhost:{self.server_port}"
 
-    def wait_for_code(self, attempts: int = 3, timeout_per_attempt=10) -> Optional[int]:
+    def wait_for_code(self, attempts: int = 3, timeout_per_attempt=10) -> Optional[str]:
         """
         Wait for the server to open the callback page containing the code query parameter.
 
         It tries for #attempts with a timeout of #timeout_per_attempts for each attempt.
         This prevents the CLI from getting stuck by unsolved callback URls
 
         :param attempts: Amount of attempts
```

### Comparing `oauth2_cli_auth-1.2.0/oauth2_cli_auth/simplified_flow.py` & `oauth2_cli_auth-1.3.0/oauth2_cli_auth/simplified_flow.py`

 * *Files identical despite different names*

### Comparing `oauth2_cli_auth-1.2.0/pyproject.toml` & `oauth2_cli_auth-1.3.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oauth2-cli-auth"
-version = "1.2.0"
+version = "1.3.0"
 description = "Authenticate against OAuth2 Provider in Python CLIs"
 authors = ["Timo Reymann <mail@timo-reymann.de>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/timo-reymann/python-oauth2-cli-auth"
 packages = [
     { include = "oauth2_cli_auth" }
@@ -30,16 +30,15 @@
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/timo-reymann/python-oauth2-cli-auth/issues"
 
 [[tool.poetry.source]]
 name = "testpypi"
 url = "https://test.pypi.org/legacy/"
-default = false
-secondary = false
+priority="explicit"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.3"
 coverage = "^7.3.2"
 pdoc3 = "^0.10.0"
 
 [tool.coverage.run]
```

### Comparing `oauth2_cli_auth-1.2.0/PKG-INFO` & `oauth2_cli_auth-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oauth2-cli-auth
-Version: 1.2.0
+Version: 1.3.0
 Summary: Authenticate against OAuth2 Provider in Python CLIs
 Home-page: https://github.com/timo-reymann/python-oauth2-cli-auth
 License: MIT
 Author: Timo Reymann
 Author-email: mail@timo-reymann.de
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,14 +15,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Project-URL: Bug Tracker, https://github.com/timo-reymann/python-oauth2-cli-auth/issues
 Project-URL: Repository, https://github.com/timo-reymann/python-oauth2-cli-auth
 Description-Content-Type: text/markdown
 
 oauth2-cli-auth
 ===
 [![LICENSE](https://img.shields.io/github/license/timo-reymann/python-oauth2-cli-auth)](https://github.com/timo-reymann/python-oauth2-cli-auth/blob/main/LICENSE)
```

