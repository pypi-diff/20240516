# Comparing `tmp/kt2-0.0.8a0.tar.gz` & `tmp/kt2-0.0.9a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kt2-0.0.8a0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "kt2-0.0.9a0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `kt2-0.0.8a0.tar` & `kt2-0.0.9a0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0        0 2023-10-17 11:36:13.265344 kt2-0.0.8a0/.env
--rw-r--r--   0        0        0      256 2023-11-28 13:07:47.746542 kt2-0.0.8a0/.gitignore
--rw-r--r--   0        0        0      738 2023-11-02 10:30:05.236239 kt2-0.0.8a0/CHANGES.rst
--rw-r--r--   0        0        0        0 2023-10-18 06:36:55.319173 kt2-0.0.8a0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1079 2023-10-17 11:39:54.380776 kt2-0.0.8a0/LICENSE
--rw-r--r--   0        0        0      605 2023-10-23 20:51:59.369489 kt2-0.0.8a0/Makefile
--rw-r--r--   0        0        0     4220 2023-10-24 07:04:15.174826 kt2-0.0.8a0/README.md
--rw-r--r--   0        0        0       47 2023-11-28 14:59:04.709179 kt2-0.0.8a0/kt2/__init__.py
--rw-r--r--   0        0        0     3482 2023-11-01 10:50:37.280928 kt2-0.0.8a0/kt2/cli.py
--rw-r--r--   0        0        0    12700 2023-11-02 10:27:40.992861 kt2-0.0.8a0/kt2/client.py
--rw-r--r--   0        0        0     6200 2023-11-02 10:25:38.172171 kt2-0.0.8a0/kt2/commands.py
--rw-r--r--   0        0        0      284 2023-10-30 21:39:04.650335 kt2-0.0.8a0/kt2/errors.py
--rw-r--r--   0        0        0      466 2023-10-23 14:30:09.279647 kt2-0.0.8a0/kt2/helpers.py
--rw-r--r--   0        0        0     1675 2023-10-24 08:58:44.735982 kt2-0.0.8a0/kt2/jwks.py
--rw-r--r--   0        0        0     1077 2023-10-31 07:59:55.214829 kt2-0.0.8a0/kt2/logging.py
--rw-r--r--   0        0        0    13909 2023-11-28 14:58:56.530295 kt2-0.0.8a0/kt2/models.py
--rw-r--r--   0        0        0     8402 2023-11-01 11:17:51.459235 kt2-0.0.8a0/kt2/oauth.py
--rw-r--r--   0        0        0        0 2023-10-18 11:31:18.761284 kt2-0.0.8a0/kt2/py.typed
--rw-r--r--   0        0        0     1076 2023-10-24 08:34:59.798810 kt2-0.0.8a0/kt2/settings.py
--rw-r--r--   0        0        0      530 2023-10-30 12:23:04.734778 kt2-0.0.8a0/kt2/types.py
--rw-r--r--   0        0        0     3937 2023-11-28 14:31:43.905445 kt2-0.0.8a0/kt2/utils.py
--rw-r--r--   0        0        0     1087 2023-10-31 07:48:07.097437 kt2-0.0.8a0/pyproject.toml
--rw-r--r--   0        0        0       63 2023-10-23 20:49:18.895796 kt2-0.0.8a0/requirements.txt
--rw-r--r--   0        0        0      389 2023-10-23 20:50:59.367898 kt2-0.0.8a0/scripts/README.md
--rwxr-xr-x   0        0        0      160 2023-10-23 20:51:02.819720 kt2-0.0.8a0/scripts/format.sh
--rwxr-xr-x   0        0        0      292 2023-10-23 20:51:19.108041 kt2-0.0.8a0/scripts/lint.sh
--rwxr-xr-x   0        0        0       69 2023-10-23 20:50:53.357610 kt2-0.0.8a0/scripts/release.sh
--rwxr-xr-x   0        0        0      247 2023-10-23 20:50:54.577691 kt2-0.0.8a0/scripts/test-integration.sh
--rw-r--r--   0        0        0        0 2023-10-17 11:36:12.936549 kt2-0.0.8a0/tests/__init__.py
--rw-r--r--   0        0        0     5071 1970-01-01 00:00:00.000000 kt2-0.0.8a0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-10-17 11:36:13.265344 kt2-0.0.9a0/.env
+-rw-r--r--   0        0        0      256 2023-11-28 13:07:47.746542 kt2-0.0.9a0/.gitignore
+-rw-r--r--   0        0        0      738 2023-11-02 10:30:05.236239 kt2-0.0.9a0/CHANGES.rst
+-rw-r--r--   0        0        0        0 2023-10-18 06:36:55.319173 kt2-0.0.9a0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1079 2023-10-17 11:39:54.380776 kt2-0.0.9a0/LICENSE
+-rw-r--r--   0        0        0      627 2023-12-05 09:14:50.736281 kt2-0.0.9a0/Makefile
+-rw-r--r--   0        0        0     4220 2023-10-24 07:04:15.174826 kt2-0.0.9a0/README.md
+-rw-r--r--   0        0        0       47 2023-12-05 09:08:56.324934 kt2-0.0.9a0/kt2/__init__.py
+-rw-r--r--   0        0        0     3482 2023-11-01 10:50:37.280928 kt2-0.0.9a0/kt2/cli.py
+-rw-r--r--   0        0        0    12700 2023-11-02 10:27:40.992861 kt2-0.0.9a0/kt2/client.py
+-rw-r--r--   0        0        0     6200 2023-11-02 10:25:38.172171 kt2-0.0.9a0/kt2/commands.py
+-rw-r--r--   0        0        0      284 2023-10-30 21:39:04.650335 kt2-0.0.9a0/kt2/errors.py
+-rw-r--r--   0        0        0      466 2023-10-23 14:30:09.279647 kt2-0.0.9a0/kt2/helpers.py
+-rw-r--r--   0        0        0     1675 2023-10-24 08:58:44.735982 kt2-0.0.9a0/kt2/jwks.py
+-rw-r--r--   0        0        0     1077 2023-10-31 07:59:55.214829 kt2-0.0.9a0/kt2/logging.py
+-rw-r--r--   0        0        0    13909 2023-11-28 14:58:56.530295 kt2-0.0.9a0/kt2/models.py
+-rw-r--r--   0        0        0     8418 2023-12-05 08:28:18.538060 kt2-0.0.9a0/kt2/oauth.py
+-rw-r--r--   0        0        0        0 2023-10-18 11:31:18.761284 kt2-0.0.9a0/kt2/py.typed
+-rw-r--r--   0        0        0     1076 2023-10-24 08:34:59.798810 kt2-0.0.9a0/kt2/settings.py
+-rw-r--r--   0        0        0      530 2023-10-30 12:23:04.734778 kt2-0.0.9a0/kt2/types.py
+-rw-r--r--   0        0        0     3937 2023-11-28 14:31:43.905445 kt2-0.0.9a0/kt2/utils.py
+-rw-r--r--   0        0        0     1087 2023-10-31 07:48:07.097437 kt2-0.0.9a0/pyproject.toml
+-rw-r--r--   0        0        0       63 2023-10-23 20:49:18.895796 kt2-0.0.9a0/requirements.txt
+-rw-r--r--   0        0        0      389 2023-10-23 20:50:59.367898 kt2-0.0.9a0/scripts/README.md
+-rwxr-xr-x   0        0        0      160 2023-10-23 20:51:02.819720 kt2-0.0.9a0/scripts/format.sh
+-rwxr-xr-x   0        0        0      292 2023-10-23 20:51:19.108041 kt2-0.0.9a0/scripts/lint.sh
+-rwxr-xr-x   0        0        0       69 2023-10-23 20:50:53.357610 kt2-0.0.9a0/scripts/release.sh
+-rwxr-xr-x   0        0        0      247 2023-10-23 20:50:54.577691 kt2-0.0.9a0/scripts/test-integration.sh
+-rw-r--r--   0        0        0        0 2023-10-17 11:36:12.936549 kt2-0.0.9a0/tests/__init__.py
+-rw-r--r--   0        0        0     5071 1970-01-01 00:00:00.000000 kt2-0.0.9a0/PKG-INFO
```

### Comparing `kt2-0.0.8a0/CHANGES.rst` & `kt2-0.0.9a0/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `kt2-0.0.8a0/LICENSE` & `kt2-0.0.9a0/LICENSE`

 * *Files identical despite different names*

### Comparing `kt2-0.0.8a0/Makefile` & `kt2-0.0.9a0/Makefile`

 * *Files 10% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 lint:
 	./scripts/lint.sh
 
 format:
 	./scripts/format.sh
 
 release:
+	rm -f koppeltaal.log
 	./scripts/release.sh
 
 test:
 	./scripts/test-integration.sh
 
 shell:
 	ipython
```

### Comparing `kt2-0.0.8a0/README.md` & `kt2-0.0.9a0/README.md`

 * *Files identical despite different names*

### Comparing `kt2-0.0.8a0/kt2/cli.py` & `kt2-0.0.9a0/kt2/cli.py`

 * *Files identical despite different names*

### Comparing `kt2-0.0.8a0/kt2/client.py` & `kt2-0.0.9a0/kt2/client.py`

 * *Files identical despite different names*

### Comparing `kt2-0.0.8a0/kt2/commands.py` & `kt2-0.0.9a0/kt2/commands.py`

 * *Files identical despite different names*

### Comparing `kt2-0.0.8a0/kt2/jwks.py` & `kt2-0.0.9a0/kt2/jwks.py`

 * *Files identical despite different names*

### Comparing `kt2-0.0.8a0/kt2/logging.py` & `kt2-0.0.9a0/kt2/logging.py`

 * *Files identical despite different names*

### Comparing `kt2-0.0.8a0/kt2/models.py` & `kt2-0.0.9a0/kt2/models.py`

 * *Files identical despite different names*

### Comparing `kt2-0.0.8a0/kt2/oauth.py` & `kt2-0.0.9a0/kt2/oauth.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
     def get_authorization_url(
         self,
         redirect_uri: str,
         iss: str,
         launch: str,
         state: str,
         code_verifier: str,
-        scope: Optional[List[str]] = "launch",
+        scope: Optional[List[str]] = "launch openid fhirUser",
     ) -> str:
         try:
             params = AuthorizeParams(
                 aud=iss,
                 launch=launch,
                 client_id=self.client_id,
                 redirect_uri=redirect_uri,
```

### Comparing `kt2-0.0.8a0/kt2/settings.py` & `kt2-0.0.9a0/kt2/settings.py`

 * *Files identical despite different names*

### Comparing `kt2-0.0.8a0/kt2/types.py` & `kt2-0.0.9a0/kt2/types.py`

 * *Files identical despite different names*

### Comparing `kt2-0.0.8a0/kt2/utils.py` & `kt2-0.0.9a0/kt2/utils.py`

 * *Files identical despite different names*

### Comparing `kt2-0.0.8a0/pyproject.toml` & `kt2-0.0.9a0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kt2-0.0.8a0/PKG-INFO` & `kt2-0.0.9a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kt2
-Version: 0.0.8a0
+Version: 0.0.9a0
 Summary: koppeltaal 
 Author-email: TK <tk@terminalkitten.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: pydantic==1.10.12
 Requires-Dist: click
 Requires-Dist: httpx
```

