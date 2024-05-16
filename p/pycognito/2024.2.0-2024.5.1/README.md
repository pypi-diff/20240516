# Comparing `tmp/pycognito-2024.2.0.tar.gz` & `tmp/pycognito-2024.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycognito-2024.2.0.tar", last modified: Wed Feb 14 12:58:15 2024, max compression
+gzip compressed data, was "pycognito-2024.5.1.tar", last modified: Thu May 16 09:59:40 2024, max compression
```

## Comparing `pycognito-2024.2.0.tar` & `pycognito-2024.5.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 12:58:15.598676 pycognito-2024.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-14 12:58:04.000000 pycognito-2024.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    24943 2024-02-14 12:58:15.598676 pycognito-2024.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23982 2024-02-14 12:58:04.000000 pycognito-2024.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 12:58:15.594676 pycognito-2024.2.0/pycognito/
--rw-r--r--   0 runner    (1001) docker     (127)    37837 2024-02-14 12:58:04.000000 pycognito-2024.2.0/pycognito/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21354 2024-02-14 12:58:04.000000 pycognito-2024.2.0/pycognito/aws_srp.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-02-14 12:58:04.000000 pycognito-2024.2.0/pycognito/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-02-14 12:58:04.000000 pycognito-2024.2.0/pycognito/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 12:58:15.598676 pycognito-2024.2.0/pycognito.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    24943 2024-02-14 12:58:15.000000 pycognito-2024.2.0/pycognito.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-02-14 12:58:15.000000 pycognito-2024.2.0/pycognito.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 12:58:15.000000 pycognito-2024.2.0/pycognito.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-14 12:58:15.000000 pycognito-2024.2.0/pycognito.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-14 12:58:15.000000 pycognito-2024.2.0/pycognito.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 12:58:15.000000 pycognito-2024.2.0/pycognito.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-02-14 12:58:15.598676 pycognito-2024.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-02-14 12:58:04.000000 pycognito-2024.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:59:40.297475 pycognito-2024.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-16 09:59:33.000000 pycognito-2024.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    24981 2024-05-16 09:59:40.297475 pycognito-2024.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    23997 2024-05-16 09:59:33.000000 pycognito-2024.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:59:40.297475 pycognito-2024.5.1/pycognito/
+-rw-r--r--   0 runner    (1001) docker     (127)    38166 2024-05-16 09:59:33.000000 pycognito-2024.5.1/pycognito/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21355 2024-05-16 09:59:33.000000 pycognito-2024.5.1/pycognito/aws_srp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-16 09:59:33.000000 pycognito-2024.5.1/pycognito/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-16 09:59:33.000000 pycognito-2024.5.1/pycognito/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:59:40.297475 pycognito-2024.5.1/pycognito.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    24981 2024-05-16 09:59:40.000000 pycognito-2024.5.1/pycognito.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-16 09:59:40.000000 pycognito-2024.5.1/pycognito.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 09:59:40.000000 pycognito-2024.5.1/pycognito.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-16 09:59:40.000000 pycognito-2024.5.1/pycognito.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-16 09:59:40.000000 pycognito-2024.5.1/pycognito.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 09:59:40.000000 pycognito-2024.5.1/pycognito.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-16 09:59:40.297475 pycognito-2024.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-16 09:59:33.000000 pycognito-2024.5.1/setup.py
```

### Comparing `pycognito-2024.2.0/LICENSE` & `pycognito-2024.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pycognito-2024.2.0/PKG-INFO` & `pycognito-2024.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: pycognito
-Version: 2024.2.0
+Version: 2024.5.1
 Summary: Python class to integrate Boto3's Cognito client so it is easy to login users. With SRP support.
 Home-page: https://github.com/pvizeli/pycognito
-Download-URL: https://github.com/pvizeli/pycognito/tarball/2024.2.0
+Download-URL: https://github.com/pvizeli/pycognito/tarball/2024.5.1
 Author: Pascal Vizeli
 Author-email: pvizeli@syshack.ch
 License: Apache License 2.0
 Keywords: aws,cognito,api,gateway,serverless
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Environment :: Web Environment
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: boto3>=1.10.49
 Requires-Dist: envs>=1.3
 Requires-Dist: pyjwt[crypto]>=2.8.0
 Requires-Dist: requests>=2.22.0
 
@@ -65,17 +66,19 @@
   - [Updating Device Status](#updating-device-status)
   - [Authenticating your Device](#authenticating-your-device)
   - [Forget Device](#forget-device)
 - [SRP Requests Authenticator](#srp-requests-authenticator)
 
 ## Python Versions Supported
 
-- 3.6
-- 3.7
 - 3.8
+- 3.9
+- 3.10
+- 3.11
+- 3.12
 
 ## Install
 
 `pip install pycognito`
 
 ## Environment Variables
```

### Comparing `pycognito-2024.2.0/README.md` & `pycognito-2024.5.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -41,17 +41,19 @@
   - [Updating Device Status](#updating-device-status)
   - [Authenticating your Device](#authenticating-your-device)
   - [Forget Device](#forget-device)
 - [SRP Requests Authenticator](#srp-requests-authenticator)
 
 ## Python Versions Supported
 
-- 3.6
-- 3.7
 - 3.8
+- 3.9
+- 3.10
+- 3.11
+- 3.12
 
 ## Install
 
 `pip install pycognito`
 
 ## Environment Variables
```

### Comparing `pycognito-2024.2.0/pycognito/__init__.py` & `pycognito-2024.5.1/pycognito/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,28 +256,37 @@
                 token,
                 hmac_key,
                 algorithms=["RS256"],
                 audience=self.client_id if token_use != "access" else None,
                 issuer=self.user_pool_url,
                 options={
                     "require": required_claims,
+                    "verify_iat": False,
                 },
             )
         except jwt.PyJWTError as err:
             raise TokenVerificationException(
                 f"Your {id_name!r} token could not be verified ({err})."
             ) from None
         verified, header = decoded["payload"], decoded["header"]
 
         token_use_verified = verified.get("token_use") == token_use
         if not token_use_verified:
             raise TokenVerificationException(
                 f"Your {id_name!r} token use ({token_use!r}) could not be verified."
             )
 
+        if (iat := verified.get("iat")) is not None:
+            try:
+                int(iat)
+            except ValueError as execption:
+                raise TokenVerificationException(
+                    f"Your {id_name!r} token's iat claim is not a valid integer."
+                ) from execption
+
         # Compute and verify at_hash (formerly done by python-jose)
         if "at_hash" in verified:
             alg_obj = jwt.get_algorithm_by_name(header["alg"])
             digest = alg_obj.compute_hash_digest(self.access_token)
             at_hash = base64.urlsafe_b64encode(digest[: (len(digest) // 2)]).rstrip("=")
             if at_hash != verified["at_hash"]:
                 raise TokenVerificationException(
@@ -487,16 +496,16 @@
             client_secret=self.client_secret,
         )
         try:
             tokens = aws.authenticate_user(client_metadata=client_metadata)
         except MFAChallengeException as mfa_challenge:
             self.mfa_tokens = mfa_challenge.get_tokens()
             raise mfa_challenge
-        else:
-            self._set_tokens(tokens)
+
+        self._set_tokens(tokens)
 
     def new_password_challenge(self, password, new_password):
         """
         Respond to the new password challenge using the SRP protocol
         :param password: The user's current passsword
         :param password: The user's new passsword
         """
```

### Comparing `pycognito-2024.2.0/pycognito/aws_srp.py` & `pycognito-2024.5.1/pycognito/aws_srp.py`

 * *Files 1% similar despite different names*

```diff
@@ -395,15 +395,15 @@
             challenge_response = self.process_challenge(
                 response["ChallengeParameters"], auth_params
             )
             tokens = boto_client.respond_to_auth_challenge(
                 ClientId=self.client_id,
                 ChallengeName=self.PASSWORD_VERIFIER_CHALLENGE,
                 ChallengeResponses=challenge_response,
-                **dict(ClientMetadata=client_metadata) if client_metadata else {},
+                **({"ClientMetadata": client_metadata} if client_metadata else {}),
             )
             if tokens.get("ChallengeName") == self.DEVICE_SRP_CHALLENGE:
                 challenge_response = {
                     "USERNAME": self.username,
                     "DEVICE_KEY": self.device_key,
                     "SRP_A": long_to_hex(self.large_a_value),
                 }
```

### Comparing `pycognito-2024.2.0/pycognito/exceptions.py` & `pycognito-2024.5.1/pycognito/exceptions.py`

 * *Files identical despite different names*

### Comparing `pycognito-2024.2.0/pycognito/utils.py` & `pycognito-2024.5.1/pycognito/utils.py`

 * *Files identical despite different names*

### Comparing `pycognito-2024.2.0/pycognito.egg-info/PKG-INFO` & `pycognito-2024.5.1/pycognito.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: pycognito
-Version: 2024.2.0
+Version: 2024.5.1
 Summary: Python class to integrate Boto3's Cognito client so it is easy to login users. With SRP support.
 Home-page: https://github.com/pvizeli/pycognito
-Download-URL: https://github.com/pvizeli/pycognito/tarball/2024.2.0
+Download-URL: https://github.com/pvizeli/pycognito/tarball/2024.5.1
 Author: Pascal Vizeli
 Author-email: pvizeli@syshack.ch
 License: Apache License 2.0
 Keywords: aws,cognito,api,gateway,serverless
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Environment :: Web Environment
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: boto3>=1.10.49
 Requires-Dist: envs>=1.3
 Requires-Dist: pyjwt[crypto]>=2.8.0
 Requires-Dist: requests>=2.22.0
 
@@ -65,17 +66,19 @@
   - [Updating Device Status](#updating-device-status)
   - [Authenticating your Device](#authenticating-your-device)
   - [Forget Device](#forget-device)
 - [SRP Requests Authenticator](#srp-requests-authenticator)
 
 ## Python Versions Supported
 
-- 3.6
-- 3.7
 - 3.8
+- 3.9
+- 3.10
+- 3.11
+- 3.12
 
 ## Install
 
 `pip install pycognito`
 
 ## Environment Variables
```

### Comparing `pycognito-2024.2.0/setup.py` & `pycognito-2024.5.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 
 from setuptools import setup, find_packages
 
-VERSION = "2024.2.0"
+VERSION = "2024.5.1"
 
 setup(
     name="pycognito",
     version=VERSION,
     description="Python class to integrate Boto3's Cognito client so it is easy to login users. With SRP support.",
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
@@ -29,9 +29,10 @@
     install_requires=[
         "boto3>=1.10.49",
         "envs>=1.3",
         "pyjwt[crypto]>=2.8.0",
         "requests>=2.22.0",
     ],
     include_package_data=True,
+    python_requires=">=3.8",
     zip_safe=True,
 )
```

