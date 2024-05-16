# Comparing `tmp/appmesh-0.9.7-py3-none-any.whl.zip` & `tmp/appmesh-0.9.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 15945 bytes, number of entries: 6
--rw-r--r--  2.0 unx       11 b- defN 24-May-08 12:01 appmesh/__init__.py
--rw-r--r--  2.0 unx    58043 b- defN 24-May-08 12:01 appmesh/appmesh_client.py
--rw-r--r--  2.0 unx    10786 b- defN 24-May-08 12:01 appmesh-0.9.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-08 12:01 appmesh-0.9.7.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-May-08 12:01 appmesh-0.9.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      455 b- defN 24-May-08 12:01 appmesh-0.9.7.dist-info/RECORD
-6 files, 69395 bytes uncompressed, 15123 bytes compressed:  78.2%
+Zip file size: 16100 bytes, number of entries: 6
+-rw-r--r--  2.0 unx       11 b- defN 24-May-16 06:19 appmesh/__init__.py
+-rw-r--r--  2.0 unx    58878 b- defN 24-May-16 06:19 appmesh/appmesh_client.py
+-rw-r--r--  2.0 unx    10786 b- defN 24-May-16 06:20 appmesh-0.9.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-16 06:20 appmesh-0.9.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-May-16 06:20 appmesh-0.9.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      455 b- defN 24-May-16 06:20 appmesh-0.9.8.dist-info/RECORD
+6 files, 70230 bytes uncompressed, 15278 bytes compressed:  78.2%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: appmesh/__init__.py
 Comment: 
 
 Filename: appmesh/appmesh_client.py
 Comment: 
 
-Filename: appmesh-0.9.7.dist-info/METADATA
+Filename: appmesh-0.9.8.dist-info/METADATA
 Comment: 
 
-Filename: appmesh-0.9.7.dist-info/WHEEL
+Filename: appmesh-0.9.8.dist-info/WHEEL
 Comment: 
 
-Filename: appmesh-0.9.7.dist-info/top_level.txt
+Filename: appmesh-0.9.8.dist-info/top_level.txt
 Comment: 
 
-Filename: appmesh-0.9.7.dist-info/RECORD
+Filename: appmesh-0.9.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## appmesh/appmesh_client.py

```diff
@@ -12,14 +12,15 @@
 
 from enum import Enum, unique
 from http import HTTPStatus
 from urllib import parse
 from datetime import datetime
 import requests
 
+# pylint: disable=broad-exception-raised,line-too-long
 
 DEFAULT_TOKEN_EXPIRE_SECONDS = "P1W"  # default 7 day(s)
 DEFAULT_RUN_APP_TIMEOUT_SECONDS = "PT1H"  # 1 hour
 DEFAULT_RUN_APP_LIFECYCLE_SECONDS = "PT10H"  # 10 hours
 REST_TEXT_MESSAGE_JSON_KEY = "message"
 MESSAGE_ENCODING_UTF8 = "utf-8"
 TCP_MESSAGE_HEADER_LENGTH = 4
@@ -49,29 +50,33 @@
 class App(object):
     """
     App object present an application in App Mesh
     """
 
     @unique
     class Permission(Enum):
-        Deny = "1"
-        Read = "2"
-        Write = "3"
+        """Application permission definition"""
+
+        DENY = "1"
+        READ = "2"
+        WRITE = "3"
 
     class Behavior(object):
         """
         Application error handling behavior definition object
         """
 
         @unique
         class Action(Enum):
-            Restart = "restart"
-            Standby = "standby"
-            Keepalive = "keepalive"
-            Remove = "remove"
+            """Application exit behavior definition"""
+
+            RESTART = "restart"
+            STANDBY = "standby"
+            KEEPALIVE = "keepalive"
+            REMOVE = "remove"
 
         def __init__(self, data=None) -> None:
             if isinstance(data, (str, bytes, bytearray)):
                 data = json.loads(data)
             # default exit behavior [restart,standby,keepalive,remove]
             self.exit = _get_str_item(data, "exit")
             # exit code behavior (e.g, --control 0:restart --control 1:standby), higher priority than default exit behavior
@@ -131,14 +136,16 @@
         # application name
         self.name = _get_str_item(data, "name")
         # full command line with arguments
         self.command = _get_str_item(data, "command")
 
         # use shell mode, cmd can be more shell commands with string format
         self.shell = _get_bool_item(data, "shell")
+        # app run in session login mode
+        self.session_login = _get_bool_item(data, "session_login")
         # application description
         self.description = _get_str_item(data, "description")
         # metadata string/JSON (input for application, pass to process stdin)
         self.metadata = _get_native_item(data, "metadata")
         # working directory
         self.working_dir = _get_str_item(data, "working_dir")
         # initial application status (true is enable, false is disabled)
@@ -254,16 +261,15 @@
         Returns:
             int: return exit code if process finished, return None for timeout or exception.
         """
         return self.__client.run_async_wait(self, stdout_print, timeout)
 
 
 class AppMeshClient(metaclass=abc.ABCMeta):
-    """
-    Client object used to access App Mesh REST Service
+    """App Mesh client object used to access App Mesh REST Service
 
     - install pip package: python3 -m pip install --upgrade appmesh
     - import module: from appmesh import appmesh_client
     """
 
     @unique
     class Method(Enum):
@@ -326,15 +332,15 @@
         Args:
             user_name (str): the name of the user.
             user_pwd (str): the password of the user.
             totp_code (str, optional): the TOTP code if enabled for the user.
             timeout_seconds (int | str, optional): token expire timeout of seconds. support ISO 8601 durations (e.g., 'P1Y2M3DT4H5M6S' 'P1W').
 
         Returns:
-            str: JWT token if verify success, otherwise return None.
+            str: JWT token.
         """
         self.jwt_token = None
         resp = self._request_http(
             AppMeshClient.Method.POST,
             path="/appmesh/login",
             header={
                 "Username": base64.b64encode(user_name.encode()),
@@ -357,58 +363,51 @@
                     "Expire-Seconds": self._parse_duration(timeout_seconds),
                 },
             )
             if resp.status_code == HTTPStatus.OK:
                 if "Access-Token" in resp.json():
                     self.jwt_token = resp.json()["Access-Token"]
             else:
-                print(resp.text)
+                raise Exception(resp.text)
         else:
-            print(resp.text)
-            # resp.raise_for_status()
+            raise Exception(resp.text)
         return self.jwt_token
 
     def logoff(self) -> bool:
         """Logoff current session from server
 
         Returns:
             bool: logoff success or failure.
         """
         resp = self._request_http(AppMeshClient.Method.POST, path="/appmesh/self/logoff")
-        if resp.status_code == HTTPStatus.OK:
-            return True
-        else:
-            # resp.raise_for_status()
-            print(resp.text)
-            return False
+        if resp.status_code != HTTPStatus.OK:
+            raise Exception(resp.text)
+        return resp.status_code == HTTPStatus.OK
 
     def authentication(self, token: str, permission=None) -> bool:
         """Login with token and verify permission when specified
 
         Args:
             token (str): JWT token returned from login().
             permission (str, optional): the permission ID used to verify the token user
                 permission ID can be:
-                - pre-defined by App Mesh from security.json (e.g 'app-view', 'app-delete')
-                - defined by input from role_update() or security.json
+                - pre-defined by App Mesh from security.yaml (e.g 'app-view', 'app-delete')
+                - defined by input from role_update() or security.yaml
 
         Returns:
             bool: authentication success or failure.
         """
         self.jwt_token = token
         headers = {}
         if permission:
             headers["Auth-Permission"] = permission
         resp = self._request_http(AppMeshClient.Method.POST, path="/appmesh/auth", header=headers)
-        if resp.status_code == HTTPStatus.OK:
-            return True
-        else:
-            # resp.raise_for_status()
-            print(resp.text)
-            return False
+        if resp.status_code != HTTPStatus.OK:
+            raise Exception(resp.text)
+        return resp.status_code == HTTPStatus.OK
 
     def renew(self, timeout_seconds=DEFAULT_TOKEN_EXPIRE_SECONDS) -> str:
         """Renew current token
 
         Args:
             timeout_seconds (int | str, optional): token expire timeout of seconds. support ISO 8601 durations (e.g., 'P1Y2M3DT4H5M6S' 'P1W').
 
@@ -422,33 +421,28 @@
             header={
                 "Expire-Seconds": self._parse_duration(timeout_seconds),
             },
         )
         if resp.status_code == HTTPStatus.OK:
             if "Access-Token" in resp.json():
                 self.jwt_token = resp.json()["Access-Token"]
-        else:
-            print(resp.text)
-            # resp.raise_for_status()
-        return self.jwt_token
+                return self.jwt_token
+        raise Exception(resp.text)
 
     def totp_secret(self) -> str:
         """Generate TOTP secret for current login user and return MFA URI with JSON body
 
         Returns:
             str: TOTP secret str
         """
         resp = self._request_http(method=AppMeshClient.Method.POST, path="/appmesh/totp/secret")
         if resp.status_code == HTTPStatus.OK:
             totp_uri = base64.b64decode(resp.json()["Mfa-Uri"]).decode()
             return self._parse_totp_uri(totp_uri).get("secret")
-        else:
-            print(resp.text)
-            # resp.raise_for_status()
-        return None
+        raise Exception(resp.text)
 
     def totp_setup(self, totp_code: str) -> bool:
         """Setup 2FA for current login user
 
         Args:
             totp_code (str): TOTP code
 
@@ -456,14 +450,16 @@
             bool: success or failure.
         """
         resp = self._request_http(
             method=AppMeshClient.Method.POST,
             path=f"/appmesh/totp/setup",
             header={"Totp": base64.b64encode(totp_code.encode())},
         )
+        if resp.status_code != HTTPStatus.OK:
+            raise Exception(resp.text)
         return resp.status_code == HTTPStatus.OK
 
     def totp_disable(self, user="self") -> bool:
         """Disable 2FA for current user
 
         Args:
             user (str, optional): user name for disable TOTP.
@@ -471,15 +467,17 @@
         Returns:
             bool: success or failure.
         """
         resp = self._request_http(
             method=AppMeshClient.Method.POST,
             path=f"/appmesh/totp/{user}/disable",
         )
-        return (resp.status_code == HTTPStatus.OK), resp.json()[REST_TEXT_MESSAGE_JSON_KEY]
+        if resp.status_code != HTTPStatus.OK:
+            raise Exception(resp.text)
+        return resp.status_code == HTTPStatus.OK
 
     @staticmethod
     def _parse_totp_uri(totp_uri: str) -> dict:
         """Extract TOTP parameters
 
         Args:
             totp_uri (str): TOTP uri
@@ -565,25 +563,27 @@
                 "timeout": str(timeout),
             },
         )
         out_position = None if not resp.headers.__contains__("Output-Position") else int(resp.headers["Output-Position"])
         exit_code = None if not resp.headers.__contains__("Exit-Code") else int(resp.headers["Exit-Code"])
         return (resp.status_code == HTTPStatus.OK), resp.text, out_position, exit_code
 
-    def app_health(self, app_name: str):
+    def app_health(self, app_name: str) -> int:
         """Get application health status, 0 is health.
 
         Args:
             app_name (str): the application name.
 
         Returns:
-            str: '0' is heathy, '1' is unhealthy.
+            int: '0' is heathy, '1' is unhealthy.
         """
         resp = self._request_http(AppMeshClient.Method.GET, path=f"/appmesh/app/{app_name}/health")
-        return (resp.status_code == HTTPStatus.OK), resp.text
+        if resp.status_code != HTTPStatus.OK:
+            raise Exception(resp.text)
+        return int(resp.text)
 
     ########################################
     # Application manage
     ########################################
     def app_add(self, app: App) -> App:
         """Register an application
 
@@ -597,78 +597,83 @@
             failed request
         """
         resp = self._request_http(AppMeshClient.Method.PUT, path="/appmesh/app/{0}".format(app.name), body=app.json())
         if resp.status_code != HTTPStatus.OK:
             raise Exception(resp.text)
         return App(resp.json())
 
-    def app_delete(self, app_name: str):
+    def app_delete(self, app_name: str) -> bool:
         """Remove an application.
 
         Args:
             app_name (str): the application name.
 
         Returns:
             bool: success or failure.
-            str: text message.
         """
         resp = self._request_http(AppMeshClient.Method.DELETE, path=f"/appmesh/app/{app_name}")
-        return (resp.status_code == HTTPStatus.OK), resp.json()[REST_TEXT_MESSAGE_JSON_KEY]
+        if resp.status_code != HTTPStatus.OK:
+            raise Exception(resp.text)
+        return resp.status_code == HTTPStatus.OK
 
-    def app_enable(self, app_name: str):
+    def app_enable(self, app_name: str) -> bool:
         """Enable an application
 
         Args:
             app_name (str): the application name.
 
         Returns:
             bool: success or failure.
-            str: text message.
         """
         resp = self._request_http(AppMeshClient.Method.POST, path=f"/appmesh/app/{app_name}/enable")
-        return (resp.status_code == HTTPStatus.OK), resp.json()[REST_TEXT_MESSAGE_JSON_KEY]
+        if resp.status_code != HTTPStatus.OK:
+            raise Exception(resp.text)
+        return resp.status_code == HTTPStatus.OK
 
-    def app_disable(self, app_name: str):
+    def app_disable(self, app_name: str) -> bool:
         """Stop and disable an application
 
         Args:
             app_name (str): the application name.
 
         Returns:
             bool: success or failure.
-            str: text message.
         """
         resp = self._request_http(AppMeshClient.Method.POST, path=f"/appmesh/app/{app_name}/disable")
-        return (resp.status_code == HTTPStatus.OK), resp.json()[REST_TEXT_MESSAGE_JSON_KEY]
+        if resp.status_code != HTTPStatus.OK:
+            raise Exception(resp.text)
+        return resp.status_code == HTTPStatus.OK
 
     ########################################
     # Cloud management
     ########################################
-    def cloud_app_view_all(self):
+    def cloud_app_view_all(self) -> dict:
         """Get all cloud applications
 
         Returns:
-            bool: success or failure.
             dict: cloud applications in JSON format.
         """
         resp = self._request_http(AppMeshClient.Method.GET, path="/appmesh/cloud/applications")
-        return (resp.status_code == HTTPStatus.OK), resp.json()
+        if resp.status_code != HTTPStatus.OK:
+            raise Exception(resp.text)
+        return resp.json()
 
-    def cloud_app(self, app_name: str):
+    def cloud_app(self, app_name: str) -> dict:
         """Get an cloud application
 
         Args:
             app_name (str): the application name.
 
         Returns:
-            bool: success or failure.
             dict: application in JSON format.
         """
         resp = self._request_http(AppMeshClient.Method.GET, path=f"/appmesh/cloud/app/{app_name}")
-        return (resp.status_code == HTTPStatus.OK), resp.json()
+        if resp.status_code != HTTPStatus.OK:
+            raise Exception(resp.text)
+        return resp.json()
 
     def cloud_app_output(self, app_name: str, host_name: str, stdout_position: int = 0, stdout_index: int = 0, stdout_maxsize: int = 10240, process_uuid: str = ""):
         """Get cloud application stdout/stderr from master agent
 
         Args:
             app_name (str): the application name
             host_name (str): the target host name where the application is running
@@ -704,118 +709,124 @@
         Args:
             app_name (str): The application name for cloud
 
         Returns:
             bool: success or failure.
         """
         resp = self._request_http(AppMeshClient.Method.DELETE, path=f"/appmesh/cloud/app/{app_name}")
+        if resp.status_code != HTTPStatus.OK:
+            raise Exception(resp.text)
         return resp.status_code == HTTPStatus.OK
 
-    def cloud_app_add(self, app_json: dict):
+    def cloud_app_add(self, app_json: dict) -> dict:
         """Add a cloud application
 
         Args:
             app_json (dict): the cloud application definition with replication, condition and resource requirement
 
          Returns:
-            bool: success or failure.
             dict: cluster application json.
         """
         resp = self._request_http(AppMeshClient.Method.PUT, path="/appmesh/cloud/app/{0}".format(app_json["content"]["name"]), body=app_json)
-        return (resp.status_code == HTTPStatus.OK), resp.json()
+        if resp.status_code != HTTPStatus.OK:
+            raise Exception(resp.text)
+        return resp.json()
 
-    def cloud_nodes(self):
+    def cloud_nodes(self) -> dict:
         """Get cluster node list
 
         Returns:
-            bool: success or failure.
             dict: cluster node list json.
         """
         resp = self._request_http(AppMeshClient.Method.GET, path="/appmesh/cloud/nodes")
-        return (resp.status_code == HTTPStatus.OK), resp.json()
+        if resp.status_code != HTTPStatus.OK:
+            raise Exception(resp.text)
+        return resp.json()
 
     ########################################
     # Configuration
     ########################################
-    def host_resource(self):
+    def host_resource(self) -> dict:
         """Get App Mesh host resource report include CPU, memory and disk
 
         Returns:
-            bool: success or failure.
             dict: the host resource json.
         """
         resp = self._request_http(AppMeshClient.Method.GET, path="/appmesh/resources")
-        return (resp.status_code == HTTPStatus.OK), resp.json()
+        if resp.status_code != HTTPStatus.OK:
+            raise Exception(resp.text)
+        return resp.json()
 
-    def config_view(self):
+    def config_view(self) -> dict:
         """Get App Mesh configuration JSON
 
         Returns:
-            bool: success or failure.
             dict: the configuration json.
         """
         resp = self._request_http(AppMeshClient.Method.GET, path="/appmesh/config")
-        return (resp.status_code == HTTPStatus.OK), resp.json()
+        if resp.status_code != HTTPStatus.OK:
+            raise Exception(resp.text)
+        return resp.json()
 
-    def config_set(self, cfg_json):
-        """Update configuration, the format follow 'config.json', support partial update
+    def config_set(self, cfg_json) -> dict:
+        """Update configuration, the format follow 'config.yaml', support partial update
 
         Args:
             cfg_json (dict): the new configuration json.
 
         Returns:
-            bool: success or failure.
             dict: the updated configuration json.
         """
         resp = self._request_http(AppMeshClient.Method.POST, path="/appmesh/config", body=cfg_json)
-        result = resp.json()
-        return (resp.status_code == HTTPStatus.OK), result
+        if resp.status_code != HTTPStatus.OK:
+            raise Exception(resp.text)
+        return resp.json()
 
-    def log_level_set(self, level: str = "DEBUG"):
+    def log_level_set(self, level: str = "DEBUG") -> str:
         """Update App Mesh log level(DEBUG/INFO/NOTICE/WARN/ERROR), a wrapper of config_set()
 
         Args:
             level (str, optional): log level.
 
         Returns:
-            bool: success or failure.
-            dict: the updated configuration json.
+            str: the updated log level.
         """
         resp = self._request_http(AppMeshClient.Method.POST, path="/appmesh/config", body={"LogLevel": level})
-        if resp.status_code == HTTPStatus.OK:
-            return True, resp.json()["LogLevel"]
-        return (resp.status_code == HTTPStatus.OK), resp.json()
+        if resp.status_code != HTTPStatus.OK:
+            raise Exception(resp.text)
+        return resp.json()["LogLevel"]
 
     ########################################
     # User Management
     ########################################
-    def user_passwd_update(self, new_password: str, user_name: str = "self"):
+    def user_passwd_update(self, new_password: str, user_name: str = "self") -> bool:
         """Change user password
 
         Args:
             user_name (str): the user name.
             new_password (str):the new password string
 
         Returns:
-            bool: success or failure.
-            str: result message.
+            bool: success
         """
         resp = self._request_http(
             method=AppMeshClient.Method.POST,
             path=f"/appmesh/user/{user_name}/passwd",
             header={"New-Password": base64.b64encode(new_password.encode())},
         )
-        return (resp.status_code == HTTPStatus.OK), resp.json()[REST_TEXT_MESSAGE_JSON_KEY]
+        if resp.status_code != HTTPStatus.OK:
+            raise Exception(resp.text)
+        return True
 
     def user_add(self, user_name: str, user_json: dict) -> bool:
         """Add a new user, not available for LDAP user
 
         Args:
             user_name (str): the user name.
-            user_json (dict): user definition, follow same user format from security.json.
+            user_json (dict): user definition, follow same user format from security.yaml.
 
         Returns:
             bool: success or failure.
         """
         resp = self._request_http(
             method=AppMeshClient.Method.PUT,
             path=f"/appmesh/user/{user_name}",
@@ -847,14 +858,16 @@
         Returns:
             bool: success or failure.
         """
         resp = self._request_http(
             method=AppMeshClient.Method.POST,
             path=f"/appmesh/user/{user_name}/lock",
         )
+        if resp.status_code != HTTPStatus.OK:
+            raise Exception(resp.text)
         return resp.status_code == HTTPStatus.OK
 
     def user_unlock(self, user_name: str) -> bool:
         """Unlock a user
 
         Args:
             user_name (str): the user name.
@@ -862,87 +875,97 @@
         Returns:
             bool: success or failure.
         """
         resp = self._request_http(
             method=AppMeshClient.Method.POST,
             path=f"/appmesh/user/{user_name}/unlock",
         )
+        if resp.status_code != HTTPStatus.OK:
+            raise Exception(resp.text)
         return resp.status_code == HTTPStatus.OK
 
-    def users_view(self):
+    def users_view(self) -> dict:
         """Get all users
 
         Returns:
-            bool: success or failure.
-            dict: all user definition.
+            dict: all user definition
         """
         resp = self._request_http(method=AppMeshClient.Method.GET, path="/appmesh/users")
-        return (resp.status_code == HTTPStatus.OK), resp.json()
+        if resp.status_code != HTTPStatus.OK:
+            raise Exception(resp.text)
+        return resp.json()
 
-    def user_self(self):
+    def user_self(self) -> dict:
         """Get current user infomation
 
         Returns:
-            bool: success or failure.
             dict: user definition.
         """
         resp = self._request_http(method=AppMeshClient.Method.GET, path="/appmesh/user/self")
-        return (resp.status_code == HTTPStatus.OK), resp.json()
+        if resp.status_code != HTTPStatus.OK:
+            raise Exception(resp.text)
+        return resp.json()
 
-    def groups_view(self):
+    def groups_view(self) -> list:
         """Get all user groups
 
         Returns:
-            bool: success or failure.
             dict: user group array.
         """
         resp = self._request_http(method=AppMeshClient.Method.GET, path="/appmesh/user/groups")
-        return (resp.status_code == HTTPStatus.OK), resp.json()
+        if resp.status_code != HTTPStatus.OK:
+            raise Exception(resp.text)
+        return resp.json()
 
-    def permissions_view(self):
+    def permissions_view(self) -> list:
         """Get all available permissions
 
         Returns:
-            bool: success or failure.
-            dict: permission array.
+            dict: permission array
         """
         resp = self._request_http(method=AppMeshClient.Method.GET, path="/appmesh/permissions")
-        return (resp.status_code == HTTPStatus.OK), resp.json()
+        if resp.status_code != HTTPStatus.OK:
+            raise Exception(resp.text)
+        return resp.json()
 
-    def permissions_for_user(self):
+    def permissions_for_user(self) -> list:
         """Get current user permissions
 
         Returns:
-            bool: success or failure.
             dict: user permission array.
         """
         resp = self._request_http(method=AppMeshClient.Method.GET, path="/appmesh/user/permissions")
-        return (resp.status_code == HTTPStatus.OK), resp.json()
+        if resp.status_code != HTTPStatus.OK:
+            raise Exception(resp.text)
+        return resp.json()
 
-    def roles_view(self):
+    def roles_view(self) -> list:
         """Get all roles with permission definition
 
         Returns:
-            bool: success or failure.
             dict: all role definition.
         """
         resp = self._request_http(method=AppMeshClient.Method.GET, path="/appmesh/roles")
-        return (resp.status_code == HTTPStatus.OK), resp.json()
+        if resp.status_code != HTTPStatus.OK:
+            raise Exception(resp.text)
+        return resp.json()
 
     def role_update(self, role_name: str, role_permission_json: dict) -> bool:
         """Update (or add) a role with defined permissions, the permission ID can be App Mesh pre-defined or other permission ID.
 
         Args:
             role_name (str): the role name.
             role_permission_json (dict): role permission definition array, e.g: ["app-control", "app-delete", "cloud-app-reg", "cloud-app-delete"]
 
         Returns:
             bool: success or failure.
         """
         resp = self._request_http(method=AppMeshClient.Method.POST, path=f"/appmesh/role/{role_name}", body=role_permission_json)
+        if resp.status_code != HTTPStatus.OK:
+            raise Exception(resp.text)
         return resp.status_code == HTTPStatus.OK
 
     def role_delete(self, role_name: str) -> bool:
         """Delete a user role
 
         Args:
             role_name (str): the role name.
@@ -950,14 +973,16 @@
         Returns:
             bool: success or failure.
         """
         resp = self._request_http(
             method=AppMeshClient.Method.DELETE,
             path=f"/appmesh/role/{role_name}",
         )
+        if resp.status_code != HTTPStatus.OK:
+            raise Exception(resp.text)
         return resp.status_code == HTTPStatus.OK
 
     ########################################
     # Tag management
     ########################################
     def tag_add(self, tag_name: str, tag_value: str) -> bool:
         """Add a new label
@@ -970,50 +995,56 @@
             bool: success or failure.
         """
         resp = self._request_http(
             AppMeshClient.Method.PUT,
             query={"value": tag_value},
             path=f"/appmesh/label/{tag_name}",
         )
+        if resp.status_code != HTTPStatus.OK:
+            raise Exception(resp.text)
         return resp.status_code == HTTPStatus.OK
 
     def tag_delete(self, tag_name: str) -> bool:
         """Delete a label
 
         Args:
             tag_name (str): the label name.
 
         Returns:
             bool: success or failure.
         """
         resp = self._request_http(AppMeshClient.Method.DELETE, path=f"/appmesh/label/{tag_name}")
+        if resp.status_code != HTTPStatus.OK:
+            raise Exception(resp.text)
         return resp.status_code == HTTPStatus.OK
 
-    def tag_view(self):
+    def tag_view(self) -> dict:
         """Get the server labels
 
         Returns:
-            bool: success or failure.
             dict: label data.
         """
         resp = self._request_http(AppMeshClient.Method.GET, path="/appmesh/labels")
-        return (resp.status_code == HTTPStatus.OK), resp.json()
+        if resp.status_code != HTTPStatus.OK:
+            raise Exception(resp.text)
+        return resp.json()
 
     ########################################
     # Promethus metrics
     ########################################
     def metrics(self):
         """Prometheus metrics (this does not call Prometheus API /metrics, just copy the same metrics data)
 
         Returns:
-            bool: success or failure.
             str: prometheus metrics texts
         """
         resp = self._request_http(AppMeshClient.Method.GET, path="/appmesh/metrics")
-        return resp.status_code == HTTPStatus.OK, resp.text
+        if resp.status_code != HTTPStatus.OK:
+            raise Exception(resp.text)
+        return resp.text
 
     ########################################
     # File management
     ########################################
     def file_download(self, file_path: str, local_file: str) -> bool:
         """Copy a remote file to local, the local file will have the same permission as the remote file
 
@@ -1021,45 +1052,45 @@
             file_path (str): the remote file path.
             local_file (str): the local file path to be downloaded.
 
         Returns:
             bool: success or failure.
         """
         resp = self._request_http(AppMeshClient.Method.GET, path="/appmesh/file/download", header={"File-Path": file_path})
-        if resp.status_code == HTTPStatus.OK:
-            with open(local_file, "wb") as fp:
-                for chunk in resp.iter_content(chunk_size=512):
-                    if chunk:
-                        fp.write(chunk)
-            if resp.headers.__contains__("File-Mode"):
-                os.chmod(path=local_file, mode=int(resp.headers["File-Mode"]))
-            if resp.headers.__contains__("File-User") and resp.headers.__contains__("File-Group"):
-                file_uid = int(resp.headers["File-User"])
-                file_gid = int(resp.headers["File-Group"])
-                try:
-                    os.chown(path=local_file, uid=file_uid, gid=file_gid)
-                except Exception as ex:
-                    print(ex)
-            return True
-        return False
+        if resp.status_code != HTTPStatus.OK:
+            raise Exception(resp.text)
+
+        with open(local_file, "wb") as fp:
+            for chunk in resp.iter_content(chunk_size=512):
+                if chunk:
+                    fp.write(chunk)
+        if resp.headers.__contains__("File-Mode"):
+            os.chmod(path=local_file, mode=int(resp.headers["File-Mode"]))
+        if resp.headers.__contains__("File-User") and resp.headers.__contains__("File-Group"):
+            file_uid = int(resp.headers["File-User"])
+            file_gid = int(resp.headers["File-Group"])
+            try:
+                os.chown(path=local_file, uid=file_uid, gid=file_gid)
+            except Exception as ex:
+                print(ex)
+        return resp.status_code == HTTPStatus.OK
 
-    def file_upload(self, local_file: str, file_path: str):
+    def file_upload(self, local_file: str, file_path: str) -> bool:
         """Upload a local file to the remote server, the remote file will have the same permission as the local file
 
         Dependency:
             sudo apt install python3-pip
             pip3 install requests_toolbelt
 
         Args:
             local_file (str): the local file path.
             file_path (str): the target remote file to be uploaded.
 
         Returns:
             bool: success or failure.
-            str: text message.
         """
         from requests_toolbelt import MultipartEncoder
 
         with open(file=local_file, mode="rb") as fp:
             encoder = MultipartEncoder(fields={"filename": os.path.basename(file_path), "file": ("filename", fp, "application/octet-stream")})
             file_stat = os.stat(local_file)
             header = {}
@@ -1071,17 +1102,17 @@
             # https://stackoverflow.com/questions/22567306/python-requests-file-upload
             resp = self._request_http(
                 AppMeshClient.Method.POST_STREAM,
                 path="/appmesh/file/upload",
                 header=header,
                 body=encoder,
             )
-            if resp.status_code == HTTPStatus.OK:
-                return True, ""
-            return False, resp.json()[REST_TEXT_MESSAGE_JSON_KEY]
+            if resp.status_code != HTTPStatus.OK:
+                raise Exception(resp.text)
+        return True
 
     ########################################
     # Application run
     ########################################
     def _parse_duration(self, timeout) -> str:
         if isinstance(timeout, int):
             return str(timeout)
@@ -1210,23 +1241,15 @@
         if method is AppMeshClient.Method.GET:
             return requests.get(url=rest_url, params=query, headers=header, cert=self.ssl_client_cert, verify=self.ssl_verify, timeout=self.rest_timeout)
         elif method is AppMeshClient.Method.POST:
             return requests.post(
                 url=rest_url, params=query, headers=header, data=json.dumps(body) if type(body) in (dict, list) else body, cert=self.ssl_client_cert, verify=self.ssl_verify, timeout=self.rest_timeout
             )
         elif method is AppMeshClient.Method.POST_STREAM:
-            return requests.post(
-                url=rest_url,
-                params=query,
-                headers=header,
-                data=body,
-                cert=self.ssl_client_cert,
-                verify=self.ssl_verify,
-                stream=True,
-            )
+            return requests.post(url=rest_url, params=query, headers=header, data=body, cert=self.ssl_client_cert, verify=self.ssl_verify, stream=True, timeout=self.rest_timeout)
         elif method is AppMeshClient.Method.DELETE:
             return requests.delete(url=rest_url, headers=header, cert=self.ssl_client_cert, verify=self.ssl_verify, timeout=self.rest_timeout)
         elif method is AppMeshClient.Method.PUT:
             return requests.put(url=rest_url, params=query, headers=header, json=body, cert=self.ssl_client_cert, verify=self.ssl_verify, timeout=self.rest_timeout)
         else:
             raise Exception("Invalid http method", method)
```

## Comparing `appmesh-0.9.7.dist-info/METADATA` & `appmesh-0.9.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appmesh
-Version: 0.9.7
+Version: 0.9.8
 Summary: Client SDK for App Mesh
 Home-page: https://github.com/laoshanxi/app-mesh
 Author: laoshanxi
 Author-email: 178029200@qq.com
 License: MIT
 Keywords: appmesh AppMesh app-mesh
 Classifier: Programming Language :: Python :: 3
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: appmesh Version: 0.9.7 Summary: Client SDK for App
+Metadata-Version: 2.1 Name: appmesh Version: 0.9.8 Summary: Client SDK for App
 Mesh Home-page: https://github.com/laoshanxi/app-mesh Author: laoshanxi Author-
 email: 178029200@qq.com License: MIT Keywords: appmesh AppMesh app-mesh
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown Requires-Dist:
 requests Requires-Dist: msgpack Requires-Dist: requests-toolbelt Requires-Dist:
 aniso8601 ï»¿[![language.badge]][language.url] [![standard.badge]]
```

