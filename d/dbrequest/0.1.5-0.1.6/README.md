# Comparing `tmp/dbrequest-0.1.5.tar.gz` & `tmp/dbrequest-0.1.6.tar.gz`

## Comparing `dbrequest-0.1.5.tar` & `dbrequest-0.1.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 dbrequest-0.1.5/.gitattributes
--rw-r--r--   0        0        0     8017 2020-02-02 00:00:00.000000 dbrequest-0.1.5/README.ru.md
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 dbrequest-0.1.5/example/create_table.sql
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 dbrequest-0.1.5/example/main.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 dbrequest-0.1.5/example/user.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 dbrequest-0.1.5/example/user_fields.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 dbrequest-0.1.5/example/user_request.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 dbrequest-0.1.5/src/dbrequest/__init__.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 dbrequest-0.1.5/src/dbrequest/interfaces.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 dbrequest-0.1.5/src/dbrequest/sql_requests.py
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 dbrequest-0.1.5/src/dbrequest/config/config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbrequest-0.1.5/src/dbrequest/core/__init__.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 dbrequest-0.1.5/src/dbrequest/core/fields.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 dbrequest-0.1.5/src/dbrequest/core/idb_request.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 dbrequest-0.1.5/src/dbrequest/core/interfaces.py
--rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 dbrequest-0.1.5/src/dbrequest/core/requests.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 dbrequest-0.1.5/src/dbrequest/core/savable.py
--rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 dbrequest-0.1.5/src/dbrequest/core/saver_loader.py
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 dbrequest-0.1.5/src/dbrequest/core/type_converters.py
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 dbrequest-0.1.5/src/dbrequest/core/universal_requests.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 dbrequest-0.1.5/src/dbrequest/executors/__init__.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 dbrequest-0.1.5/src/dbrequest/executors/interfaces.py
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 dbrequest-0.1.5/src/dbrequest/executors/sqlite_executor.py
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 dbrequest-0.1.5/src/dbrequest/executors/universal_executor.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 dbrequest-0.1.5/src/dbrequest/sql/__init__.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 dbrequest-0.1.5/src/dbrequest/sql/interfaces.py
--rw-r--r--   0        0        0     4011 2020-02-02 00:00:00.000000 dbrequest-0.1.5/src/dbrequest/sql/properties.py
--rw-r--r--   0        0        0     5617 2020-02-02 00:00:00.000000 dbrequest-0.1.5/src/dbrequest/sql/requests.py
--rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 dbrequest-0.1.5/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 dbrequest-0.1.5/LICENSE
--rw-r--r--   0        0        0     6235 2020-02-02 00:00:00.000000 dbrequest-0.1.5/README.md
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 dbrequest-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     6922 2020-02-02 00:00:00.000000 dbrequest-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 dbrequest-0.1.6/.gitattributes
+-rw-r--r--   0        0        0     8017 2020-02-02 00:00:00.000000 dbrequest-0.1.6/README.ru.md
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 dbrequest-0.1.6/example/create_table.sql
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 dbrequest-0.1.6/example/main.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 dbrequest-0.1.6/example/user.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 dbrequest-0.1.6/example/user_fields.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 dbrequest-0.1.6/example/user_request.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 dbrequest-0.1.6/src/dbrequest/__init__.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 dbrequest-0.1.6/src/dbrequest/interfaces.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 dbrequest-0.1.6/src/dbrequest/sql_requests.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 dbrequest-0.1.6/src/dbrequest/config/config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbrequest-0.1.6/src/dbrequest/core/__init__.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 dbrequest-0.1.6/src/dbrequest/core/fields.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 dbrequest-0.1.6/src/dbrequest/core/idb_request.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 dbrequest-0.1.6/src/dbrequest/core/interfaces.py
+-rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 dbrequest-0.1.6/src/dbrequest/core/requests.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 dbrequest-0.1.6/src/dbrequest/core/savable.py
+-rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 dbrequest-0.1.6/src/dbrequest/core/saver_loader.py
+-rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 dbrequest-0.1.6/src/dbrequest/core/type_converters.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 dbrequest-0.1.6/src/dbrequest/core/universal_requests.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 dbrequest-0.1.6/src/dbrequest/executors/__init__.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 dbrequest-0.1.6/src/dbrequest/executors/interfaces.py
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 dbrequest-0.1.6/src/dbrequest/executors/sqlite_executor.py
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 dbrequest-0.1.6/src/dbrequest/executors/universal_executor.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 dbrequest-0.1.6/src/dbrequest/sql/__init__.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 dbrequest-0.1.6/src/dbrequest/sql/interfaces.py
+-rw-r--r--   0        0        0     4011 2020-02-02 00:00:00.000000 dbrequest-0.1.6/src/dbrequest/sql/properties.py
+-rw-r--r--   0        0        0     5617 2020-02-02 00:00:00.000000 dbrequest-0.1.6/src/dbrequest/sql/requests.py
+-rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 dbrequest-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 dbrequest-0.1.6/LICENSE
+-rw-r--r--   0        0        0     6235 2020-02-02 00:00:00.000000 dbrequest-0.1.6/README.md
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 dbrequest-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     6922 2020-02-02 00:00:00.000000 dbrequest-0.1.6/PKG-INFO
```

### Comparing `dbrequest-0.1.5/README.ru.md` & `dbrequest-0.1.6/README.ru.md`

 * *Files identical despite different names*

### Comparing `dbrequest-0.1.5/example/main.py` & `dbrequest-0.1.6/example/main.py`

 * *Files identical despite different names*

### Comparing `dbrequest-0.1.5/example/user.py` & `dbrequest-0.1.6/example/user.py`

 * *Files identical despite different names*

### Comparing `dbrequest-0.1.5/example/user_fields.py` & `dbrequest-0.1.6/example/user_fields.py`

 * *Files identical despite different names*

### Comparing `dbrequest-0.1.5/src/dbrequest/config/config.py` & `dbrequest-0.1.6/src/dbrequest/config/config.py`

 * *Files identical despite different names*

### Comparing `dbrequest-0.1.5/src/dbrequest/core/fields.py` & `dbrequest-0.1.6/src/dbrequest/core/fields.py`

 * *Files identical despite different names*

### Comparing `dbrequest-0.1.5/src/dbrequest/core/idb_request.py` & `dbrequest-0.1.6/src/dbrequest/core/idb_request.py`

 * *Files identical despite different names*

### Comparing `dbrequest-0.1.5/src/dbrequest/core/interfaces.py` & `dbrequest-0.1.6/src/dbrequest/core/interfaces.py`

 * *Files identical despite different names*

### Comparing `dbrequest-0.1.5/src/dbrequest/core/requests.py` & `dbrequest-0.1.6/src/dbrequest/core/requests.py`

 * *Files identical despite different names*

### Comparing `dbrequest-0.1.5/src/dbrequest/core/saver_loader.py` & `dbrequest-0.1.6/src/dbrequest/core/saver_loader.py`

 * *Files identical despite different names*

### Comparing `dbrequest-0.1.5/src/dbrequest/core/type_converters.py` & `dbrequest-0.1.6/src/dbrequest/core/type_converters.py`

 * *Files 7% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
     def fromDatabase(self, value: int) -> Date:
         if value is not None:
             return Date.fromordinal(value)
 
 class AbstractJsonableDBTypeConverter(AbstractDBTypeConverter):
     def toDatabase(self, value: Any) -> str:
-        return json.dumps(value)
+        return json.dumps(value, ensure_ascii=False, indent=2)
 
     def fromDatabase(self, value: str) -> Any:
         if value is not None:
             return json.loads(value)
         
 class ListDBTypeConverter(AbstractJsonableDBTypeConverter):
     def __init__(self) -> None:
```

### Comparing `dbrequest-0.1.5/src/dbrequest/core/universal_requests.py` & `dbrequest-0.1.6/src/dbrequest/core/universal_requests.py`

 * *Files identical despite different names*

### Comparing `dbrequest-0.1.5/src/dbrequest/executors/sqlite_executor.py` & `dbrequest-0.1.6/src/dbrequest/executors/sqlite_executor.py`

 * *Files identical despite different names*

### Comparing `dbrequest-0.1.5/src/dbrequest/executors/universal_executor.py` & `dbrequest-0.1.6/src/dbrequest/executors/universal_executor.py`

 * *Files identical despite different names*

### Comparing `dbrequest-0.1.5/src/dbrequest/sql/properties.py` & `dbrequest-0.1.6/src/dbrequest/sql/properties.py`

 * *Files identical despite different names*

### Comparing `dbrequest-0.1.5/src/dbrequest/sql/requests.py` & `dbrequest-0.1.6/src/dbrequest/sql/requests.py`

 * *Files identical despite different names*

### Comparing `dbrequest-0.1.5/.gitignore` & `dbrequest-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `dbrequest-0.1.5/LICENSE` & `dbrequest-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dbrequest-0.1.5/README.md` & `dbrequest-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `dbrequest-0.1.5/pyproject.toml` & `dbrequest-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dbrequest"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
     { name="korandr", email="korandrmail@ya.ru" },
 ]
 description = "Abstraction from DBMS, queries without explicit use of SQL, and convenient work with high-level object-containers."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `dbrequest-0.1.5/PKG-INFO` & `dbrequest-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dbrequest
-Version: 0.1.5
+Version: 0.1.6
 Summary: Abstraction from DBMS, queries without explicit use of SQL, and convenient work with high-level object-containers.
 Project-URL: Github, https://github.com/korandr/dbrequest
 Project-URL: Documentation, https://github.com/korandr/dbrequest/wiki
 Author-email: korandr <korandrmail@ya.ru>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

