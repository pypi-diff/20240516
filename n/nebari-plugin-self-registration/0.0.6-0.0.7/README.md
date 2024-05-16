# Comparing `tmp/nebari_plugin_self_registration-0.0.6.tar.gz` & `tmp/nebari_plugin_self_registration-0.0.7.tar.gz`

## Comparing `nebari_plugin_self_registration-0.0.6.tar` & `nebari_plugin_self_registration-0.0.7.tar`

### file list

```diff
@@ -1,45 +1,50 @@
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.6/.github/workflows/publish-docker-image.yaml
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.6/.github/workflows/publish-pypi.yaml
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.6/docker/.dockerignore
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.6/docker/Dockerfile
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.6/docker/requirements.txt
--rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.6/docker/app/job.py
--rw-r--r--   0        0        0     6060 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.6/docker/app/main.py
--rw-r--r--   0        0        0     8321 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.6/docker/app/static/logo.png
--rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.6/docker/app/static/styles.css
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.6/docker/app/templates/index.html
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.6/docker/app/templates/success.html
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.6/src/nebari_plugin_self_registration/__about__.py
--rw-r--r--   0        0        0     7332 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.6/src/nebari_plugin_self_registration/__init__.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.6/src/nebari_plugin_self_registration/terraform/main.tf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.6/src/nebari_plugin_self_registration/terraform/outputs.tf
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.6/src/nebari_plugin_self_registration/terraform/variables.tf
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.6/src/nebari_plugin_self_registration/terraform/versions.tf
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.6/src/nebari_plugin_self_registration/terraform/modules/keycloak/main.tf
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.6/src/nebari_plugin_self_registration/terraform/modules/keycloak/outputs.tf
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.6/src/nebari_plugin_self_registration/terraform/modules/keycloak/variables.tf
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.6/src/nebari_plugin_self_registration/terraform/modules/keycloak/versions.tf
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.6/src/nebari_plugin_self_registration/terraform/modules/self-registration/main.tf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.6/src/nebari_plugin_self_registration/terraform/modules/self-registration/outputs.tf
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.6/src/nebari_plugin_self_registration/terraform/modules/self-registration/variables.tf
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.6/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/.helmignore
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.6/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/Chart.yaml
--rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.6/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/values.yaml
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.6/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/NOTES.txt
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.6/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/_helpers.tpl
--rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.6/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/deployment.yaml
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.6/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/hpa.yaml
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.6/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/ingress.yaml
--rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.6/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/job.yaml
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.6/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/secret.yaml
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.6/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/service.yaml
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.6/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/serviceaccount.yaml
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.6/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/traefik.yaml
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.6/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/tests/test-connection.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.6/src/nebari_plugin_self_registration/tests/unit/__init__.py
--rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.6/src/nebari_plugin_self_registration/tests/unit/test_plugin.py
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.6/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.6/LICENSE
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.6/README.md
--rw-r--r--   0        0        0     3523 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/.github/workflows/publish-docker-image.yaml
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/.github/workflows/publish-pypi.yaml
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/docker/.dockerignore
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/docker/Dockerfile
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/docker/requirements.txt
+-rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/docker/app/job.py
+-rw-r--r--   0        0        0     6060 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/docker/app/main.py
+-rw-r--r--   0        0        0     8321 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/docker/app/static/logo.png
+-rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/docker/app/static/styles.css
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/docker/app/templates/index.html
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/docker/app/templates/success.html
+-rw-r--r--   0        0        0   203481 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/images/account-confirm.png
+-rw-r--r--   0        0        0   143215 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/images/account-register.png
+-rw-r--r--   0        0        0    97043 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/images/nebari-splash.png
+-rw-r--r--   0        0        0   215778 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/images/verify-email.png
+-rw-r--r--   0        0        0    16370 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/images/welcome-nebari.png
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/__about__.py
+-rw-r--r--   0        0        0     7303 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/__init__.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/main.tf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/outputs.tf
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/variables.tf
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/versions.tf
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/keycloak/main.tf
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/keycloak/outputs.tf
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/keycloak/variables.tf
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/keycloak/versions.tf
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/main.tf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/outputs.tf
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/variables.tf
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/.helmignore
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/Chart.yaml
+-rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/values.yaml
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/NOTES.txt
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/_helpers.tpl
+-rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/deployment.yaml
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/hpa.yaml
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/ingress.yaml
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/job.yaml
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/secret.yaml
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/service.yaml
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/serviceaccount.yaml
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/traefik.yaml
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/tests/test-connection.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/tests/unit/__init__.py
+-rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/tests/unit/test_plugin.py
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/LICENSE
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/README.md
+-rw-r--r--   0        0        0     3523 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/PKG-INFO
```

### Comparing `nebari_plugin_self_registration-0.0.6/.github/workflows/publish-docker-image.yaml` & `nebari_plugin_self_registration-0.0.7/.github/workflows/publish-docker-image.yaml`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.6/.github/workflows/publish-pypi.yaml` & `nebari_plugin_self_registration-0.0.7/.github/workflows/publish-pypi.yaml`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.6/docker/app/job.py` & `nebari_plugin_self_registration-0.0.7/docker/app/job.py`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.6/docker/app/main.py` & `nebari_plugin_self_registration-0.0.7/docker/app/main.py`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.6/docker/app/static/logo.png` & `nebari_plugin_self_registration-0.0.7/docker/app/static/logo.png`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.6/docker/app/static/styles.css` & `nebari_plugin_self_registration-0.0.7/docker/app/static/styles.css`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.6/docker/app/templates/index.html` & `nebari_plugin_self_registration-0.0.7/docker/app/templates/index.html`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.6/docker/app/templates/success.html` & `nebari_plugin_self_registration-0.0.7/docker/app/templates/success.html`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.6/src/nebari_plugin_self_registration/__init__.py` & `nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,19 +75,19 @@
 
         for i in range(num_attempts):
             try:
                 realm_admin = KeycloakAdmin(
                     keycloak_url,
                     username=username,
                     password=password,
-                    realm_name=master_realm_name,
+                    user_realm_name=master_realm_name,
+                    realm_name=client_realm_name,
                     client_id=client_id,
                     verify=verify,
                 )
-                realm_admin.realm_name = client_realm_name # switch to nebari realm
                 c = realm_admin.get_client_id(CLIENT_NAME) # lookup client guid
                 existing_client = realm_admin.get_client(c) # query client info
                 if existing_client != None and existing_client["name"] == CLIENT_NAME:
                     print(
                         f"Attempt {i+1} succeeded connecting to keycloak and nebari client={CLIENT_NAME} exists"
                     )
                     return True
```

### Comparing `nebari_plugin_self_registration-0.0.6/src/nebari_plugin_self_registration/terraform/main.tf` & `nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/main.tf`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.6/src/nebari_plugin_self_registration/terraform/variables.tf` & `nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.6/src/nebari_plugin_self_registration/terraform/modules/keycloak/main.tf` & `nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/keycloak/main.tf`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.6/src/nebari_plugin_self_registration/terraform/modules/self-registration/main.tf` & `nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/main.tf`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.6/src/nebari_plugin_self_registration/terraform/modules/self-registration/variables.tf` & `nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.6/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/Chart.yaml` & `nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/Chart.yaml`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.6/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/values.yaml` & `nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/values.yaml`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.6/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/NOTES.txt` & `nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/NOTES.txt`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.6/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/_helpers.tpl` & `nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.6/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/deployment.yaml` & `nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/deployment.yaml`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.6/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/hpa.yaml` & `nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/hpa.yaml`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.6/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/ingress.yaml` & `nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/ingress.yaml`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.6/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/job.yaml` & `nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/job.yaml`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.6/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/traefik.yaml` & `nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/traefik.yaml`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.6/src/nebari_plugin_self_registration/tests/unit/test_plugin.py` & `nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/tests/unit/test_plugin.py`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.6/.gitignore` & `nebari_plugin_self_registration-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.6/LICENSE` & `nebari_plugin_self_registration-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.6/pyproject.toml` & `nebari_plugin_self_registration-0.0.7/pyproject.toml`

 * *Files identical despite different names*

