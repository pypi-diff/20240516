# Comparing `tmp/aipkgs_core-0.4.6.tar.gz` & `tmp/aipkgs_core-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aipkgs_core-0.4.6.tar", max compression
+gzip compressed data, was "aipkgs_core-1.0.1.tar", max compression
```

## Comparing `aipkgs_core-0.4.6.tar` & `aipkgs_core-1.0.1.tar`

### file list

```diff
@@ -1,36 +1,42 @@
--rw-r--r--   0        0        0     1058 2022-03-08 13:06:48.926815 aipkgs_core-0.4.6/LICENSE.md
--rw-r--r--   0        0        0        0 2022-03-08 13:06:48.926754 aipkgs_core-0.4.6/README.rst
--rw-r--r--   0        0        0      519 2022-09-03 21:38:40.961067 aipkgs_core-0.4.6/aipkgs_core/__init__.py
--rw-r--r--   0        0        0      620 2022-04-01 17:46:38.417317 aipkgs_core-0.4.6/aipkgs_core/encryption/__pycache__/encryption.cpython-38.pyc
--rw-r--r--   0        0        0      621 2022-09-03 21:08:25.855962 aipkgs_core-0.4.6/aipkgs_core/encryption/__pycache__/encryption.cpython-39.pyc
--rw-r--r--   0        0        0     1070 2022-03-08 13:06:48.926158 aipkgs_core-0.4.6/aipkgs_core/encryption/encryption.py
--rw-r--r--   0        0        0     3097 2024-05-15 21:44:20.889369 aipkgs_core-0.4.6/aipkgs_core/jwt/helpers.py
--rw-r--r--   0        0        0      857 2024-05-15 21:41:48.931415 aipkgs_core-0.4.6/aipkgs_core/jwt/model.py
--rw-r--r--   0        0        0      408 2023-10-29 22:52:51.609411 aipkgs_core-0.4.6/aipkgs_core/logger/helpers.py
--rw-r--r--   0        0        0     2124 2022-04-01 17:46:38.433739 aipkgs_core-0.4.6/aipkgs_core/utils/__pycache__/date_helpers.cpython-38.pyc
--rw-r--r--   0        0        0     2161 2022-09-03 21:08:25.861529 aipkgs_core-0.4.6/aipkgs_core/utils/__pycache__/date_helpers.cpython-39.pyc
--rw-r--r--   0        0        0     1655 2022-04-01 17:46:33.794476 aipkgs_core-0.4.6/aipkgs_core/utils/__pycache__/dir_helpers.cpython-38.pyc
--rw-r--r--   0        0        0     1654 2022-09-03 21:01:09.128303 aipkgs_core-0.4.6/aipkgs_core/utils/__pycache__/dir_helpers.cpython-39.pyc
--rw-r--r--   0        0        0      496 2022-04-01 17:46:33.832091 aipkgs_core-0.4.6/aipkgs_core/utils/__pycache__/email.cpython-38.pyc
--rw-r--r--   0        0        0      495 2022-09-03 21:01:09.190830 aipkgs_core-0.4.6/aipkgs_core/utils/__pycache__/email.cpython-39.pyc
--rw-r--r--   0        0        0     1298 2022-04-01 17:46:33.756440 aipkgs_core-0.4.6/aipkgs_core/utils/__pycache__/file_helpers.cpython-38.pyc
--rw-r--r--   0        0        0     1311 2022-09-03 21:01:09.121203 aipkgs_core-0.4.6/aipkgs_core/utils/__pycache__/file_helpers.cpython-39.pyc
--rw-r--r--   0        0        0      930 2022-04-01 17:46:38.432909 aipkgs_core-0.4.6/aipkgs_core/utils/__pycache__/json.cpython-38.pyc
--rw-r--r--   0        0        0      931 2022-09-03 21:08:25.860844 aipkgs_core-0.4.6/aipkgs_core/utils/__pycache__/json.cpython-39.pyc
--rw-r--r--   0        0        0      571 2022-04-01 17:46:38.302196 aipkgs_core-0.4.6/aipkgs_core/utils/__pycache__/phone_number.cpython-38.pyc
--rw-r--r--   0        0        0      572 2022-09-03 21:01:09.369200 aipkgs_core-0.4.6/aipkgs_core/utils/__pycache__/phone_number.cpython-39.pyc
--rw-r--r--   0        0        0     1412 2022-04-01 17:46:38.363966 aipkgs_core-0.4.6/aipkgs_core/utils/__pycache__/string_helpers.cpython-38.pyc
--rw-r--r--   0        0        0     1414 2022-09-03 21:08:25.846360 aipkgs_core-0.4.6/aipkgs_core/utils/__pycache__/string_helpers.cpython-39.pyc
--rw-r--r--   0        0        0      166 2022-04-01 17:46:38.413690 aipkgs_core-0.4.6/aipkgs_core/utils/__pycache__/utils.cpython-38.pyc
--rw-r--r--   0        0        0      167 2022-09-03 21:08:25.855049 aipkgs_core-0.4.6/aipkgs_core/utils/__pycache__/utils.cpython-39.pyc
--rw-r--r--   0        0        0     2196 2022-04-01 17:48:43.916256 aipkgs_core-0.4.6/aipkgs_core/utils/date_helpers.py
--rw-r--r--   0        0        0     1315 2022-03-11 08:48:14.567742 aipkgs_core-0.4.6/aipkgs_core/utils/dir_helpers.py
--rw-r--r--   0        0        0     1084 2024-05-14 10:16:31.693520 aipkgs_core-0.4.6/aipkgs_core/utils/email.py
--rw-r--r--   0        0        0      700 2022-03-08 13:06:48.925633 aipkgs_core-0.4.6/aipkgs_core/utils/file_helpers.py
--rw-r--r--   0        0        0      827 2022-03-08 13:06:48.925703 aipkgs_core-0.4.6/aipkgs_core/utils/json.py
--rw-r--r--   0        0        0      304 2022-03-08 13:06:48.926210 aipkgs_core-0.4.6/aipkgs_core/utils/phone_number.py
--rw-r--r--   0        0        0     1542 2022-08-20 15:51:07.521999 aipkgs_core-0.4.6/aipkgs_core/utils/singleton.py
--rw-r--r--   0        0        0     1105 2022-09-03 21:08:23.013667 aipkgs_core-0.4.6/aipkgs_core/utils/string_helpers.py
--rw-r--r--   0        0        0      654 2024-05-09 14:48:47.729452 aipkgs_core-0.4.6/aipkgs_core/utils/utils.py
--rw-r--r--   0        0        0     1013 2024-05-15 21:44:36.868193 aipkgs_core-0.4.6/pyproject.toml
--rw-r--r--   0        0        0      824 1970-01-01 00:00:00.000000 aipkgs_core-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0     1058 2022-03-08 13:06:48.926815 aipkgs_core-1.0.1/LICENSE.md
+-rw-r--r--   0        0        0        0 2022-03-08 13:06:48.926754 aipkgs_core-1.0.1/README.rst
+-rw-r--r--   0        0        0      519 2022-09-03 21:38:40.961067 aipkgs_core-1.0.1/aipkgs_core/__init__.py
+-rw-r--r--   0        0        0     4379 2024-05-15 21:48:55.750080 aipkgs_core-1.0.1/aipkgs_core/decorators/flask_decorators.py
+-rw-r--r--   0        0        0      505 2024-05-12 01:53:30.572535 aipkgs_core-1.0.1/aipkgs_core/decorators/headers.py
+-rw-r--r--   0        0        0      620 2022-04-01 17:46:38.417317 aipkgs_core-1.0.1/aipkgs_core/encryption/__pycache__/encryption.cpython-38.pyc
+-rw-r--r--   0        0        0      621 2022-09-03 21:08:25.855962 aipkgs_core-1.0.1/aipkgs_core/encryption/__pycache__/encryption.cpython-39.pyc
+-rw-r--r--   0        0        0     1070 2022-03-08 13:06:48.926158 aipkgs_core-1.0.1/aipkgs_core/encryption/encryption.py
+-rw-r--r--   0        0        0     3145 2024-05-15 21:50:25.991984 aipkgs_core-1.0.1/aipkgs_core/jwt/helpers.py
+-rw-r--r--   0        0        0      857 2024-05-15 21:41:48.931415 aipkgs_core-1.0.1/aipkgs_core/jwt/model.py
+-rw-r--r--   0        0        0      408 2023-10-29 22:52:51.609411 aipkgs_core-1.0.1/aipkgs_core/logger/helpers.py
+-rw-r--r--   0        0        0     1864 2024-05-15 21:54:07.642852 aipkgs_core-1.0.1/aipkgs_core/responses/error.py
+-rw-r--r--   0        0        0     1418 2024-05-15 21:52:09.876274 aipkgs_core-1.0.1/aipkgs_core/responses/response.py
+-rw-r--r--   0        0        0     1000 2024-05-15 21:52:27.080619 aipkgs_core-1.0.1/aipkgs_core/responses/success.py
+-rw-r--r--   0        0        0      435 2024-05-15 21:52:21.512199 aipkgs_core-1.0.1/aipkgs_core/responses/verbose.py
+-rw-r--r--   0        0        0     2124 2022-04-01 17:46:38.433739 aipkgs_core-1.0.1/aipkgs_core/utils/__pycache__/date_helpers.cpython-38.pyc
+-rw-r--r--   0        0        0     2161 2022-09-03 21:08:25.861529 aipkgs_core-1.0.1/aipkgs_core/utils/__pycache__/date_helpers.cpython-39.pyc
+-rw-r--r--   0        0        0     1655 2022-04-01 17:46:33.794476 aipkgs_core-1.0.1/aipkgs_core/utils/__pycache__/dir_helpers.cpython-38.pyc
+-rw-r--r--   0        0        0     1654 2022-09-03 21:01:09.128303 aipkgs_core-1.0.1/aipkgs_core/utils/__pycache__/dir_helpers.cpython-39.pyc
+-rw-r--r--   0        0        0      496 2022-04-01 17:46:33.832091 aipkgs_core-1.0.1/aipkgs_core/utils/__pycache__/email.cpython-38.pyc
+-rw-r--r--   0        0        0      495 2022-09-03 21:01:09.190830 aipkgs_core-1.0.1/aipkgs_core/utils/__pycache__/email.cpython-39.pyc
+-rw-r--r--   0        0        0     1298 2022-04-01 17:46:33.756440 aipkgs_core-1.0.1/aipkgs_core/utils/__pycache__/file_helpers.cpython-38.pyc
+-rw-r--r--   0        0        0     1311 2022-09-03 21:01:09.121203 aipkgs_core-1.0.1/aipkgs_core/utils/__pycache__/file_helpers.cpython-39.pyc
+-rw-r--r--   0        0        0      930 2022-04-01 17:46:38.432909 aipkgs_core-1.0.1/aipkgs_core/utils/__pycache__/json.cpython-38.pyc
+-rw-r--r--   0        0        0      931 2022-09-03 21:08:25.860844 aipkgs_core-1.0.1/aipkgs_core/utils/__pycache__/json.cpython-39.pyc
+-rw-r--r--   0        0        0      571 2022-04-01 17:46:38.302196 aipkgs_core-1.0.1/aipkgs_core/utils/__pycache__/phone_number.cpython-38.pyc
+-rw-r--r--   0        0        0      572 2022-09-03 21:01:09.369200 aipkgs_core-1.0.1/aipkgs_core/utils/__pycache__/phone_number.cpython-39.pyc
+-rw-r--r--   0        0        0     1412 2022-04-01 17:46:38.363966 aipkgs_core-1.0.1/aipkgs_core/utils/__pycache__/string_helpers.cpython-38.pyc
+-rw-r--r--   0        0        0     1414 2022-09-03 21:08:25.846360 aipkgs_core-1.0.1/aipkgs_core/utils/__pycache__/string_helpers.cpython-39.pyc
+-rw-r--r--   0        0        0      166 2022-04-01 17:46:38.413690 aipkgs_core-1.0.1/aipkgs_core/utils/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0        0        0      167 2022-09-03 21:08:25.855049 aipkgs_core-1.0.1/aipkgs_core/utils/__pycache__/utils.cpython-39.pyc
+-rw-r--r--   0        0        0     2196 2022-04-01 17:48:43.916256 aipkgs_core-1.0.1/aipkgs_core/utils/date_helpers.py
+-rw-r--r--   0        0        0     1315 2022-03-11 08:48:14.567742 aipkgs_core-1.0.1/aipkgs_core/utils/dir_helpers.py
+-rw-r--r--   0        0        0     1084 2024-05-14 10:16:31.693520 aipkgs_core-1.0.1/aipkgs_core/utils/email.py
+-rw-r--r--   0        0        0      700 2022-03-08 13:06:48.925633 aipkgs_core-1.0.1/aipkgs_core/utils/file_helpers.py
+-rw-r--r--   0        0        0      827 2022-03-08 13:06:48.925703 aipkgs_core-1.0.1/aipkgs_core/utils/json.py
+-rw-r--r--   0        0        0      304 2022-03-08 13:06:48.926210 aipkgs_core-1.0.1/aipkgs_core/utils/phone_number.py
+-rw-r--r--   0        0        0     1542 2022-08-20 15:51:07.521999 aipkgs_core-1.0.1/aipkgs_core/utils/singleton.py
+-rw-r--r--   0        0        0     1105 2022-09-03 21:08:23.013667 aipkgs_core-1.0.1/aipkgs_core/utils/string_helpers.py
+-rw-r--r--   0        0        0      654 2024-05-09 14:48:47.729452 aipkgs_core-1.0.1/aipkgs_core/utils/utils.py
+-rw-r--r--   0        0        0     1040 2024-05-15 21:54:37.601153 aipkgs_core-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      872 1970-01-01 00:00:00.000000 aipkgs_core-1.0.1/PKG-INFO
```

### Comparing `aipkgs_core-0.4.6/LICENSE.md` & `aipkgs_core-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.6/aipkgs_core/__init__.py` & `aipkgs_core-1.0.1/aipkgs_core/__init__.py`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.6/aipkgs_core/encryption/__pycache__/encryption.cpython-38.pyc` & `aipkgs_core-1.0.1/aipkgs_core/encryption/__pycache__/encryption.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.6/aipkgs_core/encryption/__pycache__/encryption.cpython-39.pyc` & `aipkgs_core-1.0.1/aipkgs_core/encryption/__pycache__/encryption.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.6/aipkgs_core/encryption/encryption.py` & `aipkgs_core-1.0.1/aipkgs_core/encryption/encryption.py`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.6/aipkgs_core/jwt/helpers.py` & `aipkgs_core-1.0.1/aipkgs_core/jwt/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,45 @@
+from aipkgs_requests import status
 from flask import jsonify, make_response
 from flask_jwt_extended import JWTManager, create_access_token, create_refresh_token, get_jwt_identity, get_jwt
 
 from aipkgs_core.jwt.model import JWTModel
 
-HTTP_401_UNAUTHORIZED = 401
-
 
 class JWTHelper:
     @staticmethod
     def fire(jwt: JWTManager):
         # The following callbacks are used for customizing jwt response/error messages.
         # The original ones may not be in a very pretty format (opinionated)
         @jwt.expired_token_loader
         def expired_token_callback(jwt_header, jwt_data):
             model = JWTModel(jwt_data)
             if model.is_access():
-                return make_response(jsonify({"message": "The token has expired.", "error": "token_expired"}), HTTP_401_UNAUTHORIZED)
+                return make_response(jsonify({"message": "The token has expired.", "error": "token_expired"}), status.HTTP_401_UNAUTHORIZED)
             else:
-                return make_response(jsonify({"message": "The token has expired.", "error": "token_expired"}), HTTP_401_UNAUTHORIZED)
+                return make_response(jsonify({"message": "The token has expired.", "error": "token_expired"}), status.HTTP_401_UNAUTHORIZED)
 
         @jwt.invalid_token_loader
         def invalid_token_callback(error):  # we have to keep the argument here, since it's passed in by the caller internally
-            return make_response(jsonify({"message": "Signature verification failed.", "error": "invalid_token"}), HTTP_401_UNAUTHORIZED)
+            return make_response(jsonify({"message": "Signature verification failed.", "error": "invalid_token"}), status.HTTP_401_UNAUTHORIZED)
 
         @jwt.unauthorized_loader
         def missing_token_callback(error):
             return make_response(jsonify({
                 "description": "Request does not contain an access token.",
                 "error": "authorization_required",
-            }), HTTP_401_UNAUTHORIZED)
+            }), status.HTTP_401_UNAUTHORIZED)
 
         @jwt.needs_fresh_token_loader
         def token_not_fresh_callback(jwt_header, jwt_data):
-            return make_response(jsonify({"description": "The token is not fresh.", "error": "fresh_token_required"}), HTTP_401_UNAUTHORIZED)
+            return make_response(jsonify({"description": "The token is not fresh.", "error": "fresh_token_required"}), status.HTTP_401_UNAUTHORIZED)
 
         @jwt.revoked_token_loader
         def revoked_token_callback(jwt_header, jwt_data):  # called on blacklisted
-            return make_response(jsonify({"description": "The token has been revoked.", "error": "token_revoked"}), HTTP_401_UNAUTHORIZED)  # tokens
+            return make_response(jsonify({"description": "The token has been revoked.", "error": "token_revoked"}), status.HTTP_401_UNAUTHORIZED)  # tokens
 
 
 class AuthHelper:
     @staticmethod
     def generate_new_tokens(identity: str, fresh: bool = None, additional_claims: {} = None) -> (str, str):
         additional_claims = additional_claims if additional_claims else {}
         access_token = AuthHelper.generate_access_token(identity=identity, fresh=fresh or False, additional_claims=additional_claims)
```

### Comparing `aipkgs_core-0.4.6/aipkgs_core/jwt/model.py` & `aipkgs_core-1.0.1/aipkgs_core/jwt/model.py`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.6/aipkgs_core/utils/__pycache__/date_helpers.cpython-38.pyc` & `aipkgs_core-1.0.1/aipkgs_core/utils/__pycache__/date_helpers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.6/aipkgs_core/utils/__pycache__/date_helpers.cpython-39.pyc` & `aipkgs_core-1.0.1/aipkgs_core/utils/__pycache__/date_helpers.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.6/aipkgs_core/utils/__pycache__/dir_helpers.cpython-38.pyc` & `aipkgs_core-1.0.1/aipkgs_core/utils/__pycache__/dir_helpers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.6/aipkgs_core/utils/__pycache__/dir_helpers.cpython-39.pyc` & `aipkgs_core-1.0.1/aipkgs_core/utils/__pycache__/dir_helpers.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.6/aipkgs_core/utils/__pycache__/file_helpers.cpython-38.pyc` & `aipkgs_core-1.0.1/aipkgs_core/utils/__pycache__/file_helpers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.6/aipkgs_core/utils/__pycache__/file_helpers.cpython-39.pyc` & `aipkgs_core-1.0.1/aipkgs_core/utils/__pycache__/file_helpers.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.6/aipkgs_core/utils/__pycache__/json.cpython-38.pyc` & `aipkgs_core-1.0.1/aipkgs_core/utils/__pycache__/json.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.6/aipkgs_core/utils/__pycache__/json.cpython-39.pyc` & `aipkgs_core-1.0.1/aipkgs_core/utils/__pycache__/json.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.6/aipkgs_core/utils/__pycache__/phone_number.cpython-38.pyc` & `aipkgs_core-1.0.1/aipkgs_core/utils/__pycache__/phone_number.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.6/aipkgs_core/utils/__pycache__/phone_number.cpython-39.pyc` & `aipkgs_core-1.0.1/aipkgs_core/utils/__pycache__/phone_number.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.6/aipkgs_core/utils/__pycache__/string_helpers.cpython-38.pyc` & `aipkgs_core-1.0.1/aipkgs_core/utils/__pycache__/string_helpers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.6/aipkgs_core/utils/__pycache__/string_helpers.cpython-39.pyc` & `aipkgs_core-1.0.1/aipkgs_core/utils/__pycache__/string_helpers.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.6/aipkgs_core/utils/date_helpers.py` & `aipkgs_core-1.0.1/aipkgs_core/utils/date_helpers.py`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.6/aipkgs_core/utils/dir_helpers.py` & `aipkgs_core-1.0.1/aipkgs_core/utils/dir_helpers.py`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.6/aipkgs_core/utils/email.py` & `aipkgs_core-1.0.1/aipkgs_core/utils/email.py`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.6/aipkgs_core/utils/file_helpers.py` & `aipkgs_core-1.0.1/aipkgs_core/utils/file_helpers.py`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.6/aipkgs_core/utils/json.py` & `aipkgs_core-1.0.1/aipkgs_core/utils/json.py`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.6/aipkgs_core/utils/singleton.py` & `aipkgs_core-1.0.1/aipkgs_core/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.6/aipkgs_core/utils/string_helpers.py` & `aipkgs_core-1.0.1/aipkgs_core/utils/string_helpers.py`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.6/aipkgs_core/utils/utils.py` & `aipkgs_core-1.0.1/aipkgs_core/utils/utils.py`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.6/pyproject.toml` & `aipkgs_core-1.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core>=1.0.1"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "aipkgs-core"
-version = "0.4.6"
+version = "1.0.1"
 description = "Core package for aipy packages."
 authors = ["Alexy <alexy.ib@outlook.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://gitlab.com/aipy/public/packages.git"
 repository = "https://gitlab.com/aipy/public/packages.git"
 keywords = ["ai"]
@@ -34,14 +34,15 @@
 requests = "^2.28.1"
 pendulum = "^2.0.0"
 email-validator = "^2.1.1"
 emoji = "^2.11.1"
 phonenumbers = "^8.13.36"
 bcrypt = "^4.1.3"
 flask-jwt-extended = "^4.6.0"
+aipkgs-requests = "^0.1.4"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [tool.poetry.group.dev.dependencies]
 autopep8 = "^2.0.1"
```

### Comparing `aipkgs_core-0.4.6/PKG-INFO` & `aipkgs_core-1.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: aipkgs-core
-Version: 0.4.6
+Version: 1.0.1
 Summary: Core package for aipy packages.
 Home-page: https://gitlab.com/aipy/public/packages.git
 License: MIT
 Keywords: ai
 Author: Alexy
 Author-email: alexy.ib@outlook.com
 Requires-Python: >=3.11.3,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: aipkgs-requests (>=0.1.4,<0.2.0)
 Requires-Dist: bcrypt (>=4.1.3,<5.0.0)
 Requires-Dist: email-validator (>=2.1.1,<3.0.0)
 Requires-Dist: emoji (>=2.11.1,<3.0.0)
 Requires-Dist: flask-jwt-extended (>=4.6.0,<5.0.0)
 Requires-Dist: pendulum (>=2.0.0,<3.0.0)
 Requires-Dist: phonenumbers (>=8.13.36,<9.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
```

