# Comparing `tmp/taktile_auth-1.1.6.tar.gz` & `tmp/taktile_auth-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taktile_auth-1.1.6.tar", max compression
+gzip compressed data, was "taktile_auth-1.1.7.tar", max compression
```

## Comparing `taktile_auth-1.1.6.tar` & `taktile_auth-1.1.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      689 2024-05-14 14:10:38.207352 taktile_auth-1.1.6/PYPI.md
--rw-r--r--   0        0        0     1045 2024-05-14 14:10:38.207352 taktile_auth-1.1.6/pyproject.toml
--rw-r--r--   0        0        0      633 2024-05-14 14:10:38.207352 taktile_auth-1.1.6/taktile_auth/__init__.py
--rw-r--r--   0        0        0     5353 2024-05-14 14:10:38.207352 taktile_auth-1.1.6/taktile_auth/assets/resources.yaml
--rw-r--r--   0        0        0     5078 2024-05-14 14:10:38.207352 taktile_auth-1.1.6/taktile_auth/assets/roles.yaml
--rw-r--r--   0        0        0    10429 2024-05-14 14:10:38.211352 taktile_auth-1.1.6/taktile_auth/client.py
--rw-r--r--   0        0        0      347 2024-05-14 14:10:38.211352 taktile_auth-1.1.6/taktile_auth/entities/__init__.py
--rw-r--r--   0        0        0     1663 2024-05-14 14:10:38.211352 taktile_auth-1.1.6/taktile_auth/entities/permission.py
--rw-r--r--   0        0        0     2784 2024-05-14 14:10:38.211352 taktile_auth-1.1.6/taktile_auth/entities/resource.py
--rw-r--r--   0        0        0     3601 2024-05-14 14:10:38.211352 taktile_auth-1.1.6/taktile_auth/entities/role.py
--rw-r--r--   0        0        0      449 2024-05-14 14:10:38.211352 taktile_auth-1.1.6/taktile_auth/enums.py
--rw-r--r--   0        0        0      177 2024-05-14 14:10:38.211352 taktile_auth-1.1.6/taktile_auth/exceptions.py
--rw-r--r--   0        0        0      426 2024-05-14 14:10:38.211352 taktile_auth-1.1.6/taktile_auth/parser/__init__.py
--rw-r--r--   0        0        0     1166 2024-05-14 14:10:38.211352 taktile_auth-1.1.6/taktile_auth/parser/utils.py
--rw-r--r--   0        0        0     2288 2024-05-14 14:10:38.211352 taktile_auth-1.1.6/taktile_auth/parser/yaml_parsing.py
--rw-r--r--   0        0        0        0 2024-05-14 14:10:38.211352 taktile_auth-1.1.6/taktile_auth/py.typed
--rw-r--r--   0        0        0        0 2024-05-14 14:10:38.211352 taktile_auth-1.1.6/taktile_auth/schemas/__init__.py
--rw-r--r--   0        0        0      420 2024-05-14 14:10:38.211352 taktile_auth-1.1.6/taktile_auth/schemas/session.py
--rw-r--r--   0        0        0     2108 2024-05-14 14:10:38.211352 taktile_auth-1.1.6/taktile_auth/schemas/token.py
--rw-r--r--   0        0        0     1759 2024-05-14 14:10:38.211352 taktile_auth-1.1.6/taktile_auth/settings.py
--rw-r--r--   0        0        0        0 2024-05-14 14:10:38.211352 taktile_auth-1.1.6/taktile_auth/test_utils/__init__.py
--rw-r--r--   0        0        0      502 2024-05-14 14:10:38.211352 taktile_auth-1.1.6/taktile_auth/test_utils/cache_test_utils.py
--rw-r--r--   0        0        0     5978 2024-05-14 14:10:38.211352 taktile_auth-1.1.6/taktile_auth/test_utils/jwt_test_utils.py
--rw-r--r--   0        0        0        0 2024-05-14 14:10:38.211352 taktile_auth-1.1.6/taktile_auth/utils/__init__.py
--rw-r--r--   0        0        0      429 2024-05-14 14:10:38.211352 taktile_auth-1.1.6/taktile_auth/utils/cache.py
--rw-r--r--   0        0        0     2257 2024-05-14 14:10:38.211352 taktile_auth-1.1.6/taktile_auth/utils/sqlalchemy.py
--rw-r--r--   0        0        0     1568 1970-01-01 00:00:00.000000 taktile_auth-1.1.6/setup.py
--rw-r--r--   0        0        0     1320 1970-01-01 00:00:00.000000 taktile_auth-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0      689 2024-05-16 07:52:13.789559 taktile_auth-1.1.7/PYPI.md
+-rw-r--r--   0        0        0     1045 2024-05-16 07:52:13.789559 taktile_auth-1.1.7/pyproject.toml
+-rw-r--r--   0        0        0      633 2024-05-16 07:52:13.789559 taktile_auth-1.1.7/taktile_auth/__init__.py
+-rw-r--r--   0        0        0     5353 2024-05-16 07:52:13.789559 taktile_auth-1.1.7/taktile_auth/assets/resources.yaml
+-rw-r--r--   0        0        0     4979 2024-05-16 07:52:13.789559 taktile_auth-1.1.7/taktile_auth/assets/roles.yaml
+-rw-r--r--   0        0        0    10429 2024-05-16 07:52:13.789559 taktile_auth-1.1.7/taktile_auth/client.py
+-rw-r--r--   0        0        0      347 2024-05-16 07:52:13.789559 taktile_auth-1.1.7/taktile_auth/entities/__init__.py
+-rw-r--r--   0        0        0     1663 2024-05-16 07:52:13.789559 taktile_auth-1.1.7/taktile_auth/entities/permission.py
+-rw-r--r--   0        0        0     2784 2024-05-16 07:52:13.789559 taktile_auth-1.1.7/taktile_auth/entities/resource.py
+-rw-r--r--   0        0        0     3601 2024-05-16 07:52:13.789559 taktile_auth-1.1.7/taktile_auth/entities/role.py
+-rw-r--r--   0        0        0      449 2024-05-16 07:52:13.789559 taktile_auth-1.1.7/taktile_auth/enums.py
+-rw-r--r--   0        0        0      177 2024-05-16 07:52:13.789559 taktile_auth-1.1.7/taktile_auth/exceptions.py
+-rw-r--r--   0        0        0      426 2024-05-16 07:52:13.789559 taktile_auth-1.1.7/taktile_auth/parser/__init__.py
+-rw-r--r--   0        0        0     1166 2024-05-16 07:52:13.789559 taktile_auth-1.1.7/taktile_auth/parser/utils.py
+-rw-r--r--   0        0        0     2288 2024-05-16 07:52:13.789559 taktile_auth-1.1.7/taktile_auth/parser/yaml_parsing.py
+-rw-r--r--   0        0        0        0 2024-05-16 07:52:13.789559 taktile_auth-1.1.7/taktile_auth/py.typed
+-rw-r--r--   0        0        0        0 2024-05-16 07:52:13.789559 taktile_auth-1.1.7/taktile_auth/schemas/__init__.py
+-rw-r--r--   0        0        0      420 2024-05-16 07:52:13.789559 taktile_auth-1.1.7/taktile_auth/schemas/session.py
+-rw-r--r--   0        0        0     2108 2024-05-16 07:52:13.789559 taktile_auth-1.1.7/taktile_auth/schemas/token.py
+-rw-r--r--   0        0        0     1759 2024-05-16 07:52:13.789559 taktile_auth-1.1.7/taktile_auth/settings.py
+-rw-r--r--   0        0        0        0 2024-05-16 07:52:13.789559 taktile_auth-1.1.7/taktile_auth/test_utils/__init__.py
+-rw-r--r--   0        0        0      502 2024-05-16 07:52:13.789559 taktile_auth-1.1.7/taktile_auth/test_utils/cache_test_utils.py
+-rw-r--r--   0        0        0     5978 2024-05-16 07:52:13.789559 taktile_auth-1.1.7/taktile_auth/test_utils/jwt_test_utils.py
+-rw-r--r--   0        0        0        0 2024-05-16 07:52:13.789559 taktile_auth-1.1.7/taktile_auth/utils/__init__.py
+-rw-r--r--   0        0        0      429 2024-05-16 07:52:13.789559 taktile_auth-1.1.7/taktile_auth/utils/cache.py
+-rw-r--r--   0        0        0     2257 2024-05-16 07:52:13.789559 taktile_auth-1.1.7/taktile_auth/utils/sqlalchemy.py
+-rw-r--r--   0        0        0     1568 1970-01-01 00:00:00.000000 taktile_auth-1.1.7/setup.py
+-rw-r--r--   0        0        0     1320 1970-01-01 00:00:00.000000 taktile_auth-1.1.7/PKG-INFO
```

### Comparing `taktile_auth-1.1.6/PYPI.md` & `taktile_auth-1.1.7/PYPI.md`

 * *Files identical despite different names*

### Comparing `taktile_auth-1.1.6/pyproject.toml` & `taktile_auth-1.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "taktile-auth"
-version = "1.1.6"
+version = "1.1.7"
 description = "Auth Package for Taktile"
 readme = "PYPI.md"
 authors = ["Taktile GmbH <devops@taktile.com>"]
 license = "Apache-2.0"
 include = ["taktile_auth/assets/*"]
 
 [tool.poetry.dependencies]
```

### Comparing `taktile_auth-1.1.6/taktile_auth/__init__.py` & `taktile_auth-1.1.7/taktile_auth/__init__.py`

 * *Files identical despite different names*

### Comparing `taktile_auth-1.1.6/taktile_auth/assets/resources.yaml` & `taktile_auth-1.1.7/taktile_auth/assets/resources.yaml`

 * *Files identical despite different names*

### Comparing `taktile_auth-1.1.6/taktile_auth/assets/roles.yaml` & `taktile_auth-1.1.7/taktile_auth/assets/roles.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -120,16 +120,14 @@
     - r:workspace_decision_history_api/org_id,ws_id
     - d:workspace_decision_history/org_id,ws_id
     - w+d:workspace_api_keys/org_id,ws_id
     - w:workspace_live_job_trigger/org_id,ws_id
     - w:workspace_connection_secret/org_id,ws_id
 api_key_job_admin/org_id,ws_id:
     - r+w+d:workspace_job/org_id,ws_id
-    - w:workspace_live_job_trigger/org_id,ws_id
-    - w:workspace_sandbox_job_trigger/org_id,ws_id
 api_key_sandbox/org_id,ws_id:
     - w+r:workspace_sandbox_endpoint/org_id,ws_id
     - w+d:workspace_connection_resource/org_id,ws_id
     - d_member/org_id
     - ws_viewer/org_id,ws_id
     - r:workspace_connection/org_id,ws_id
     - r+w+d:workspace_connection_tenant/org_id,ws_id
```

### Comparing `taktile_auth-1.1.6/taktile_auth/client.py` & `taktile_auth-1.1.7/taktile_auth/client.py`

 * *Files identical despite different names*

### Comparing `taktile_auth-1.1.6/taktile_auth/entities/permission.py` & `taktile_auth-1.1.7/taktile_auth/entities/permission.py`

 * *Files identical despite different names*

### Comparing `taktile_auth-1.1.6/taktile_auth/entities/resource.py` & `taktile_auth-1.1.7/taktile_auth/entities/resource.py`

 * *Files identical despite different names*

### Comparing `taktile_auth-1.1.6/taktile_auth/entities/role.py` & `taktile_auth-1.1.7/taktile_auth/entities/role.py`

 * *Files identical despite different names*

### Comparing `taktile_auth-1.1.6/taktile_auth/parser/utils.py` & `taktile_auth-1.1.7/taktile_auth/parser/utils.py`

 * *Files identical despite different names*

### Comparing `taktile_auth-1.1.6/taktile_auth/parser/yaml_parsing.py` & `taktile_auth-1.1.7/taktile_auth/parser/yaml_parsing.py`

 * *Files identical despite different names*

### Comparing `taktile_auth-1.1.6/taktile_auth/schemas/token.py` & `taktile_auth-1.1.7/taktile_auth/schemas/token.py`

 * *Files identical despite different names*

### Comparing `taktile_auth-1.1.6/taktile_auth/settings.py` & `taktile_auth-1.1.7/taktile_auth/settings.py`

 * *Files identical despite different names*

### Comparing `taktile_auth-1.1.6/taktile_auth/test_utils/jwt_test_utils.py` & `taktile_auth-1.1.7/taktile_auth/test_utils/jwt_test_utils.py`

 * *Files identical despite different names*

### Comparing `taktile_auth-1.1.6/taktile_auth/utils/sqlalchemy.py` & `taktile_auth-1.1.7/taktile_auth/utils/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `taktile_auth-1.1.6/setup.py` & `taktile_auth-1.1.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'PyYAML>=6.0,<7.0',
  'cryptography>=42.0,<43.0',
  'pydantic<3.0',
  'requests==2.31.0']
 
 setup_kwargs = {
     'name': 'taktile-auth',
-    'version': '1.1.6',
+    'version': '1.1.7',
     'description': 'Auth Package for Taktile',
     'long_description': '# Taktile Auth\n\n[![pypi status](https://img.shields.io/pypi/v/taktile-auth.svg)](https://pypi.python.org/pypi/taktile-auth)\n[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)\n\nThis package is part of the Taktile ecosystem.\n\nTaktile enables data science teams to industrialize, scale, and maintain machine learning models. Our ML development platform makes it easy to create your own end-to-end ML applications:\n\n- Turn models into auto-scaling APIs in a few lines of code\n- Easily add model tests\n- Create and share model explanations through the Taktile UI\n\nFind more information in our [docs](https://docs.taktile.com).\n',
     'author': 'Taktile GmbH',
     'author_email': 'devops@taktile.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `taktile_auth-1.1.6/PKG-INFO` & `taktile_auth-1.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taktile-auth
-Version: 1.1.6
+Version: 1.1.7
 Summary: Auth Package for Taktile
 License: Apache-2.0
 Author: Taktile GmbH
 Author-email: devops@taktile.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

