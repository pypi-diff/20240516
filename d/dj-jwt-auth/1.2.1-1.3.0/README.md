# Comparing `tmp/dj-jwt-auth-1.2.1.tar.gz` & `tmp/dj-jwt-auth-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj-jwt-auth-1.2.1.tar", last modified: Tue Mar 26 12:44:08 2024, max compression
+gzip compressed data, was "dj-jwt-auth-1.3.0.tar", last modified: Thu May 16 16:26:57 2024, max compression
```

## Comparing `dj-jwt-auth-1.2.1.tar` & `dj-jwt-auth-1.3.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 12:44:08.924437 dj-jwt-auth-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-03-26 12:44:08.924437 dj-jwt-auth-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-03-26 12:43:57.000000 dj-jwt-auth-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 12:44:08.924437 dj-jwt-auth-1.2.1/dj_jwt_auth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-03-26 12:44:08.000000 dj-jwt-auth-1.2.1/dj_jwt_auth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-03-26 12:44:08.000000 dj-jwt-auth-1.2.1/dj_jwt_auth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 12:44:08.000000 dj-jwt-auth-1.2.1/dj_jwt_auth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-26 12:44:08.000000 dj-jwt-auth-1.2.1/dj_jwt_auth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-26 12:44:08.000000 dj-jwt-auth-1.2.1/dj_jwt_auth.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 12:44:08.924437 dj-jwt-auth-1.2.1/django_jwt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 12:43:57.000000 dj-jwt-auth-1.2.1/django_jwt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-03-26 12:43:57.000000 dj-jwt-auth-1.2.1/django_jwt/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-26 12:43:57.000000 dj-jwt-auth-1.2.1/django_jwt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-03-26 12:43:57.000000 dj-jwt-auth-1.2.1/django_jwt/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-26 12:43:57.000000 dj-jwt-auth-1.2.1/django_jwt/pkce.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-03-26 12:43:57.000000 dj-jwt-auth-1.2.1/django_jwt/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-03-26 12:43:57.000000 dj-jwt-auth-1.2.1/django_jwt/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-03-26 12:43:57.000000 dj-jwt-auth-1.2.1/django_jwt/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-03-26 12:43:57.000000 dj-jwt-auth-1.2.1/django_jwt/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-03-26 12:43:57.000000 dj-jwt-auth-1.2.1/django_jwt/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-03-26 12:43:57.000000 dj-jwt-auth-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-03-26 12:44:08.924437 dj-jwt-auth-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-26 12:43:57.000000 dj-jwt-auth-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 12:44:08.924437 dj-jwt-auth-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 12:43:57.000000 dj-jwt-auth-1.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-03-26 12:43:57.000000 dj-jwt-auth-1.2.1/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-03-26 12:43:57.000000 dj-jwt-auth-1.2.1/tests/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-26 12:43:57.000000 dj-jwt-auth-1.2.1/tests/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:26:57.102511 dj-jwt-auth-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-05-16 16:26:57.102511 dj-jwt-auth-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-05-16 16:26:46.000000 dj-jwt-auth-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:26:57.102511 dj-jwt-auth-1.3.0/dj_jwt_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-05-16 16:26:57.000000 dj-jwt-auth-1.3.0/dj_jwt_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-16 16:26:57.000000 dj-jwt-auth-1.3.0/dj_jwt_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 16:26:57.000000 dj-jwt-auth-1.3.0/dj_jwt_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-16 16:26:57.000000 dj-jwt-auth-1.3.0/dj_jwt_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-16 16:26:57.000000 dj-jwt-auth-1.3.0/dj_jwt_auth.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:26:57.102511 dj-jwt-auth-1.3.0/django_jwt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 16:26:46.000000 dj-jwt-auth-1.3.0/django_jwt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-16 16:26:46.000000 dj-jwt-auth-1.3.0/django_jwt/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-16 16:26:46.000000 dj-jwt-auth-1.3.0/django_jwt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-16 16:26:46.000000 dj-jwt-auth-1.3.0/django_jwt/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-16 16:26:46.000000 dj-jwt-auth-1.3.0/django_jwt/pkce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-16 16:26:46.000000 dj-jwt-auth-1.3.0/django_jwt/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-16 16:26:46.000000 dj-jwt-auth-1.3.0/django_jwt/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5163 2024-05-16 16:26:46.000000 dj-jwt-auth-1.3.0/django_jwt/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-16 16:26:46.000000 dj-jwt-auth-1.3.0/django_jwt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-05-16 16:26:46.000000 dj-jwt-auth-1.3.0/django_jwt/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-16 16:26:46.000000 dj-jwt-auth-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-16 16:26:57.106511 dj-jwt-auth-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-16 16:26:46.000000 dj-jwt-auth-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:26:57.102511 dj-jwt-auth-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 16:26:46.000000 dj-jwt-auth-1.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-16 16:26:46.000000 dj-jwt-auth-1.3.0/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7432 2024-05-16 16:26:46.000000 dj-jwt-auth-1.3.0/tests/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-16 16:26:46.000000 dj-jwt-auth-1.3.0/tests/urls.py
```

### Comparing `dj-jwt-auth-1.2.1/PKG-INFO` & `dj-jwt-auth-1.3.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,89 +1,99 @@
-Metadata-Version: 2.1
-Name: dj-jwt-auth
-Version: 1.2.1
-Summary: A Django package for JSON Web Token validation and verification. Using PyJWT.
-Home-page: https://www.example.com/
-Author: Konstantin Seleznev
-Author-email: k.seleznev@elsevier.com
-License: MIT
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 # Django-JWT
 
 This is a package to verify and validate JSON Web Tokens (JWT) in Django.
 
 ### Installation
-1. Install the package using pip.
+1. Install the package using pip:
+```bash
+    pip install dj-jwt-auth
+```
 
 2. Add "django_jwt" to your INSTALLED_APPS setting like this::
 ```
     INSTALLED_APPS = [
         ...
-        'django_jwt',
+        "django_jwt",
     ]
 ```
 
 3. Add "django_jwt.middleware.JWTAuthMiddleware" to your MIDDLEWARE setting like this::
 ```
     MIDDLEWARE = [
         ...
-        'django_jwt.middleware.JWTAuthMiddleware',
+        "django_jwt.middleware.JWTAuthMiddleware",
     ]
 ```
 
 ### Configuration:
 Required variables:
-- OIDC_CONFIG_ROUTES - dict of 'algorithm': 'config_url', by default is empty. If filled will be used instead of OIDC_CERTS_URL
+- OIDC_CONFIG_ROUTES - dict of "algorithm": "config_url". Required for using JWTAuthMiddleware. Example: 
 ```
    OIDC_CONFIG_ROUTES = {
-       'RS256': 'https://keyCloak/realms/h/.well-known/openid-configuration',
-       'HS256': 'https://keyCloak/realms/h/.well-known/openid-configuration',
+       "RS256": "https://keyCloak/realms/h/.well-known/openid-configuration",
+       "HS256": "https://keyCloak/realms/h/.well-known/openid-configuration",
    } 
 ```
-
 Optional variables:
 - OIDC_AUDIENCE - by default ["account", "broker"]
+
 User retated variables:
 - OIDC_USER_UPDATE - if True, user model will be updated from userinfo endpoint if MODIFIED date has changed, by default True
 - OIDC_USER_MODIFIED_FIELD - user model field to store last modified date, by default `modified_timestamp`
 - OIDC_TOKEN_MODIFIED_FIELD - access token field to store last modified date, by default `updated_at`
-- OIDC_USER_UID - User model' unique identifier, by default `kc_id`
+- OIDC_USER_UID - User model" unique identifier, by default `kc_id`
 - OIDC_USER_MAPPING - mapping between JWT claims and user model fields, by default:
 ```
     OIDC_USER_MAPPING = {
-        'first_name': 'first_name',
-        'last_name': 'last_name',
-        'username': 'username',
+        "first_name": "first_name",
+        "last_name": "last_name",
+        "username": "username",
     }
 ```
 - OIDC_USER_DEFAULTS - default values for user model fields, by default:
 ```
     OIDC_USER_DEFAULTS = {
-        'is_active': True,
+        "is_active": True,
     }
 ```
 
 - OIDC_USER_ON_CREATE and OIDC_USER_ON_UPDATE - functions to be called on user creation and update, by default:
 ```
     OIDC_USER_ON_CREATE = None
     OIDC_USER_ON_UPDATE = None
 ```
-- OIDC_ADMIN_ISSUER - URL of the OIDC provider, by default None
 These functions should accept two arguments: user and request.
 
+### Admin panel integration:
+To integrate admin panel with OIDC, add OIDC_ADMIN_ISSUER and OIDC_ADMIN_CLIENT_ID to settings.
+- OIDC_ADMIN_ISSUER - required for admin-panel access through OIDC. Example: 
+```
+    OIDC_ADMIN_ISSUER = "https://keyCloak/realms/h/.well-known/openid-configuration"
+```
+- OIDC_ADMIN_CLIENT_ID - by default "complete-anatomy"
+To mapping roles to admin panel permissions, use OIDC_ADMIN_ROLES. Example:
+```python
+from django_jwt.user import ROLE
+
+OIDC_ADMIN_ROLES = [
+    ROLE(
+        name="admin",  # name from token
+        is_superuser=True,
+    ),
+    ROLE(
+        name="staff",
+        groups=["LMS (Full)", "Organizations (Full)", "Customer Support (Full)"],
+        permissions=["Can add user"],
+    ),
+]
+```
+And add login view to urls.py:
+```python
+urlpatterns = [
+    path("admin/", include("django_jwt.urls")),
+    ...
+]
+```
+Login URL will be available at `/admin/oidc/`.
+
 ### Testing:
-Run command `python runtests.py` to run tests.
+Run command `python runtests.py` to run tests.
```

### Comparing `dj-jwt-auth-1.2.1/django_jwt/config.py` & `dj-jwt-auth-1.3.0/django_jwt/config.py`

 * *Files identical despite different names*

### Comparing `dj-jwt-auth-1.2.1/django_jwt/middleware.py` & `dj-jwt-auth-1.3.0/django_jwt/middleware.py`

 * *Files identical despite different names*

### Comparing `dj-jwt-auth-1.2.1/django_jwt/pkce.py` & `dj-jwt-auth-1.3.0/django_jwt/pkce.py`

 * *Files identical despite different names*

### Comparing `dj-jwt-auth-1.2.1/django_jwt/settings.py` & `dj-jwt-auth-1.3.0/django_jwt/settings.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,7 +35,13 @@
     None,
 )
 
 OIDC_CONFIG_ROUTES = getattr(settings, "OIDC_CONFIG_ROUTES", None)
 OIDC_ADMIN_ISSUER = getattr(settings, "OIDC_ADMIN_ISSUER", None)
 OIDC_ADMIN_CLIENT_ID = getattr(settings, "OIDC_ADMIN_CLIENT_ID", "complete-anatomy")
 OIDC_ADMIN_SCOPE = getattr(settings, "OIDC_ADMIN_SCOPE", "openid")
+OIDC_ADMIN_ROLES = getattr(settings, "OIDC_ADMIN_ROLES", [])
+
+for role in OIDC_ADMIN_ROLES:
+    from django_jwt.user import ROLE
+
+    assert isinstance(role, ROLE), f"Role must be a namedtuple, got {type(role)}"
```

### Comparing `dj-jwt-auth-1.2.1/django_jwt/user.py` & `dj-jwt-auth-1.3.0/django_jwt/user.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,25 @@
+from collections import namedtuple
 from datetime import datetime
+from functools import cache
 from logging import getLogger
 
 import pytz
 from django.contrib.auth import get_user_model
+from django.contrib.auth.models import Group, Permission
 from django.http.request import HttpRequest
 
 from django_jwt import settings
 from django_jwt.utils import oidc_handler
 
 utc = pytz.UTC
 log = getLogger(__name__)
 
 model = get_user_model()
+ROLE = namedtuple("Role", ["name", "is_superuser", "groups", "permissions"], defaults=["", False, [], []])
 
 
 class UserHandler:
     modified_at = None
 
     def __init__(self, payload: dict, request: HttpRequest, access_token: str):
         # payload of access token without user info
@@ -96,7 +100,49 @@
 
         except model.DoesNotExist:
             self._collect_user_data()
             try:
                 return self._get_by_email()
             except model.DoesNotExist:
                 return self._create_new_user()
+
+
+class RoleHandler:
+    """
+    Process user roles and permissions from access token.
+    Token be like:
+    ...
+    "resource_access": {
+        "complete_anatomy": {
+            "roles": [
+                "admin"
+            ]
+        }
+    },
+    """
+
+    @property
+    def roles(self) -> dict:
+        return {role.name: role for role in settings.OIDC_ADMIN_ROLES}
+
+    @cache
+    def get_permissions(self, role_name: str) -> Permission:
+        return Permission.objects.filter(codename__in=self.roles[role_name].permissions)
+
+    @cache
+    def get_groups(self, role_name: str) -> Group:
+        return Group.objects.filter(name__in=self.roles[role_name].groups)
+
+    def apply(self, user: model, access_token: dict):
+        token_roles = access_token.get("resource_access", {}).get(settings.OIDC_ADMIN_CLIENT_ID, {}).get("roles", [])
+        for role_name in token_roles:
+            if role_name in self.roles:
+                role = self.roles[role_name]
+                user.groups.add(*self.get_groups(role_name))
+                user.user_permissions.add(*self.get_permissions(role_name))
+                if role.is_superuser != user.is_superuser:
+                    user.is_superuser = role.is_superuser
+                    user.save(update_fields=["is_superuser"])
+                break
+
+
+role_handler = RoleHandler()
```

### Comparing `dj-jwt-auth-1.2.1/django_jwt/utils.py` & `dj-jwt-auth-1.3.0/django_jwt/utils.py`

 * *Files identical despite different names*

### Comparing `dj-jwt-auth-1.2.1/django_jwt/views.py` & `dj-jwt-auth-1.3.0/django_jwt/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from django.views import View
 from requests.exceptions import HTTPError
 
 from django_jwt import settings as jwt_settings
 from django_jwt.config import config
 from django_jwt.exceptions import BadRequestException, ConfigException
 from django_jwt.pkce import PKCESecret
-from django_jwt.user import UserHandler
+from django_jwt.user import UserHandler, role_handler
 from django_jwt.utils import get_access_token, oidc_handler
 
 log = getLogger(__name__)
 
 
 def silent_sso_check(request):
     return HttpResponse("<html><body><script>parent.postMessage(location.href, location.origin)</script></body></html>")
@@ -77,13 +77,14 @@
 
         redirect_uri = request.build_absolute_uri(reverse("receive_redirect_view"))
         if state := cache.get(state):
             token = get_access_token(code, redirect_uri, state)
             data = oidc_handler.decode_token(token)
             user = UserHandler(data, request, token).get_user()
             log.info(f"OIDC Admin login: {user}", extra={"data": data})
+            role_handler.apply(user, data)
             if not user.is_staff:
                 raise BadRequestException("User is not staff")
             login(request, user, backend=settings.DEFAULT_AUTHENTICATION_BACKEND)
             return redirect("admin:index")
 
         raise BadRequestException("No PKCE secret found in cache")
```

### Comparing `dj-jwt-auth-1.2.1/setup.cfg` & `dj-jwt-auth-1.3.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dj-jwt-auth
-version = 1.2.1
+version = 1.3.0
 description = A Django package for JSON Web Token validation and verification. Using PyJWT.
 long_description = file: README.md
 url = https://www.example.com/
 author = Konstantin Seleznev
 author_email = k.seleznev@elsevier.com
 license = MIT
 classifiers =
```

