# Comparing `tmp/MariaDB-SQLBuilder-1.0.0a6.tar.gz` & `tmp/mariadb_sqlbuilder-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MariaDB-SQLBuilder-1.0.0a6.tar", last modified: Tue Mar 14 15:40:04 2023, max compression
+gzip compressed data, was "mariadb_sqlbuilder-1.1.tar", last modified: Wed May 15 22:50:59 2024, max compression
```

## Comparing `MariaDB-SQLBuilder-1.0.0a6.tar` & `mariadb_sqlbuilder-1.1.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:40:04.358814 MariaDB-SQLBuilder-1.0.0a6/
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-03-14 15:39:50.000000 MariaDB-SQLBuilder-1.0.0a6/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:40:04.354814 MariaDB-SQLBuilder-1.0.0a6/MariaDB_SQLBuilder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-03-14 15:40:04.000000 MariaDB-SQLBuilder-1.0.0a6/MariaDB_SQLBuilder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-03-14 15:40:04.000000 MariaDB-SQLBuilder-1.0.0a6/MariaDB_SQLBuilder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 15:40:04.000000 MariaDB-SQLBuilder-1.0.0a6/MariaDB_SQLBuilder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-14 15:40:04.000000 MariaDB-SQLBuilder-1.0.0a6/MariaDB_SQLBuilder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-14 15:40:04.000000 MariaDB-SQLBuilder-1.0.0a6/MariaDB_SQLBuilder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-03-14 15:40:04.358814 MariaDB-SQLBuilder-1.0.0a6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-03-14 15:39:50.000000 MariaDB-SQLBuilder-1.0.0a6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:40:04.354814 MariaDB-SQLBuilder-1.0.0a6/mariadb_sqlbuilder/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-03-14 15:39:50.000000 MariaDB-SQLBuilder-1.0.0a6/mariadb_sqlbuilder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:40:04.354814 MariaDB-SQLBuilder-1.0.0a6/mariadb_sqlbuilder/builder/
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-03-14 15:39:50.000000 MariaDB-SQLBuilder-1.0.0a6/mariadb_sqlbuilder/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11705 2023-03-14 15:39:50.000000 MariaDB-SQLBuilder-1.0.0a6/mariadb_sqlbuilder/builder/base_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-03-14 15:39:50.000000 MariaDB-SQLBuilder-1.0.0a6/mariadb_sqlbuilder/builder/delete_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-03-14 15:39:50.000000 MariaDB-SQLBuilder-1.0.0a6/mariadb_sqlbuilder/builder/dict_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-03-14 15:39:50.000000 MariaDB-SQLBuilder-1.0.0a6/mariadb_sqlbuilder/builder/exists_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-03-14 15:39:50.000000 MariaDB-SQLBuilder-1.0.0a6/mariadb_sqlbuilder/builder/insert_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-03-14 15:39:50.000000 MariaDB-SQLBuilder-1.0.0a6/mariadb_sqlbuilder/builder/join_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-03-14 15:39:50.000000 MariaDB-SQLBuilder-1.0.0a6/mariadb_sqlbuilder/builder/select_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-03-14 15:39:50.000000 MariaDB-SQLBuilder-1.0.0a6/mariadb_sqlbuilder/builder/update_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-03-14 15:39:50.000000 MariaDB-SQLBuilder-1.0.0a6/mariadb_sqlbuilder/builder/upsert_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-03-14 15:39:50.000000 MariaDB-SQLBuilder-1.0.0a6/mariadb_sqlbuilder/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-03-14 15:39:50.000000 MariaDB-SQLBuilder-1.0.0a6/mariadb_sqlbuilder/exepetions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:40:04.358814 MariaDB-SQLBuilder-1.0.0a6/mariadb_sqlbuilder/helpful/
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-03-14 15:39:50.000000 MariaDB-SQLBuilder-1.0.0a6/mariadb_sqlbuilder/helpful/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-03-14 15:39:50.000000 MariaDB-SQLBuilder-1.0.0a6/mariadb_sqlbuilder/helpful/conditions_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-03-14 15:39:50.000000 MariaDB-SQLBuilder-1.0.0a6/mariadb_sqlbuilder/helpful/connection_dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-03-14 15:39:50.000000 MariaDB-SQLBuilder-1.0.0a6/mariadb_sqlbuilder/helpful/filter_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11884 2023-03-14 15:39:50.000000 MariaDB-SQLBuilder-1.0.0a6/mariadb_sqlbuilder/helpful/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-03-14 15:39:50.000000 MariaDB-SQLBuilder-1.0.0a6/mariadb_sqlbuilder/helpful/validator_dummy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:40:04.358814 MariaDB-SQLBuilder-1.0.0a6/mariadb_sqlbuilder/sqlscript/
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-03-14 15:39:50.000000 MariaDB-SQLBuilder-1.0.0a6/mariadb_sqlbuilder/sqlscript/splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-14 15:40:04.358814 MariaDB-SQLBuilder-1.0.0a6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-03-14 15:39:50.000000 MariaDB-SQLBuilder-1.0.0a6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:50:59.295782 mariadb_sqlbuilder-1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-05-15 22:50:51.000000 mariadb_sqlbuilder-1.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:50:59.295782 mariadb_sqlbuilder-1.1/MariaDB_SQLBuilder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-05-15 22:50:59.000000 mariadb_sqlbuilder-1.1/MariaDB_SQLBuilder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-15 22:50:59.000000 mariadb_sqlbuilder-1.1/MariaDB_SQLBuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 22:50:59.000000 mariadb_sqlbuilder-1.1/MariaDB_SQLBuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-15 22:50:59.000000 mariadb_sqlbuilder-1.1/MariaDB_SQLBuilder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 22:50:59.000000 mariadb_sqlbuilder-1.1/MariaDB_SQLBuilder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-05-15 22:50:59.295782 mariadb_sqlbuilder-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-15 22:50:51.000000 mariadb_sqlbuilder-1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:50:59.291782 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-15 22:50:51.000000 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:50:59.295782 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/builder/
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-15 22:50:51.000000 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15951 2024-05-15 22:50:51.000000 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/builder/base_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-15 22:50:51.000000 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/builder/delete_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-15 22:50:51.000000 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/builder/dict_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-15 22:50:51.000000 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/builder/exists_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-05-15 22:50:51.000000 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/builder/insert_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-05-15 22:50:51.000000 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/builder/join_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-05-15 22:50:51.000000 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/builder/select_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-05-15 22:50:51.000000 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/builder/update_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-05-15 22:50:51.000000 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/builder/upsert_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-05-15 22:50:51.000000 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-15 22:50:51.000000 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/exepetions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:50:59.295782 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/helpful/
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-05-15 22:50:51.000000 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/helpful/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-15 22:50:51.000000 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/helpful/conditions_saver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-15 22:50:51.000000 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/helpful/connection_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-15 22:50:51.000000 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/helpful/filter_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-15 22:50:51.000000 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/helpful/subquery_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11867 2024-05-15 22:50:51.000000 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/helpful/validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-15 22:50:51.000000 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/helpful/validator_dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:50:59.295782 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/sqlscript/
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-15 22:50:51.000000 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/sqlscript/splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 22:50:59.295782 mariadb_sqlbuilder-1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-15 22:50:51.000000 mariadb_sqlbuilder-1.1/setup.py
```

### Comparing `MariaDB-SQLBuilder-1.0.0a6/LICENSE` & `mariadb_sqlbuilder-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `MariaDB-SQLBuilder-1.0.0a6/MariaDB_SQLBuilder.egg-info/PKG-INFO` & `mariadb_sqlbuilder-1.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,24 @@
-Metadata-Version: 2.1
-Name: MariaDB-SQLBuilder
-Version: 1.0.0a6
-Summary: MariaDB SQL Builder is a simple way to use Maria SQL. Use your own SQL or use the integrated Maria SQL Builder tool.
-Home-page: https://github.com/princessmiku/MariaDB-SQLBuilder
-Author: Miku
-Author-email: 
-License: LGPL 2.1
-Keywords: database,mariadb,sql,builder,script builder,mariadb sql,orm
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # MariaDB SQL Builder
 
 -----
 
 [![License - GNU LPGL version 2.1](https://img.shields.io/badge/License-GNU_LPGL_version_2.1-green)](https://opensource.org/licenses/LGPL-2.1)
 [![Python - ^3.7](https://img.shields.io/badge/Python-^3.7-blue)](https://www.python.org/)
 [![Downloads](https://pepy.tech/badge/mariadb-sqlbuilder)](https://pepy.tech/project/mariadb-sqlbuilder)
 
-## Warning! Update 1.0 change many functions and variable names to the pep8 standard
+## Security fix 1.1
+
+If you are interested, the content is below
 
-Too lazy to write SQL? Then use the SQL Builder to make your life easier!
+### MariaDB license
+
+This library uses MariaDB Connector/Python, which is released under the terms of the GPLv2 license. For more 
+information, please see the [license file in the repository](https://github.com/mariadb-corporation/mariadb-connector-python/blob/1.1/LICENSE).
 
-MariaDB SQL Builder is a simple way to use SQL.
-Use your own SQL or use the integrated SQL Builder tool.
 
 # [Install](https://github.com/princessmiku/MariaDB-SQLBuilder/wiki/Installation)
 Install the package with pip
 ``pip install mariadb-sqlbuilder``
 
 Installation with pip + github
 ``pip install git+https://github.com/princessmiku/MariaDB-SQLBuilder``
@@ -71,12 +56,41 @@
 - **[Insert](https://github.com/princessmiku/MariaDB-SQLBuilder/wiki/Builder---Insert)**
 - **[Update](https://github.com/princessmiku/MariaDB-SQLBuilder/wiki/Builder---Update)**
 - **[Upsert](https://github.com/princessmiku/MariaDB-SQLBuilder/wiki/Builder---Upsert)**
 - **[Delete](https://github.com/princessmiku/MariaDB-SQLBuilder/wiki/Builder---Delete)**
 - **[CustomSQL](https://github.com/princessmiku/MariaDB-SQLBuilder/wiki/Custom-SQL)**
 
 
+## Content of the fix
+
+I have found a security problem. Variables should be given directly
+to the cursor instead of writing them to the SQL. This prevents SQL injections.
+
+By changing the avoidance of sql injection, the function “get_sql()” now returns “?”
+at the points where variables were before.
+
+To get the variables back, there is now “values_for_execute”, which contains the variables in the correct order.
+The variables are returned in the type as they are stored. 
+String as string, integer as integer, datetime as datetime...
+
+**Example**
+
+- ``conn.table().update().values_for_execute``
+- ``conn.table().select().values_for_execute``
+
+The variables are used in the statements where I suspect the possibility of SQL injection.
+
+- Setting variables
+- Where to query (conditions)
+
+Setting keys or table names, for example, is normally not something a user should do, 
+so they are written to SQL as normal.
+
+I learned a lot while working on other projects. 
+This has given me some knowledge about security. 
+So I thought it was right to apply this to old projects as well.
+
 ----------------------------------------------------------------
 
 <br>
 Not completely used but <br>
 Translated with www.DeepL.com/Translator (free version)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `MariaDB-SQLBuilder-1.0.0a6/MariaDB_SQLBuilder.egg-info/SOURCES.txt` & `mariadb_sqlbuilder-1.1/MariaDB_SQLBuilder.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -19,10 +19,11 @@
 mariadb_sqlbuilder/builder/select_builder.py
 mariadb_sqlbuilder/builder/update_builder.py
 mariadb_sqlbuilder/builder/upsert_builder.py
 mariadb_sqlbuilder/helpful/arithmetic.py
 mariadb_sqlbuilder/helpful/conditions_saver.py
 mariadb_sqlbuilder/helpful/connection_dummy.py
 mariadb_sqlbuilder/helpful/filter_operator.py
+mariadb_sqlbuilder/helpful/subquery_operator.py
 mariadb_sqlbuilder/helpful/validator.py
 mariadb_sqlbuilder/helpful/validator_dummy.py
 mariadb_sqlbuilder/sqlscript/splitter.py
```

### Comparing `MariaDB-SQLBuilder-1.0.0a6/mariadb_sqlbuilder/builder/__init__.py` & `mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `MariaDB-SQLBuilder-1.0.0a6/mariadb_sqlbuilder/builder/delete_builder.py` & `mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/builder/delete_builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,19 +29,23 @@
         Executes the DELETE SQL statement built by the builder.
         :return:
         """
         if not self.is_conditions() and not self.sure_not_use_conditions:
             raise PermissionError('Delete Builder: You are not sure enough not to use where')
         cursor = self.tb.connector.get_available_cursor()
         cursor.execute(
-            self.get_sql()
+            self.get_sql(),
+            self.values_for_execute
         )
         cursor.connection.commit()
         self.tb.connector.release_cursor(cursor)
 
     def get_sql(self) -> str:
         """
         Returns the DELETE SQL statement built by the builder as a string.
         :return:
         """
         return f"DELETE FROM {self.tb.table} " \
             f"{self._get_where_sql()};"
+
+    def __str__(self):
+        return self.get_sql()
```

### Comparing `MariaDB-SQLBuilder-1.0.0a6/mariadb_sqlbuilder/builder/dict_converter.py` & `mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/builder/dict_converter.py`

 * *Files identical despite different names*

### Comparing `MariaDB-SQLBuilder-1.0.0a6/mariadb_sqlbuilder/builder/exists_builder.py` & `mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/builder/exists_builder.py`

 * *Files 11% similar despite different names*

```diff
@@ -38,15 +38,16 @@
         """
         Checks if a row exists in the table that matches the specified conditions.
         :return:
         """
         cursor = self.tb.connector.get_available_cursor()
         try:
             cursor.execute(
-                self.get_sql()
+                self.get_sql(),
+                self.values_for_execute
             )
             result = cursor.fetchone()
         except mariadb.OperationalError as err:
             if "Unknown column" in err.args[0]:
                 result = (0,)
             else:
                 self.tb.connector.release_cursor(cursor)
@@ -63,7 +64,10 @@
         """
         if not self.column_list and not self.is_conditions():
             return f"SHOW TABLES LIKE '{self.tb.table}'"
         return f"SELECT EXISTS(SELECT " \
                f"{', '.join(self.column_list) if self.column_list else '*'} " \
                f"FROM {self.tb.table} " \
                f"{self._get_where_sql()};"
+
+    def __str__(self):
+        return self.get_sql()
```

### Comparing `MariaDB-SQLBuilder-1.0.0a6/mariadb_sqlbuilder/builder/insert_builder.py` & `mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/builder/upsert_builder.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,108 +1,107 @@
 """
-This modul is there for build a sql insert query
+This modul is there for build a sql upsert query
 """
+from datetime import timedelta, datetime
 from json import dumps
 from typing import Union, Dict, List
 
-from .base_builder import BaseBuilder, _transform_value_valid
+from _decimal import Decimal
 
+from mariadb_sqlbuilder.helpful.arithmetic import Arithmetic
+from .base_builder import BaseBuilder
 
-class InsertBuilder(BaseBuilder):
+
+class UpsertBuilder(BaseBuilder):
     """
     TODO: add a description
     This is a dummy docstring.
     """
 
     def __init__(self, tb, **kwargs):
         super().__init__(tb, **kwargs)
-        self.__ignore = False
         self.__toSet = {}
         self.__jsonBuildings = []
 
-    def set(self, column: str, value: Union[str, int, None]):
+    def set(self, column: str,  value: Union[str, int, float, bool,
+        Arithmetic, timedelta, datetime, Decimal]):
         """
-        Set the value for a column in the table.
+        Set a column value for the current table.
         :param column:
         :param value:
         :return:
         """
-        if not self.tb.table in self.__toSet:
-            self.__toSet[self.tb.table] = {}
         self.tb.validator.check_value_type(self.tb.table, column, value)
-        self.__toSet[self.tb.table][column] = _transform_value_valid(value)
+        if self.tb.table not in self.__toSet:
+            self.__toSet[self.tb.table] = {}
+        self.__toSet[self.tb.table][column] = value
         return self
 
     def add_join_table(self, table: str):
         """
-        Add a join table to the set of tables to insert data into.
+        Add a join table to the UpsertBuilder object.
         :param table:
         :return:
         """
         if table in self.__toSet:
             return self
         self.__toSet[table] = {}
         return self
 
-    def table_set(self, table: str, column: str, value: Union[str, int, None]):
+    def table_set(self, table: str, column: str, value: Union[str, int, float, bool,
+        Arithmetic, timedelta, datetime, Decimal]):
         """
-        Insert data into another table in one insert.
+        Set a column value for a specific table.
         :param table:
         :param column:
         :param value:
         :return:
         """
-        if not table in self.__toSet:
-            self.__toSet[table] = {}
         self.tb.validator.check_value_type(table, column, value)
-        self.__toSet[table][column] = _transform_value_valid(value)
-        return self
-
-    def ignore(self, _ignore: bool = True):
-        """
-        Set whether to ignore errors during the insert.
-        :param _ignore:
-        :return:
-        """
-        self.__ignore = _ignore
+        if table not in self.__toSet:
+            self.__toSet[table] = {}
+        self.__toSet[table][column] = value
         return self
 
-    def execute(self) -> bool:
+    def execute(self):
         """
-        Execute the insert query.
+        Execute the UpsertBuilder object's SQL query and commit the changes.
         :return:
         """
         cursor = self.tb.connector.get_available_cursor()
-        result = cursor.execute(
-            self.get_sql()
+        cursor.execute(
+            self.get_sql(),
+            self.values_for_execute
         )
         cursor.connection.commit()
         self.tb.connector.release_cursor(cursor)
-        return result
 
     def get_sql(self) -> str:
         """
-        Get the SQL query string for the insert.
+        Get the SQL query string for the UpsertBuilder object.
         :return:
         """
+        self._values_for_execute.clear()
         for element in self.__jsonBuildings:
             self.__set_json(element[0], element[1])
         sql = ""
-        key: str
-        value: Dict[str, dict]
-        for key, value in self.__toSet.items():
-            if not value:
-                continue
-            sql += f"INSERT {'IGNORE ' if self.__ignore else ''}INTO " \
-                   f"{key} ({', '.join(value.keys())}) VALUES ({', '.join(value.values())});"
+        _key: str
+        _value: Dict[str, dict]
+        for _key, _value in self.__toSet.items():
+            self._values_for_execute += _value.values()  # first add is for INSERT values
+            self._values_for_execute += _value.values()  # second add is for on duplicate values
+            sql += f"INSERT INTO " \
+                   f"{_key} ({', '.join(_value.keys())}) VALUES ({', '.join(['?'] * len(_value.values()))}) " \
+                   f"ON DUPLICATE KEY UPDATE " \
+                   f"{', '.join([f'{key} = ?' for key in _value.keys()])};"
         return sql
 
     def __set_json(self, json: Dict[str, any], pop: List[str] = None):
         """
-        Set values using a JSON object.
+        Set column values using a JSON object.
         :param json:
         :param pop:
         :return:
         """
         if pop is None:
             pop = []
         key: str
@@ -117,15 +116,18 @@
                     self.set(key, dumps(value))
             else:
                 self.set(key, value)
         return self
 
     def set_json(self, json: Dict[str, any], pop: List[str] = None):
         """
-        Set values with a json, don't forget where
+        Set values with a json.
         :param json: dict with data example from select
         :param pop: pop keys from the json,
         if you have keys inside that are not a table but a dict/list
         :return:
         """
         self.__jsonBuildings.append([json, pop])
         return self
+
+    def __str__(self):
+        return self.get_sql()
```

### Comparing `MariaDB-SQLBuilder-1.0.0a6/mariadb_sqlbuilder/builder/join_builder.py` & `mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/builder/join_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 This modul is there for build sql joins for your query
 
 Maria DB SQL joins
 https://mariadb.com/kb/en/joining-tables-with-join-clauses/
-
 """
 from abc import ABC, abstractmethod
 
 from .base_builder import _get_tcn_without_validator
 
 
 class _JoinBuilder(ABC):
@@ -160,7 +159,10 @@
         conditions = []
         for con in self.conditions:
             conditions.append(
                 f"{_get_tcn_without_validator(self.from_table, con[0])} = " +
                 f"{_get_tcn_without_validator(self.table, con[1])}"
             )
         return f"RIGHT JOIN {self.table} ON {' AND '.join(conditions)} "
+
+    def __str__(self):
+        return self.get_sql()
```

### Comparing `MariaDB-SQLBuilder-1.0.0a6/mariadb_sqlbuilder/builder/select_builder.py` & `mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/builder/select_builder.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
     def __init__(self, tb, expressions: Union[str, list], *args, **kwargs):
         ConditionsBuilder.__init__(self, tb, **kwargs)
         BaseJoinExtension.__init__(self, tb, **kwargs)
         self._contains_arithmetic = False
         self.expressions = []
         self._loop_tb_expressions_add(self.tb.table, expressions, *args)
+        self._limit = ""
 
     def join_select(self, join_table: str, expressions: Union[str, list], *args):
         """
         Adds a JOIN clause to the SELECT query with the provided table and column.
         :param join_table:
         :param expressions:
         :return:
@@ -45,15 +46,16 @@
     def fetchone(self):
         """
         Executes the SELECT query and returns the first row of the result.
         :return:
         """
         cursor = self.tb.connector.get_available_cursor()
         cursor.execute(
-            self.get_sql()
+            self.get_sql(),
+            self.values_for_execute
         )
         result = cursor.fetchone()
         cursor.connection.commit()
         self.tb.connector.release_cursor(cursor)
         return result
 
     def fetchone_json(self):
@@ -70,15 +72,16 @@
     def fetchall(self):
         """
         Executes the SELECT query and returns all the rows of the result.
         :return:
         """
         cursor = self.tb.connector.get_available_cursor()
         cursor.execute(
-            self.get_sql()
+            self.get_sql(),
+            self.values_for_execute
         )
         result = cursor.fetchall()
         cursor.connection.commit()
         self.tb.connector.release_cursor(cursor)
         return result
 
     def fetchall_json(self):
@@ -88,22 +91,36 @@
         """
         if self._contains_arithmetic:
             raise JsonNotSupported(
                 "This query contains arithmetics, they are not supported in json returns"
             )
         return convert_to_dict_all(self.tb.table, self.expressions, self.fetchall())
 
+    def limit(self, count: int, offset: int = 0):
+        """
+        Set a max fetching limit
+        :param count:
+        :param offset:
+        :return:
+        """
+        self._limit = ""
+        if count:
+            self._limit += " LIMIT " + str(count)
+            if offset:
+                self._limit += " OFFSET " + str(offset)
+        return self
+
     def get_sql(self) -> str:
         """
         Builds the SELECT query and returns it as a string.
         :return:
         """
         return f"SELECT {', '.join(self.expressions)} FROM {self.tb.table} " \
                f"{' '.join(self._joins) if self._joins else ''} " \
-            f"{self._get_where_sql()};"
+            f"{self._get_where_sql()}{self._limit};"
 
     def _loop_tb_expressions_add(self, tb: str, expressions: Union[str, Arithmetic], *args):
         """
         Handle different types of expressions and add it correctly in the expressions list
         :param tb:
         :param expressions:
         :param args:
@@ -122,7 +139,10 @@
                 loop_expressions += args
             for expression in loop_expressions:
                 if isinstance(expression, Arithmetic):
                     self._contains_arithmetic = True
                     self.expressions.append(str(expression))
                 else:
                     self.expressions.append(_get_tcn_validator(tb, expression, self.tb.validator))
+
+    def __str__(self):
+        return self.get_sql()
```

### Comparing `MariaDB-SQLBuilder-1.0.0a6/mariadb_sqlbuilder/builder/update_builder.py` & `mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/builder/update_builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 from datetime import timedelta, datetime
 from json import dumps
 from typing import Union, Dict, List
 
 from _decimal import Decimal
 
 from mariadb_sqlbuilder.helpful.arithmetic import Arithmetic
-from .base_builder import ConditionsBuilder, _transform_value_valid, \
-    _get_tcn_without_validator
+from .base_builder import ConditionsBuilder, _get_tcn_without_validator
 from .join_builder import BaseJoinExtension
 
 
 class UpdateBuilder(ConditionsBuilder, BaseJoinExtension):
     """
     TODO: add a description
     This is a dummy docstring.
@@ -33,30 +32,32 @@
         """
         Set a value for a column in the table to update.
         :param column:
         :param value:
         :return:
         """
         self.tb.validator.check_value_type(self.tb.table, column, value)
-        self.__toSet[_get_tcn_without_validator(self.tb, column)] = _transform_value_valid(value)
+        self.__toSet[
+            _get_tcn_without_validator(self.tb.table, column)
+        ] = value
         return self
 
     def join_set(self, join_table: str, join_column: str, value: Union[str, int, float, bool,
         Arithmetic, timedelta, datetime, Decimal]):
         """
         Set a value for a column in a join table.
         :param join_table:
         :param join_column:
         :param value:
         :return:
         """
         self.tb.validator.check_value_type(join_table, join_column, value)
         self.__toSet[
             _get_tcn_without_validator(join_table, join_column)
-        ] = _transform_value_valid(value)
+        ] = value
         return self
 
     def im_sure_im_not_use_conditions(self, im_sure: bool = True):
         """
         Set a flag to indicate that the where conditions are not needed.
         :param im_sure:
         :return:
@@ -68,35 +69,45 @@
         """
         Execute the update statement.
         :return:
         """
         if not self.is_conditions() and not self.sure_not_use_conditions:
             raise PermissionError('Update Builder: You are not sure enough not to use where')
         cursor = self.tb.connector.get_available_cursor()
-        cursor.execute(
-            self.get_sql()
+        sql_script = self.get_sql()
+        result = cursor.execute(
+            sql_script,
+            self.values_for_execute
         )
         if self.__subSets:
             for subset in self.__subSets:
                 cursor.execute(subset.get_sql())
         cursor.connection.commit()
         self.tb.connector.release_cursor(cursor)
 
+    def _get_value_string(self):
+        elements = []
+        for key, value in self.__toSet.items():
+            elements.append(key + ' = ?')
+            self._values_for_execute.append(value)
+        return ', '.join(elements) + ' '
+
     def get_sql(self) -> str:
         """
         Get the SQL statement to execute.
         :return:
         """
+        self._values_for_execute.clear()  # clear the execution values
         for element in self.__jsonBuildings:
             self.__set_json(element[0], element[1])
-        sql = f"UPDATE {self.tb.table} " \
-              f"{' '.join(self._joins) if self._joins else ''} " \
-              f"SET " \
-              f"{', '.join([f'{key} = {value}' for (key, value) in self.__toSet.items()])} " \
-              f"{self._get_where_sql()};"
+
+        sql = ((f"UPDATE {self.tb.table} "
+               f"{' '.join(self._joins) if self._joins else ''} "
+               f"SET ") + self._get_value_string() +
+               f" {self._get_where_sql()};")
         return sql
 
     def __set_json(self, json: Dict[str, any], pop: List[str] = None):
         """
         Set values from a json object.
         :param json:
         :param pop:
@@ -124,7 +135,10 @@
         :param json: dict with data example from select
         :param pop: pop keys from the json,
         if you have keys inside that are not a table but a dict/list
         :return:
         """
         self.__jsonBuildings.append([json, pop])
         return self
+
+    def __str__(self):
+        return self.get_sql()
```

### Comparing `MariaDB-SQLBuilder-1.0.0a6/mariadb_sqlbuilder/connector.py` & `mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 The module is there to establish a connection to the database
 """
+
 from typing import Union
 
 import mariadb
 
 from mariadb_sqlbuilder.helpful.validator_dummy import ValidatorDummy
 from mariadb_sqlbuilder.helpful.validator import Validator
 from mariadb_sqlbuilder.builder import TableBuilder
```

### Comparing `MariaDB-SQLBuilder-1.0.0a6/mariadb_sqlbuilder/exepetions.py` & `mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/exepetions.py`

 * *Files identical despite different names*

### Comparing `MariaDB-SQLBuilder-1.0.0a6/mariadb_sqlbuilder/helpful/conditions_saver.py` & `mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/helpful/conditions_saver.py`

 * *Files identical despite different names*

### Comparing `MariaDB-SQLBuilder-1.0.0a6/mariadb_sqlbuilder/helpful/connection_dummy.py` & `mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/helpful/connection_dummy.py`

 * *Files identical despite different names*

### Comparing `MariaDB-SQLBuilder-1.0.0a6/mariadb_sqlbuilder/helpful/validator.py` & `mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/helpful/validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,17 +33,15 @@
         self.nullable = nullable
         self.range: Tuple[int, int] = (0, 0)
         self.length = length
         self.unsigned = unsigned
         self.data_type_name = data_type
         self.data_type: any = None
         self.character_set_name = character_set_name
-        if data_type in ["varchar", "text"]:
-            self.data_type = str
-        elif data_type in ["int", "bigint", "smallint", "mediumint", "tinyint", "year"]:
+        if data_type in ["int", "bigint", "smallint", "mediumint", "tinyint", "year"]:
             self.data_type = int
             if data_type == "int":
                 if unsigned:
                     if length < 10:
                         self.range = (0, int("9" * length))
                     else:
                         self.range = (0, 4294967295)
@@ -142,14 +140,16 @@
                     self.length = 16777215
             elif data_type == "longblob":
                 if length == 0:
                     self.length = 4294967295
             elif data_type == "tinyblob":
                 if length == 0:
                     self.length = 255
+            else:
+                raise TypeError('Not found')
         elif data_type in ["uuid"]:
             self.data_type = UUID
         elif data_type in ["date", "datetime", "timestamp"]:
             self.data_type = datetime
         elif data_type in ["time"]:
             self.data_type = timedelta
         elif data_type in ["enum"]:
```

### Comparing `MariaDB-SQLBuilder-1.0.0a6/mariadb_sqlbuilder/helpful/validator_dummy.py` & `mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/helpful/validator_dummy.py`

 * *Files identical despite different names*

### Comparing `MariaDB-SQLBuilder-1.0.0a6/mariadb_sqlbuilder/sqlscript/splitter.py` & `mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/sqlscript/splitter.py`

 * *Files identical despite different names*

### Comparing `MariaDB-SQLBuilder-1.0.0a6/setup.py` & `mariadb_sqlbuilder-1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pathlib
 from setuptools import setup
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 
-VERSION = '1.0.0a6'
+VERSION = '1.1'
 
 setup(
     name='MariaDB-SQLBuilder',
     long_description=README,
     long_description_content_type="text/markdown",
     version=VERSION,
     packages=[
@@ -19,18 +19,18 @@
     ],
     url='https://github.com/princessmiku/MariaDB-SQLBuilder',
     license='LGPL 2.1',
     author='Miku',
     author_email='',
     description='MariaDB SQL Builder is a simple way to use Maria SQL. '
                 'Use your own SQL or use the integrated Maria SQL Builder tool.',
-    keywords=['database', 'mariadb', 'sql', 'builder', 'script builder', 'mariadb sql', 'orm'],
+    keywords=['database', 'mariadb', 'sql', 'builder', 'script builder', 'mariadb sql'],
     python_requires='>=3.7.0',
     install_requires=[
-        "mariadb>=1.1.4",
+        "mariadb>=1.1.6",
     ],
     classifiers=[
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
```

