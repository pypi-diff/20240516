# Comparing `tmp/aipkgs_core-1.0.8.tar.gz` & `tmp/aipkgs_core-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aipkgs_core-1.0.8.tar", max compression
+gzip compressed data, was "aipkgs_core-1.0.9.tar", max compression
```

## Comparing `aipkgs_core-1.0.8.tar` & `aipkgs_core-1.0.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1058 2022-03-08 13:06:48.926815 aipkgs_core-1.0.8/LICENSE.md
--rw-r--r--   0        0        0        0 2022-03-08 13:06:48.926754 aipkgs_core-1.0.8/README.rst
--rw-r--r--   0        0        0      519 2022-09-03 21:38:40.961067 aipkgs_core-1.0.8/aipkgs_core/__init__.py
--rw-r--r--   0        0        0      708 2024-05-15 23:27:14.638083 aipkgs_core-1.0.8/aipkgs_core/decorators/helpers.py
--rw-r--r--   0        0        0      620 2022-04-01 17:46:38.417317 aipkgs_core-1.0.8/aipkgs_core/encryption/__pycache__/encryption.cpython-38.pyc
--rw-r--r--   0        0        0      621 2022-09-03 21:08:25.855962 aipkgs_core-1.0.8/aipkgs_core/encryption/__pycache__/encryption.cpython-39.pyc
--rw-r--r--   0        0        0     1070 2022-03-08 13:06:48.926158 aipkgs_core-1.0.8/aipkgs_core/encryption/encryption.py
--rw-r--r--   0        0        0     3145 2024-05-15 21:50:25.991984 aipkgs_core-1.0.8/aipkgs_core/jwt/helpers.py
--rw-r--r--   0        0        0      857 2024-05-15 21:41:48.931415 aipkgs_core-1.0.8/aipkgs_core/jwt/model.py
--rw-r--r--   0        0        0      408 2023-10-29 22:52:51.609411 aipkgs_core-1.0.8/aipkgs_core/logger/helpers.py
--rw-r--r--   0        0        0     1864 2024-05-15 21:54:07.642852 aipkgs_core-1.0.8/aipkgs_core/responses/error.py
--rw-r--r--   0        0        0     1418 2024-05-15 21:52:09.876274 aipkgs_core-1.0.8/aipkgs_core/responses/response.py
--rw-r--r--   0        0        0     1000 2024-05-15 21:52:27.080619 aipkgs_core-1.0.8/aipkgs_core/responses/success.py
--rw-r--r--   0        0        0      435 2024-05-15 21:52:21.512199 aipkgs_core-1.0.8/aipkgs_core/responses/verbose.py
--rw-r--r--   0        0        0     2124 2022-04-01 17:46:38.433739 aipkgs_core-1.0.8/aipkgs_core/utils/__pycache__/date_helpers.cpython-38.pyc
--rw-r--r--   0        0        0     2161 2022-09-03 21:08:25.861529 aipkgs_core-1.0.8/aipkgs_core/utils/__pycache__/date_helpers.cpython-39.pyc
--rw-r--r--   0        0        0     1655 2022-04-01 17:46:33.794476 aipkgs_core-1.0.8/aipkgs_core/utils/__pycache__/dir_helpers.cpython-38.pyc
--rw-r--r--   0        0        0     1654 2022-09-03 21:01:09.128303 aipkgs_core-1.0.8/aipkgs_core/utils/__pycache__/dir_helpers.cpython-39.pyc
--rw-r--r--   0        0        0      496 2022-04-01 17:46:33.832091 aipkgs_core-1.0.8/aipkgs_core/utils/__pycache__/email.cpython-38.pyc
--rw-r--r--   0        0        0      495 2022-09-03 21:01:09.190830 aipkgs_core-1.0.8/aipkgs_core/utils/__pycache__/email.cpython-39.pyc
--rw-r--r--   0        0        0     1298 2022-04-01 17:46:33.756440 aipkgs_core-1.0.8/aipkgs_core/utils/__pycache__/file_helpers.cpython-38.pyc
--rw-r--r--   0        0        0     1311 2022-09-03 21:01:09.121203 aipkgs_core-1.0.8/aipkgs_core/utils/__pycache__/file_helpers.cpython-39.pyc
--rw-r--r--   0        0        0      930 2022-04-01 17:46:38.432909 aipkgs_core-1.0.8/aipkgs_core/utils/__pycache__/json.cpython-38.pyc
--rw-r--r--   0        0        0      931 2022-09-03 21:08:25.860844 aipkgs_core-1.0.8/aipkgs_core/utils/__pycache__/json.cpython-39.pyc
--rw-r--r--   0        0        0      571 2022-04-01 17:46:38.302196 aipkgs_core-1.0.8/aipkgs_core/utils/__pycache__/phone_number.cpython-38.pyc
--rw-r--r--   0        0        0      572 2022-09-03 21:01:09.369200 aipkgs_core-1.0.8/aipkgs_core/utils/__pycache__/phone_number.cpython-39.pyc
--rw-r--r--   0        0        0     1412 2022-04-01 17:46:38.363966 aipkgs_core-1.0.8/aipkgs_core/utils/__pycache__/string_helpers.cpython-38.pyc
--rw-r--r--   0        0        0     1414 2022-09-03 21:08:25.846360 aipkgs_core-1.0.8/aipkgs_core/utils/__pycache__/string_helpers.cpython-39.pyc
--rw-r--r--   0        0        0      166 2022-04-01 17:46:38.413690 aipkgs_core-1.0.8/aipkgs_core/utils/__pycache__/utils.cpython-38.pyc
--rw-r--r--   0        0        0      167 2022-09-03 21:08:25.855049 aipkgs_core-1.0.8/aipkgs_core/utils/__pycache__/utils.cpython-39.pyc
--rw-r--r--   0        0        0     2196 2022-04-01 17:48:43.916256 aipkgs_core-1.0.8/aipkgs_core/utils/date_helpers.py
--rw-r--r--   0        0        0     1315 2022-03-11 08:48:14.567742 aipkgs_core-1.0.8/aipkgs_core/utils/dir_helpers.py
--rw-r--r--   0        0        0     1084 2024-05-14 10:16:31.693520 aipkgs_core-1.0.8/aipkgs_core/utils/email.py
--rw-r--r--   0        0        0      700 2022-03-08 13:06:48.925633 aipkgs_core-1.0.8/aipkgs_core/utils/file_helpers.py
--rw-r--r--   0        0        0      827 2022-03-08 13:06:48.925703 aipkgs_core-1.0.8/aipkgs_core/utils/json.py
--rw-r--r--   0        0        0      304 2022-03-08 13:06:48.926210 aipkgs_core-1.0.8/aipkgs_core/utils/phone_number.py
--rw-r--r--   0        0        0     1542 2022-08-20 15:51:07.521999 aipkgs_core-1.0.8/aipkgs_core/utils/singleton.py
--rw-r--r--   0        0        0     1105 2022-09-03 21:08:23.013667 aipkgs_core-1.0.8/aipkgs_core/utils/string_helpers.py
--rw-r--r--   0        0        0      654 2024-05-09 14:48:47.729452 aipkgs_core-1.0.8/aipkgs_core/utils/utils.py
--rw-r--r--   0        0        0     1040 2024-05-15 23:27:35.548464 aipkgs_core-1.0.8/pyproject.toml
--rw-r--r--   0        0        0      872 1970-01-01 00:00:00.000000 aipkgs_core-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1058 2022-03-08 13:06:48.926815 aipkgs_core-1.0.9/LICENSE.md
+-rw-r--r--   0        0        0        0 2022-03-08 13:06:48.926754 aipkgs_core-1.0.9/README.rst
+-rw-r--r--   0        0        0      519 2022-09-03 21:38:40.961067 aipkgs_core-1.0.9/aipkgs_core/__init__.py
+-rw-r--r--   0        0        0      708 2024-05-15 23:27:14.638083 aipkgs_core-1.0.9/aipkgs_core/decorators/helpers.py
+-rw-r--r--   0        0        0      620 2022-04-01 17:46:38.417317 aipkgs_core-1.0.9/aipkgs_core/encryption/__pycache__/encryption.cpython-38.pyc
+-rw-r--r--   0        0        0      621 2022-09-03 21:08:25.855962 aipkgs_core-1.0.9/aipkgs_core/encryption/__pycache__/encryption.cpython-39.pyc
+-rw-r--r--   0        0        0     1070 2022-03-08 13:06:48.926158 aipkgs_core-1.0.9/aipkgs_core/encryption/encryption.py
+-rw-r--r--   0        0        0     3145 2024-05-15 21:50:25.991984 aipkgs_core-1.0.9/aipkgs_core/jwt/helpers.py
+-rw-r--r--   0        0        0      857 2024-05-15 21:41:48.931415 aipkgs_core-1.0.9/aipkgs_core/jwt/model.py
+-rw-r--r--   0        0        0      408 2023-10-29 22:52:51.609411 aipkgs_core-1.0.9/aipkgs_core/logger/helpers.py
+-rw-r--r--   0        0        0     1864 2024-05-15 21:54:07.642852 aipkgs_core-1.0.9/aipkgs_core/responses/error.py
+-rw-r--r--   0        0        0     1418 2024-05-15 21:52:09.876274 aipkgs_core-1.0.9/aipkgs_core/responses/response.py
+-rw-r--r--   0        0        0     1000 2024-05-15 21:52:27.080619 aipkgs_core-1.0.9/aipkgs_core/responses/success.py
+-rw-r--r--   0        0        0      435 2024-05-15 21:52:21.512199 aipkgs_core-1.0.9/aipkgs_core/responses/verbose.py
+-rw-r--r--   0        0        0     2124 2022-04-01 17:46:38.433739 aipkgs_core-1.0.9/aipkgs_core/utils/__pycache__/date_helpers.cpython-38.pyc
+-rw-r--r--   0        0        0     2161 2022-09-03 21:08:25.861529 aipkgs_core-1.0.9/aipkgs_core/utils/__pycache__/date_helpers.cpython-39.pyc
+-rw-r--r--   0        0        0     1655 2022-04-01 17:46:33.794476 aipkgs_core-1.0.9/aipkgs_core/utils/__pycache__/dir_helpers.cpython-38.pyc
+-rw-r--r--   0        0        0     1654 2022-09-03 21:01:09.128303 aipkgs_core-1.0.9/aipkgs_core/utils/__pycache__/dir_helpers.cpython-39.pyc
+-rw-r--r--   0        0        0      496 2022-04-01 17:46:33.832091 aipkgs_core-1.0.9/aipkgs_core/utils/__pycache__/email.cpython-38.pyc
+-rw-r--r--   0        0        0      495 2022-09-03 21:01:09.190830 aipkgs_core-1.0.9/aipkgs_core/utils/__pycache__/email.cpython-39.pyc
+-rw-r--r--   0        0        0     1298 2022-04-01 17:46:33.756440 aipkgs_core-1.0.9/aipkgs_core/utils/__pycache__/file_helpers.cpython-38.pyc
+-rw-r--r--   0        0        0     1311 2022-09-03 21:01:09.121203 aipkgs_core-1.0.9/aipkgs_core/utils/__pycache__/file_helpers.cpython-39.pyc
+-rw-r--r--   0        0        0      930 2022-04-01 17:46:38.432909 aipkgs_core-1.0.9/aipkgs_core/utils/__pycache__/json.cpython-38.pyc
+-rw-r--r--   0        0        0      931 2022-09-03 21:08:25.860844 aipkgs_core-1.0.9/aipkgs_core/utils/__pycache__/json.cpython-39.pyc
+-rw-r--r--   0        0        0      571 2022-04-01 17:46:38.302196 aipkgs_core-1.0.9/aipkgs_core/utils/__pycache__/phone_number.cpython-38.pyc
+-rw-r--r--   0        0        0      572 2022-09-03 21:01:09.369200 aipkgs_core-1.0.9/aipkgs_core/utils/__pycache__/phone_number.cpython-39.pyc
+-rw-r--r--   0        0        0     1412 2022-04-01 17:46:38.363966 aipkgs_core-1.0.9/aipkgs_core/utils/__pycache__/string_helpers.cpython-38.pyc
+-rw-r--r--   0        0        0     1414 2022-09-03 21:08:25.846360 aipkgs_core-1.0.9/aipkgs_core/utils/__pycache__/string_helpers.cpython-39.pyc
+-rw-r--r--   0        0        0      166 2022-04-01 17:46:38.413690 aipkgs_core-1.0.9/aipkgs_core/utils/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0        0        0      167 2022-09-03 21:08:25.855049 aipkgs_core-1.0.9/aipkgs_core/utils/__pycache__/utils.cpython-39.pyc
+-rw-r--r--   0        0        0     2196 2022-04-01 17:48:43.916256 aipkgs_core-1.0.9/aipkgs_core/utils/date_helpers.py
+-rw-r--r--   0        0        0     1315 2022-03-11 08:48:14.567742 aipkgs_core-1.0.9/aipkgs_core/utils/dir_helpers.py
+-rw-r--r--   0        0        0     1084 2024-05-14 10:16:31.693520 aipkgs_core-1.0.9/aipkgs_core/utils/email.py
+-rw-r--r--   0        0        0      700 2022-03-08 13:06:48.925633 aipkgs_core-1.0.9/aipkgs_core/utils/file_helpers.py
+-rw-r--r--   0        0        0      827 2022-03-08 13:06:48.925703 aipkgs_core-1.0.9/aipkgs_core/utils/json.py
+-rw-r--r--   0        0        0      304 2022-03-08 13:06:48.926210 aipkgs_core-1.0.9/aipkgs_core/utils/phone_number.py
+-rw-r--r--   0        0        0     1542 2022-08-20 15:51:07.521999 aipkgs_core-1.0.9/aipkgs_core/utils/singleton.py
+-rw-r--r--   0        0        0     1105 2022-09-03 21:08:23.013667 aipkgs_core-1.0.9/aipkgs_core/utils/string_helpers.py
+-rw-r--r--   0        0        0      819 2024-05-16 08:59:04.801572 aipkgs_core-1.0.9/aipkgs_core/utils/utils.py
+-rw-r--r--   0        0        0     1040 2024-05-16 08:59:20.868689 aipkgs_core-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0      872 1970-01-01 00:00:00.000000 aipkgs_core-1.0.9/PKG-INFO
```

### Comparing `aipkgs_core-1.0.8/LICENSE.md` & `aipkgs_core-1.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aipkgs_core-1.0.8/aipkgs_core/__init__.py` & `aipkgs_core-1.0.9/aipkgs_core/__init__.py`

 * *Files identical despite different names*

### Comparing `aipkgs_core-1.0.8/aipkgs_core/decorators/helpers.py` & `aipkgs_core-1.0.9/aipkgs_core/decorators/helpers.py`

 * *Files identical despite different names*

### Comparing `aipkgs_core-1.0.8/aipkgs_core/encryption/__pycache__/encryption.cpython-38.pyc` & `aipkgs_core-1.0.9/aipkgs_core/encryption/__pycache__/encryption.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-1.0.8/aipkgs_core/encryption/__pycache__/encryption.cpython-39.pyc` & `aipkgs_core-1.0.9/aipkgs_core/encryption/__pycache__/encryption.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-1.0.8/aipkgs_core/encryption/encryption.py` & `aipkgs_core-1.0.9/aipkgs_core/encryption/encryption.py`

 * *Files identical despite different names*

### Comparing `aipkgs_core-1.0.8/aipkgs_core/jwt/helpers.py` & `aipkgs_core-1.0.9/aipkgs_core/jwt/helpers.py`

 * *Files identical despite different names*

### Comparing `aipkgs_core-1.0.8/aipkgs_core/jwt/model.py` & `aipkgs_core-1.0.9/aipkgs_core/jwt/model.py`

 * *Files identical despite different names*

### Comparing `aipkgs_core-1.0.8/aipkgs_core/responses/error.py` & `aipkgs_core-1.0.9/aipkgs_core/responses/error.py`

 * *Files identical despite different names*

### Comparing `aipkgs_core-1.0.8/aipkgs_core/responses/response.py` & `aipkgs_core-1.0.9/aipkgs_core/responses/response.py`

 * *Files identical despite different names*

### Comparing `aipkgs_core-1.0.8/aipkgs_core/responses/success.py` & `aipkgs_core-1.0.9/aipkgs_core/responses/success.py`

 * *Files identical despite different names*

### Comparing `aipkgs_core-1.0.8/aipkgs_core/utils/__pycache__/date_helpers.cpython-38.pyc` & `aipkgs_core-1.0.9/aipkgs_core/utils/__pycache__/date_helpers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-1.0.8/aipkgs_core/utils/__pycache__/date_helpers.cpython-39.pyc` & `aipkgs_core-1.0.9/aipkgs_core/utils/__pycache__/date_helpers.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-1.0.8/aipkgs_core/utils/__pycache__/dir_helpers.cpython-38.pyc` & `aipkgs_core-1.0.9/aipkgs_core/utils/__pycache__/dir_helpers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-1.0.8/aipkgs_core/utils/__pycache__/dir_helpers.cpython-39.pyc` & `aipkgs_core-1.0.9/aipkgs_core/utils/__pycache__/dir_helpers.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-1.0.8/aipkgs_core/utils/__pycache__/file_helpers.cpython-38.pyc` & `aipkgs_core-1.0.9/aipkgs_core/utils/__pycache__/file_helpers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-1.0.8/aipkgs_core/utils/__pycache__/file_helpers.cpython-39.pyc` & `aipkgs_core-1.0.9/aipkgs_core/utils/__pycache__/file_helpers.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-1.0.8/aipkgs_core/utils/__pycache__/json.cpython-38.pyc` & `aipkgs_core-1.0.9/aipkgs_core/utils/__pycache__/json.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-1.0.8/aipkgs_core/utils/__pycache__/json.cpython-39.pyc` & `aipkgs_core-1.0.9/aipkgs_core/utils/__pycache__/json.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-1.0.8/aipkgs_core/utils/__pycache__/phone_number.cpython-38.pyc` & `aipkgs_core-1.0.9/aipkgs_core/utils/__pycache__/phone_number.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-1.0.8/aipkgs_core/utils/__pycache__/phone_number.cpython-39.pyc` & `aipkgs_core-1.0.9/aipkgs_core/utils/__pycache__/phone_number.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-1.0.8/aipkgs_core/utils/__pycache__/string_helpers.cpython-38.pyc` & `aipkgs_core-1.0.9/aipkgs_core/utils/__pycache__/string_helpers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-1.0.8/aipkgs_core/utils/__pycache__/string_helpers.cpython-39.pyc` & `aipkgs_core-1.0.9/aipkgs_core/utils/__pycache__/string_helpers.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-1.0.8/aipkgs_core/utils/date_helpers.py` & `aipkgs_core-1.0.9/aipkgs_core/utils/date_helpers.py`

 * *Files identical despite different names*

### Comparing `aipkgs_core-1.0.8/aipkgs_core/utils/dir_helpers.py` & `aipkgs_core-1.0.9/aipkgs_core/utils/dir_helpers.py`

 * *Files identical despite different names*

### Comparing `aipkgs_core-1.0.8/aipkgs_core/utils/email.py` & `aipkgs_core-1.0.9/aipkgs_core/utils/email.py`

 * *Files identical despite different names*

### Comparing `aipkgs_core-1.0.8/aipkgs_core/utils/file_helpers.py` & `aipkgs_core-1.0.9/aipkgs_core/utils/file_helpers.py`

 * *Files identical despite different names*

### Comparing `aipkgs_core-1.0.8/aipkgs_core/utils/json.py` & `aipkgs_core-1.0.9/aipkgs_core/utils/json.py`

 * *Files identical despite different names*

### Comparing `aipkgs_core-1.0.8/aipkgs_core/utils/singleton.py` & `aipkgs_core-1.0.9/aipkgs_core/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `aipkgs_core-1.0.8/aipkgs_core/utils/string_helpers.py` & `aipkgs_core-1.0.9/aipkgs_core/utils/string_helpers.py`

 * *Files identical despite different names*

### Comparing `aipkgs_core-1.0.8/aipkgs_core/utils/utils.py` & `aipkgs_core-1.0.9/aipkgs_core/utils/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,8 +15,16 @@
 
     # Return the hashed password as a utf-8 encoded string
     return PasswordHash(hashed_password.decode('utf-8'), salt.decode('utf-8'))
 
 
 def check_password(password: str, hashed_password: str) -> bool:
     # Check if the provided password matches the hashed password
-    return bcrypt.checkpw(password.encode('utf-8'), hashed_password.encode('utf-8'))
+    return bcrypt.checkpw(password.encode('utf-8'), hashed_password.encode('utf-8'))
+
+
+def remove_extra_spaces(s: str) -> str:
+    return ' '.join(s.split())
+
+
+def remove_substring(s: str, substring: str) -> str:
+    return s.replace(substring, '')
```

### Comparing `aipkgs_core-1.0.8/pyproject.toml` & `aipkgs_core-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["poetry-core>=1.0.8"]
+requires = ["poetry-core>=1.0.9"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "aipkgs-core"
-version = "1.0.8"
+version = "1.0.9"
 description = "Core package for aipy packages."
 authors = ["Alexy <alexy.ib@outlook.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://gitlab.com/aipy/public/packages.git"
 repository = "https://gitlab.com/aipy/public/packages.git"
 keywords = ["ai"]
```

### Comparing `aipkgs_core-1.0.8/PKG-INFO` & `aipkgs_core-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aipkgs-core
-Version: 1.0.8
+Version: 1.0.9
 Summary: Core package for aipy packages.
 Home-page: https://gitlab.com/aipy/public/packages.git
 License: MIT
 Keywords: ai
 Author: Alexy
 Author-email: alexy.ib@outlook.com
 Requires-Python: >=3.11.4,<4.0.0
```

