# Comparing `tmp/luke_roberts_cloud_api-0.0.5.tar.gz` & `tmp/luke_roberts_cloud_api-0.0.6.tar.gz`

## Comparing `luke_roberts_cloud_api-0.0.5.tar` & `luke_roberts_cloud_api-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.5/.github/workflows/python-app.yml
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.5/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.5/src/luke_roberts_cloud_api/__init__.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.5/src/luke_roberts_cloud_api/const.py
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.5/src/luke_roberts_cloud_api/lamp.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.5/src/luke_roberts_cloud_api/luke_roberts_cloud.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.5/tests/main.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.5/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.5/LICENSE
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.5/README.md
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.6/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.6/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.6/src/luke_roberts_cloud_api/__init__.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.6/src/luke_roberts_cloud_api/const.py
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.6/src/luke_roberts_cloud_api/lamp.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.6/src/luke_roberts_cloud_api/luke_roberts_cloud.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.6/tests/main.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.6/LICENSE
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.6/README.md
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.6/PKG-INFO
```

### Comparing `luke_roberts_cloud_api-0.0.5/.github/workflows/python-app.yml` & `luke_roberts_cloud_api-0.0.6/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `luke_roberts_cloud_api-0.0.5/.github/workflows/python-publish.yml` & `luke_roberts_cloud_api-0.0.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `luke_roberts_cloud_api-0.0.5/src/luke_roberts_cloud_api/lamp.py` & `luke_roberts_cloud_api-0.0.6/src/luke_roberts_cloud_api/lamp.py`

 * *Files identical despite different names*

### Comparing `luke_roberts_cloud_api-0.0.5/src/luke_roberts_cloud_api/luke_roberts_cloud.py` & `luke_roberts_cloud_api-0.0.6/src/luke_roberts_cloud_api/luke_roberts_cloud.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,10 +28,11 @@
 
     async def fetch(self):
         self._lamps = []
         url = f"{BASE_URL}/lamps"
         res = req.get(url=url, headers=self._headers, timeout=10).json()
         for light in res:
             self._lamps.append(Lamp(light, self._headers))
+        return self._lamps
 
     def get_lamps(self):
         return self._lamps
```

### Comparing `luke_roberts_cloud_api-0.0.5/LICENSE` & `luke_roberts_cloud_api-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `luke_roberts_cloud_api-0.0.5/pyproject.toml` & `luke_roberts_cloud_api-0.0.6/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 [build-system]
 requires = ["requests", "hatchling"]
 build-backend = "hatchling.build"#
 
 [project]
 name = "luke_roberts_cloud_api"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Julian Lenzenweger", email="j.lenzenweger@gmail.com" },
 ]
 description = "Exposes the API of the Luke Roberts cloud via utility classes. Luke Roberts is a Lighting Manufacturer."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-
+dependencies = [
+    "requests",
+]
 [tool.hatch.build.targets.wheel]
 packages = ["src/luke_roberts_cloud_api"]
 
 
 [project.urls]
 Homepage = "https://github.com/julian-lenz/Luke-Roberts-Cloud-API/tree/main"
 Issues = "https://github.com/julian-lenz/Luke-Roberts-Cloud-API/issues"
```

### Comparing `luke_roberts_cloud_api-0.0.5/PKG-INFO` & `luke_roberts_cloud_api-0.0.6/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.3
 Name: luke_roberts_cloud_api
-Version: 0.0.5
+Version: 0.0.6
 Summary: Exposes the API of the Luke Roberts cloud via utility classes. Luke Roberts is a Lighting Manufacturer.
 Project-URL: Homepage, https://github.com/julian-lenz/Luke-Roberts-Cloud-API/tree/main
 Project-URL: Issues, https://github.com/julian-lenz/Luke-Roberts-Cloud-API/issues
 Author-email: Julian Lenzenweger <j.lenzenweger@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
+Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 # Luke Roberts Cloud API
 
 This is a Python library for abstracting the HTTP API of the lamp control for Luke Roberts lamps.
 
 ## Installation
@@ -23,18 +24,19 @@
 ```bash
 pip install luke_roberts_cloud_api
 ```
 
 ## Usage
 
 ```python
-import luke_roberts_cloud_api
+import luke_roberts_cloud_api.luke_roberts_cloud as lr
 
 # setup connection
-c
+lrcloud = lr.LukeRobertsCloud(API_KEY)
+lrcloud.fetch()
 ```
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first
 to discuss what you would like to change.
```

