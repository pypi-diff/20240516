# Comparing `tmp/fab_react_toolkit-0.4.8.tar.gz` & `tmp/fab_react_toolkit-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fab_react_toolkit-0.4.8.tar", last modified: Fri May 10 15:21:59 2024, max compression
+gzip compressed data, was "fab_react_toolkit-0.4.9.tar", last modified: Tue May 14 10:18:57 2024, max compression
```

## Comparing `fab_react_toolkit-0.4.8.tar` & `fab_react_toolkit-0.4.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:21:59.027067 fab_react_toolkit-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-10 15:21:50.000000 fab_react_toolkit-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-10 15:21:59.027067 fab_react_toolkit-0.4.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:21:59.023067 fab_react_toolkit-0.4.8/example/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:21:59.023067 fab_react_toolkit-0.4.8/example/app/
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-10 15:21:50.000000 fab_react_toolkit-0.4.8/example/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-10 15:21:50.000000 fab_react_toolkit-0.4.8/example/app/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-10 15:21:50.000000 fab_react_toolkit-0.4.8/example/app/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-10 15:21:50.000000 fab_react_toolkit-0.4.8/example/app/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-10 15:21:50.000000 fab_react_toolkit-0.4.8/example/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-10 15:21:50.000000 fab_react_toolkit-0.4.8/example/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-10 15:21:50.000000 fab_react_toolkit-0.4.8/example/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:21:59.027067 fab_react_toolkit-0.4.8/fab_react_toolkit/
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-10 15:21:50.000000 fab_react_toolkit-0.4.8/fab_react_toolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:21:59.027067 fab_react_toolkit-0.4.8/fab_react_toolkit/api/
--rw-r--r--   0 runner    (1001) docker     (127)    24100 2024-05-10 15:21:50.000000 fab_react_toolkit-0.4.8/fab_react_toolkit/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-05-10 15:21:50.000000 fab_react_toolkit-0.4.8/fab_react_toolkit/api/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-10 15:21:50.000000 fab_react_toolkit-0.4.8/fab_react_toolkit/api/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-10 15:21:50.000000 fab_react_toolkit-0.4.8/fab_react_toolkit/api/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    29193 2024-05-10 15:21:50.000000 fab_react_toolkit-0.4.8/fab_react_toolkit/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)    12522 2024-05-10 15:21:50.000000 fab_react_toolkit-0.4.8/fab_react_toolkit/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-10 15:21:50.000000 fab_react_toolkit-0.4.8/fab_react_toolkit/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-10 15:21:50.000000 fab_react_toolkit-0.4.8/fab_react_toolkit/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:21:59.027067 fab_react_toolkit-0.4.8/fab_react_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-10 15:21:58.000000 fab_react_toolkit-0.4.8/fab_react_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-10 15:21:59.000000 fab_react_toolkit-0.4.8/fab_react_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 15:21:58.000000 fab_react_toolkit-0.4.8/fab_react_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-10 15:21:58.000000 fab_react_toolkit-0.4.8/fab_react_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-10 15:21:58.000000 fab_react_toolkit-0.4.8/fab_react_toolkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-10 15:21:50.000000 fab_react_toolkit-0.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-10 15:21:50.000000 fab_react_toolkit-0.4.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 15:21:59.027067 fab_react_toolkit-0.4.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:18:57.900558 fab_react_toolkit-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-14 10:18:46.000000 fab_react_toolkit-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-14 10:18:57.896558 fab_react_toolkit-0.4.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:18:57.892558 fab_react_toolkit-0.4.9/example/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:18:57.892558 fab_react_toolkit-0.4.9/example/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-14 10:18:46.000000 fab_react_toolkit-0.4.9/example/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-14 10:18:46.000000 fab_react_toolkit-0.4.9/example/app/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-14 10:18:46.000000 fab_react_toolkit-0.4.9/example/app/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-14 10:18:46.000000 fab_react_toolkit-0.4.9/example/app/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-14 10:18:46.000000 fab_react_toolkit-0.4.9/example/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 10:18:46.000000 fab_react_toolkit-0.4.9/example/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-14 10:18:46.000000 fab_react_toolkit-0.4.9/example/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:18:57.896558 fab_react_toolkit-0.4.9/fab_react_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-14 10:18:46.000000 fab_react_toolkit-0.4.9/fab_react_toolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:18:57.896558 fab_react_toolkit-0.4.9/fab_react_toolkit/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    24100 2024-05-14 10:18:46.000000 fab_react_toolkit-0.4.9/fab_react_toolkit/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-05-14 10:18:46.000000 fab_react_toolkit-0.4.9/fab_react_toolkit/api/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-14 10:18:46.000000 fab_react_toolkit-0.4.9/fab_react_toolkit/api/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-14 10:18:46.000000 fab_react_toolkit-0.4.9/fab_react_toolkit/api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29693 2024-05-14 10:18:46.000000 fab_react_toolkit-0.4.9/fab_react_toolkit/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12522 2024-05-14 10:18:46.000000 fab_react_toolkit-0.4.9/fab_react_toolkit/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-14 10:18:46.000000 fab_react_toolkit-0.4.9/fab_react_toolkit/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-14 10:18:46.000000 fab_react_toolkit-0.4.9/fab_react_toolkit/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:18:57.896558 fab_react_toolkit-0.4.9/fab_react_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-14 10:18:57.000000 fab_react_toolkit-0.4.9/fab_react_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-14 10:18:57.000000 fab_react_toolkit-0.4.9/fab_react_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 10:18:57.000000 fab_react_toolkit-0.4.9/fab_react_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-14 10:18:57.000000 fab_react_toolkit-0.4.9/fab_react_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-14 10:18:57.000000 fab_react_toolkit-0.4.9/fab_react_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-14 10:18:46.000000 fab_react_toolkit-0.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-14 10:18:46.000000 fab_react_toolkit-0.4.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 10:18:57.900558 fab_react_toolkit-0.4.9/setup.cfg
```

### Comparing `fab_react_toolkit-0.4.8/LICENSE` & `fab_react_toolkit-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.8/PKG-INFO` & `fab_react_toolkit-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fab-react-toolkit
-Version: 0.4.8
+Version: 0.4.9
 Summary: A small example package
 Author-email: Matthias Leinweber <m.leinweber@datatactics.de>
 Project-URL: Homepage, https://github.com/dttctcs/fab-react-toolkit
 Project-URL: Issues, https://github.com/dttctcs/fab-react-toolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fab_react_toolkit-0.4.8/example/app/__init__.py` & `fab_react_toolkit-0.4.9/example/app/__init__.py`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.8/example/app/apis.py` & `fab_react_toolkit-0.4.9/example/app/apis.py`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.8/example/app/config.py` & `fab_react_toolkit-0.4.9/example/app/config.py`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.8/example/app/models.py` & `fab_react_toolkit-0.4.9/example/app/models.py`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.8/example/run.py` & `fab_react_toolkit-0.4.9/example/run.py`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.8/fab_react_toolkit/__init__.py` & `fab_react_toolkit-0.4.9/fab_react_toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.8/fab_react_toolkit/api/__init__.py` & `fab_react_toolkit-0.4.9/fab_react_toolkit/api/__init__.py`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.8/fab_react_toolkit/api/convert.py` & `fab_react_toolkit-0.4.9/fab_react_toolkit/api/convert.py`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.8/fab_react_toolkit/api/utils.py` & `fab_react_toolkit-0.4.9/fab_react_toolkit/api/utils.py`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.8/fab_react_toolkit/apis.py` & `fab_react_toolkit-0.4.9/fab_react_toolkit/apis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import jwt
 import re
 import datetime
 from apispec import APISpec
 from apispec.ext.marshmallow import MarshmallowPlugin
 from apispec.ext.marshmallow.common import resolve_schema_cls
-from flask import request, redirect, g, current_app
+from flask import request, redirect, g, current_app, url_for
 from flask_login import current_user, login_user, logout_user, login_required
 from flask_appbuilder import expose
 from flask_appbuilder.api import BaseApi, Model2SchemaConverter, safe
 from flask_appbuilder.models.sqla.interface import SQLAInterface
+from flask_appbuilder.utils.base import get_safe_redirect
 from flask_appbuilder.security.manager import AUTH_DB, AUTH_LDAP, AUTH_REMOTE_USER
 from flask_appbuilder.security.sqla.models import User, Permission, PermissionView, Role, ViewMenu
 from werkzeug.security import generate_password_hash
 from flask_appbuilder.const import (
     API_SECURITY_PASSWORD_KEY,
     API_SECURITY_USERNAME_KEY,
 )
@@ -257,28 +258,28 @@
             algorithm="HS256",
         )
 
         try:
             if provider == "twitter":
                 # not works
                 return self.appbuilder.sm.oauth_remotes[provider].authorize_redirect(
-                    redirect_uri=request.base_url + "/callback"
+                    url_for("AuthApi.oauth_authorized", provider=provider, _external=True, state=state)
                 )
             else:
                 return self.appbuilder.sm.oauth_remotes[provider].authorize_redirect(
-                    redirect_uri=request.base_url + "/callback",
+                    url_for("AuthApi.oauth_authorized", provider=provider, _external=True),
                     state=state.decode("ascii") if isinstance(state, bytes) else state,
                 )
 
         except Exception as e:
             print(e)
             return self.response_500()
 
-    @expose("/login/<provider>/callback")
-    def oauth_callback(self, provider):
+    @expose("/oauth-authorized/<provider>")
+    def oauth_authorized(self, provider):
         """OAuth redirect endpoint for the API, creates a session cookie
            Make sure to add this endpoint as the redirect uri of your provider
          ---
           get:
             description: >-
               Authenticate and create a session cookie
             parameters:
@@ -295,15 +296,19 @@
               400:
                 $ref: '#/components/responses/400'
               500:
                 $ref: '#/components/responses/500'
          """
         if provider not in self.appbuilder.sm.oauth_remotes:
             return self.response_400(message="Provider not supported")
-        resp = self.appbuilder.sm.oauth_remotes[provider].authorize_access_token()
+        try:
+          resp = self.appbuilder.sm.oauth_remotes[provider].authorize_access_token()
+        except Exception as e:
+            return self.response_500(message=f"Error authorizing OAuth access token for {str(e)}")
+        
         if resp is None:
             return self.response_400(message="Request for sign in was denied.")
 
         # Retrieves specific user info from the provider
         try:
             self.appbuilder.sm.set_oauth_session(provider, resp)
             userinfo = self.appbuilder.sm.oauth_user_info(provider, resp)
@@ -320,26 +325,32 @@
                         break
                 if not allow:
                     self.response_401()
             user = self.appbuilder.sm.auth_user_oauth(userinfo)
         if user is None:
             return self.response_400(message="Invalid login. Please try again.")
         else:
-            login_user(user)
             try:
                 # redirect uri could be stored in state, I don't see the point though
                 state = jwt.decode(
                     request.args["state"],
                     self.appbuilder.app.config["SECRET_KEY"],
                     algorithms=["HS256"],
                 )
             except jwt.InvalidTokenError:
                 raise Exception("State signature is not valid!")
 
-            return redirect(self.appbuilder.app.config["REDIRECT_URI"])
+            login_user(user)
+
+            next_url = self.appbuilder.app.config["REDIRECT_URI"]
+            # Check if there is a next url on state
+            if "next" in state and len(state["next"]) > 0:
+                next_url = get_safe_redirect(state["next"][0])
+
+            return redirect(next_url)
 
     @expose('/logout', methods=["GET"])
     @safe
     def logout(self):
         """Logs the user out and deletes session cookie"""
         logout_user()
         return self.response(200, message="Logout successful")
```

### Comparing `fab_react_toolkit-0.4.8/fab_react_toolkit/filters.py` & `fab_react_toolkit-0.4.9/fab_react_toolkit/filters.py`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.8/fab_react_toolkit/views.py` & `fab_react_toolkit-0.4.9/fab_react_toolkit/views.py`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.8/fab_react_toolkit.egg-info/PKG-INFO` & `fab_react_toolkit-0.4.9/fab_react_toolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fab-react-toolkit
-Version: 0.4.8
+Version: 0.4.9
 Summary: A small example package
 Author-email: Matthias Leinweber <m.leinweber@datatactics.de>
 Project-URL: Homepage, https://github.com/dttctcs/fab-react-toolkit
 Project-URL: Issues, https://github.com/dttctcs/fab-react-toolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fab_react_toolkit-0.4.8/fab_react_toolkit.egg-info/SOURCES.txt` & `fab_react_toolkit-0.4.9/fab_react_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.8/pyproject.toml` & `fab_react_toolkit-0.4.9/pyproject.toml`

 * *Files identical despite different names*

