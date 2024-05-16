# Comparing `tmp/flask_shopify_utils-0.1.4.tar.gz` & `tmp/flask_shopify_utils-0.1.5.tar.gz`

## Comparing `flask_shopify_utils-0.1.4.tar` & `flask_shopify_utils-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    34768 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.4/src/flask_shopify_utils/__init__.py
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.4/src/flask_shopify_utils/model.py
--rw-r--r--   0        0        0     4110 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.4/src/flask_shopify_utils/utils.py
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.4/tests/conftest.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.4/tests/test_alpha.py
--rw-r--r--   0        0        0     5250 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.4/tests/test_default_routes.py
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.4/tests/test_gdpr_routes.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.4/tests/test_graphql_cli.py
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.4/tests/test_ui_routes.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.4/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.4/LICENSE
--rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.4/README.md
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    34774 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.5/src/flask_shopify_utils/__init__.py
+-rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.5/src/flask_shopify_utils/model.py
+-rw-r--r--   0        0        0     4110 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.5/src/flask_shopify_utils/utils.py
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.5/tests/conftest.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.5/tests/test_alpha.py
+-rw-r--r--   0        0        0     5250 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.5/tests/test_default_routes.py
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.5/tests/test_gdpr_routes.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.5/tests/test_graphql_cli.py
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.5/tests/test_ui_routes.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.5/README.md
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3871 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.5/PKG-INFO
```

### Comparing `flask_shopify_utils-0.1.4/src/flask_shopify_utils/__init__.py` & `flask_shopify_utils-0.1.5/src/flask_shopify_utils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     make_response, url_for
 from jinja2 import TemplateNotFound
 from jwt import encode as jwt_encode, decode as jwt_decode, ExpiredSignatureError
 from cerberus.validator import Validator
 from pytz import timezone
 from flask_shopify_utils.utils import get_version, GraphQLClient
 
-__version__ = '0.1.4'
+__version__ = '0.1.5'
 
 JWT_DATA = TypeVar('JWT_DATA', dict, Response)
 current_time_func = None
 sqlalchemy_instance = None
 
 
 class ShopifyUtil:
@@ -657,15 +657,15 @@
                 resp = self.proxy_response(500, 'Something went wrong while fetching installation data!')
                 resp.status_code = 500
                 return resp
             record.scopes = ','.join(list(map(lambda x: x['handle'], scopes['accessScopes'])))
             self.db.commit()
             # Register GDPR mandatory webhook @todo
             # https://shopify.dev/docs/apps/auth/get-access-tokens/authorization-code-grant/getting-started
-            return redirect('https://{}/apps/{}'.format(
+            return redirect('https://{}/admin/apps/{}'.format(
                 g.store_key,
                 self.config.get('SHOPIFY_API_KEY'))
             )
 
         # Register the `install` route
         @default_routes.route('/install', methods=['GET'], endpoint='install')
         def install():
```

### Comparing `flask_shopify_utils-0.1.4/src/flask_shopify_utils/model.py` & `flask_shopify_utils-0.1.5/src/flask_shopify_utils/model.py`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.1.4/src/flask_shopify_utils/utils.py` & `flask_shopify_utils-0.1.5/src/flask_shopify_utils/utils.py`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.1.4/tests/conftest.py` & `flask_shopify_utils-0.1.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.1.4/tests/test_alpha.py` & `flask_shopify_utils-0.1.5/tests/test_alpha.py`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.1.4/tests/test_default_routes.py` & `flask_shopify_utils-0.1.5/tests/test_default_routes.py`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.1.4/tests/test_gdpr_routes.py` & `flask_shopify_utils-0.1.5/tests/test_gdpr_routes.py`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.1.4/tests/test_ui_routes.py` & `flask_shopify_utils-0.1.5/tests/test_ui_routes.py`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.1.4/LICENSE` & `flask_shopify_utils-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.1.4/README.md` & `flask_shopify_utils-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.1.4/pyproject.toml` & `flask_shopify_utils-0.1.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     "PyJWT == 2.8.0",
     "simplejson < 4"
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = [
-    "pytest == 8.1.1",
+    "pytest < 9",
     "twine == 5.0.0",
     "build == 1.2.1"
 ]
 
 [tool.pytest.ini_options]
 minversion = "7.0"
 addopts = '-vs'
```

### Comparing `flask_shopify_utils-0.1.4/PKG-INFO` & `flask_shopify_utils-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: flask-shopify-utils
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Flask extension for Shopify app development
 Project-URL: Homepage, https://github.com/leocxy/flask-shopify-utils
 Project-URL: Bug Tracker, https://github.com/leocxy/flask-shopify-utils/issues
 Author: Leo Chen
 Author-email: leo.cxy88@gmail.com
 Maintainer: Leo Chen
 Maintainer-email: leo.cxy88@gmail.com
@@ -25,15 +25,15 @@
 Requires-Dist: pytz==2024.1
 Requires-Dist: requests<3
 Requires-Dist: sgqlc<17
 Requires-Dist: shopifyapi==12.5.0
 Requires-Dist: simplejson<4
 Provides-Extra: dev
 Requires-Dist: build==1.2.1; extra == 'dev'
-Requires-Dist: pytest==8.1.1; extra == 'dev'
+Requires-Dist: pytest<9; extra == 'dev'
 Requires-Dist: twine==5.0.0; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # Flask-Shopify-Utils
 
 The utils for Flask Application that build for Shopify Custom App
```

