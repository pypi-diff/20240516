# Comparing `tmp/xl_database-0.6.3.tar.gz` & `tmp/xl_database-0.6.5.tar.gz`

## Comparing `xl_database-0.6.3.tar` & `xl_database-0.6.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 xl_database-0.6.3/src/xl_database/__init__.py
--rw-r--r--   0        0        0     5480 2020-02-02 00:00:00.000000 xl_database-0.6.3/src/xl_database/mixins.py
--rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 xl_database-0.6.3/src/xl_database/model.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 xl_database-0.6.3/src/xl_database/utils/time.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 xl_database-0.6.3/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 xl_database-0.6.3/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xl_database-0.6.3/README.md
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 xl_database-0.6.3/pyproject.toml
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 xl_database-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 xl_database-0.6.5/src/xl_database/__init__.py
+-rw-r--r--   0        0        0     5480 2020-02-02 00:00:00.000000 xl_database-0.6.5/src/xl_database/mixins.py
+-rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 xl_database-0.6.5/src/xl_database/model.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 xl_database-0.6.5/src/xl_database/utils/time.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 xl_database-0.6.5/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 xl_database-0.6.5/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xl_database-0.6.5/README.md
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 xl_database-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 xl_database-0.6.5/PKG-INFO
```

### Comparing `xl_database-0.6.3/src/xl_database/mixins.py` & `xl_database-0.6.5/src/xl_database/mixins.py`

 * *Files identical despite different names*

### Comparing `xl_database-0.6.3/src/xl_database/model.py` & `xl_database-0.6.5/src/xl_database/model.py`

 * *Files identical despite different names*

### Comparing `xl_database-0.6.3/LICENSE` & `xl_database-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xl_database-0.6.3/pyproject.toml` & `xl_database-0.6.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "xl-database"
-version = "0.6.3"
+version = "0.6.5"
 authors = [
   { name="xilong", email="xilonglab@163.com" },
 ]
 description = "xilong database library"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

