# Comparing `tmp/nothingpy-0.1.tar.gz` & `tmp/nothingpy-0.1.1.tar.gz`

## Comparing `nothingpy-0.1.tar` & `nothingpy-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 nothingpy-0.1/.idea/.gitignore
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 nothingpy-0.1/.idea/misc.xml
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 nothingpy-0.1/.idea/modules.xml
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 nothingpy-0.1/.idea/nothingpy.iml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nothingpy-0.1/.idea/vcs.xml
--rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 nothingpy-0.1/.idea/workspace.xml
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 nothingpy-0.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 nothingpy-0.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 nothingpy-0.1/research/test_code.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nothingpy-0.1/src/__init__.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 nothingpy-0.1/src/nothingpy/__init__.py
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 nothingpy-0.1/src/nothingpy/nothing.py
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 nothingpy-0.1/tests/test_nothing.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 nothingpy-0.1/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 nothingpy-0.1/LICENSE
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 nothingpy-0.1/README.md
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 nothingpy-0.1/pyproject.toml
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 nothingpy-0.1/PKG-INFO
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 nothingpy-0.1.1/.idea/.gitignore
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 nothingpy-0.1.1/.idea/misc.xml
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 nothingpy-0.1.1/.idea/modules.xml
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 nothingpy-0.1.1/.idea/nothingpy.iml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nothingpy-0.1.1/.idea/vcs.xml
+-rw-r--r--   0        0        0     3847 2020-02-02 00:00:00.000000 nothingpy-0.1.1/.idea/workspace.xml
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 nothingpy-0.1.1/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 nothingpy-0.1.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 nothingpy-0.1.1/research/test_code.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nothingpy-0.1.1/src/__init__.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 nothingpy-0.1.1/src/nothingpy/__init__.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 nothingpy-0.1.1/src/nothingpy/nothing.py
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 nothingpy-0.1.1/tests/test_nothing.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 nothingpy-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 nothingpy-0.1.1/LICENSE
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 nothingpy-0.1.1/README.md
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 nothingpy-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 nothingpy-0.1.1/PKG-INFO
```

### Comparing `nothingpy-0.1/.idea/inspectionProfiles/Project_Default.xml` & `nothingpy-0.1.1/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `nothingpy-0.1/research/test_code.py` & `nothingpy-0.1.1/research/test_code.py`

 * *Files identical despite different names*

### Comparing `nothingpy-0.1/src/nothingpy/__init__.py` & `nothingpy-0.1.1/src/nothingpy/__init__.py`

 * *Files identical despite different names*

### Comparing `nothingpy-0.1/src/nothingpy/nothing.py` & `nothingpy-0.1.1/src/nothingpy/nothing.py`

 * *Files identical despite different names*

### Comparing `nothingpy-0.1/tests/test_nothing.py` & `nothingpy-0.1.1/tests/test_nothing.py`

 * *Files identical despite different names*

### Comparing `nothingpy-0.1/.gitignore` & `nothingpy-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `nothingpy-0.1/LICENSE` & `nothingpy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nothingpy-0.1/pyproject.toml` & `nothingpy-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "nothingpy"
-version = "0.1"
+version = "0.1.1"
 authors = [
   { name="Tom Burns", email="public@llmonpy.ai" },
 ]
 description = "A None alternative for Python that reduces the need for None checks."
 readme = "README.md"
 requires-python = ">=3.4"
 classifiers = [
```

