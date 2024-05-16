# Comparing `tmp/xl_database-0.6.5.tar.gz` & `tmp/xl_database-0.6.6.tar.gz`

## Comparing `xl_database-0.6.5.tar` & `xl_database-0.6.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 xl_database-0.6.5/src/xl_database/__init__.py
--rw-r--r--   0        0        0     5480 2020-02-02 00:00:00.000000 xl_database-0.6.5/src/xl_database/mixins.py
--rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 xl_database-0.6.5/src/xl_database/model.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 xl_database-0.6.5/src/xl_database/utils/time.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 xl_database-0.6.5/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 xl_database-0.6.5/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xl_database-0.6.5/README.md
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 xl_database-0.6.5/pyproject.toml
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 xl_database-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 xl_database-0.6.6/src/xl_database/__init__.py
+-rw-r--r--   0        0        0     5480 2020-02-02 00:00:00.000000 xl_database-0.6.6/src/xl_database/mixins.py
+-rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 xl_database-0.6.6/src/xl_database/model.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 xl_database-0.6.6/src/xl_database/utils/time.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 xl_database-0.6.6/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 xl_database-0.6.6/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xl_database-0.6.6/README.md
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 xl_database-0.6.6/pyproject.toml
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 xl_database-0.6.6/PKG-INFO
```

### Comparing `xl_database-0.6.5/src/xl_database/mixins.py` & `xl_database-0.6.6/src/xl_database/mixins.py`

 * *Files identical despite different names*

### Comparing `xl_database-0.6.5/src/xl_database/model.py` & `xl_database-0.6.6/src/xl_database/model.py`

 * *Files identical despite different names*

### Comparing `xl_database-0.6.5/LICENSE` & `xl_database-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xl_database-0.6.5/pyproject.toml` & `xl_database-0.6.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "xl-database"
-version = "0.6.5"
+version = "0.6.6"
 authors = [
   { name="xilong", email="xilonglab@163.com" },
 ]
 description = "xilong database library"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `xl_database-0.6.5/PKG-INFO` & `xl_database-0.6.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xl-database
-Version: 0.6.5
+Version: 0.6.6
 Summary: xilong database library
 Project-URL: Homepage, https://git.xilonglab.com/xilong/zdatabase
 Project-URL: Bug Tracker, https://git.xilonglab.com/xilong/zdatabase/issues
 Author-email: xilong <xilonglab@163.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

