# Comparing `tmp/luke_roberts_cloud_api-0.0.6.tar.gz` & `tmp/luke_roberts_cloud_api-0.0.7.tar.gz`

## Comparing `luke_roberts_cloud_api-0.0.6.tar` & `luke_roberts_cloud_api-0.0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.6/.github/workflows/python-app.yml
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.6/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.6/src/luke_roberts_cloud_api/__init__.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.6/src/luke_roberts_cloud_api/const.py
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.6/src/luke_roberts_cloud_api/lamp.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.6/src/luke_roberts_cloud_api/luke_roberts_cloud.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.6/tests/main.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.6/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.6/LICENSE
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.6/README.md
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.7/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.7/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.7/src/luke_roberts_cloud_api/__init__.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.7/src/luke_roberts_cloud_api/const.py
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.7/src/luke_roberts_cloud_api/lamp.py
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.7/src/luke_roberts_cloud_api/luke_roberts_cloud.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.7/tests/main.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.7/LICENSE
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.7/README.md
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.7/PKG-INFO
```

### Comparing `luke_roberts_cloud_api-0.0.6/.github/workflows/python-app.yml` & `luke_roberts_cloud_api-0.0.7/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `luke_roberts_cloud_api-0.0.6/.github/workflows/python-publish.yml` & `luke_roberts_cloud_api-0.0.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `luke_roberts_cloud_api-0.0.6/src/luke_roberts_cloud_api/lamp.py` & `luke_roberts_cloud_api-0.0.7/src/luke_roberts_cloud_api/lamp.py`

 * *Files identical despite different names*

### Comparing `luke_roberts_cloud_api-0.0.6/src/luke_roberts_cloud_api/luke_roberts_cloud.py` & `luke_roberts_cloud_api-0.0.7/src/luke_roberts_cloud_api/luke_roberts_cloud.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,22 +10,20 @@
 
     _lamps = []
     _api_key: str
     _headers = dict()
 
     def __init__(self, api_key: str = "") -> None:
         self.set_api_key(api_key)
-        if self.test_connection():
-            self.fetch()
 
     def set_api_key(self, api_key: str) -> None:
         self._api_key = api_key
         self._headers['Authorization'] = f"Bearer {api_key}"
 
-    def test_connection(self):
+    async def test_connection(self):
         url = f"{BASE_URL}/lamps"
         res = req.get(url=url, headers=self._headers, timeout=10)
         return res.ok
 
     async def fetch(self):
         self._lamps = []
         url = f"{BASE_URL}/lamps"
```

### Comparing `luke_roberts_cloud_api-0.0.6/LICENSE` & `luke_roberts_cloud_api-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `luke_roberts_cloud_api-0.0.6/README.md` & `luke_roberts_cloud_api-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `luke_roberts_cloud_api-0.0.6/pyproject.toml` & `luke_roberts_cloud_api-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["requests", "hatchling"]
 build-backend = "hatchling.build"#
 
 [project]
 name = "luke_roberts_cloud_api"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Julian Lenzenweger", email="j.lenzenweger@gmail.com" },
 ]
 description = "Exposes the API of the Luke Roberts cloud via utility classes. Luke Roberts is a Lighting Manufacturer."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `luke_roberts_cloud_api-0.0.6/PKG-INFO` & `luke_roberts_cloud_api-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: luke_roberts_cloud_api
-Version: 0.0.6
+Version: 0.0.7
 Summary: Exposes the API of the Luke Roberts cloud via utility classes. Luke Roberts is a Lighting Manufacturer.
 Project-URL: Homepage, https://github.com/julian-lenz/Luke-Roberts-Cloud-API/tree/main
 Project-URL: Issues, https://github.com/julian-lenz/Luke-Roberts-Cloud-API/issues
 Author-email: Julian Lenzenweger <j.lenzenweger@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

