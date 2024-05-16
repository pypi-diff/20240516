# Comparing `tmp/luke_roberts_cloud_api-0.0.4.tar.gz` & `tmp/luke_roberts_cloud_api-0.0.5.tar.gz`

## Comparing `luke_roberts_cloud_api-0.0.4.tar` & `luke_roberts_cloud_api-0.0.5.tar`

### file list

```diff
@@ -1,7 +1,12 @@
--rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.4/src/luke_roberts_cloud_api/lrcloud.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.4/tests/main.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.4/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.4/LICENSE
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.4/README.md
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.5/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.5/src/luke_roberts_cloud_api/__init__.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.5/src/luke_roberts_cloud_api/const.py
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.5/src/luke_roberts_cloud_api/lamp.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.5/src/luke_roberts_cloud_api/luke_roberts_cloud.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.5/tests/main.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.5/LICENSE
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.5/README.md
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.5/PKG-INFO
```

### Comparing `luke_roberts_cloud_api-0.0.4/LICENSE` & `luke_roberts_cloud_api-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `luke_roberts_cloud_api-0.0.4/README.md` & `luke_roberts_cloud_api-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `luke_roberts_cloud_api-0.0.4/pyproject.toml` & `luke_roberts_cloud_api-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["requests", "hatchling"]
 build-backend = "hatchling.build"#
 
 [project]
 name = "luke_roberts_cloud_api"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Julian Lenzenweger", email="j.lenzenweger@gmail.com" },
 ]
 description = "Exposes the API of the Luke Roberts cloud via utility classes. Luke Roberts is a Lighting Manufacturer."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `luke_roberts_cloud_api-0.0.4/PKG-INFO` & `luke_roberts_cloud_api-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: luke_roberts_cloud_api
-Version: 0.0.4
+Version: 0.0.5
 Summary: Exposes the API of the Luke Roberts cloud via utility classes. Luke Roberts is a Lighting Manufacturer.
 Project-URL: Homepage, https://github.com/julian-lenz/Luke-Roberts-Cloud-API/tree/main
 Project-URL: Issues, https://github.com/julian-lenz/Luke-Roberts-Cloud-API/issues
 Author-email: Julian Lenzenweger <j.lenzenweger@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

