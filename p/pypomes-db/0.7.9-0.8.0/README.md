# Comparing `tmp/pypomes_db-0.7.9.tar.gz` & `tmp/pypomes_db-0.8.0.tar.gz`

## Comparing `pypomes_db-0.7.9.tar` & `pypomes_db-0.8.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pypomes_db-0.7.9/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0    11837 2020-02-02 00:00:00.000000 pypomes_db-0.7.9/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    29148 2020-02-02 00:00:00.000000 pypomes_db-0.7.9/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0    17931 2020-02-02 00:00:00.000000 pypomes_db-0.7.9/src/pypomes_db/migration_pomes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.7.9/src/pypomes_db/mysql_pomes.py
--rw-r--r--   0        0        0    16125 2020-02-02 00:00:00.000000 pypomes_db-0.7.9/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0    15202 2020-02-02 00:00:00.000000 pypomes_db-0.7.9/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    14035 2020-02-02 00:00:00.000000 pypomes_db-0.7.9/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.7.9/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.7.9/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.7.9/README.md
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.7.9/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.7.9/PKG-INFO
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pypomes_db-0.8.0/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0    11837 2020-02-02 00:00:00.000000 pypomes_db-0.8.0/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    29148 2020-02-02 00:00:00.000000 pypomes_db-0.8.0/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0    17983 2020-02-02 00:00:00.000000 pypomes_db-0.8.0/src/pypomes_db/migration_pomes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.8.0/src/pypomes_db/mysql_pomes.py
+-rw-r--r--   0        0        0    16125 2020-02-02 00:00:00.000000 pypomes_db-0.8.0/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0    15231 2020-02-02 00:00:00.000000 pypomes_db-0.8.0/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    14035 2020-02-02 00:00:00.000000 pypomes_db-0.8.0/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.8.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.8.0/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.8.0/README.md
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.8.0/PKG-INFO
```

### Comparing `pypomes_db-0.7.9/src/pypomes_db/__init__.py` & `pypomes_db-0.8.0/src/pypomes_db/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.9/src/pypomes_db/db_common.py` & `pypomes_db-0.8.0/src/pypomes_db/db_common.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.9/src/pypomes_db/db_pomes.py` & `pypomes_db-0.8.0/src/pypomes_db/db_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.9/src/pypomes_db/migration_pomes.py` & `pypomes_db-0.8.0/src/pypomes_db/migration_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,14 +94,15 @@
         if target_engine == "sqlserver":
             target_cursor.fast_executemany = True
 
         # execute the query
         source_cursor.execute(statement=sel_stmt)
 
         # fetch rows in batches/all rows
+        row_count: int = 0
         rows: list[tuple]
         if batch_size:
             rows = source_cursor.fetchmany(size=batch_size)
         else:
             rows = source_cursor.fetchall()
         while rows:
             match target_engine:
@@ -125,45 +126,46 @@
                             _db_log(logger=logger,
                                     engine="postgres",
                                     level=WARNING,
                                     stmt=f"Found NULLs in values for {insert_stmt}")
                             # search for NULLs in input data
                             cleaned_rows: [tuple] = []
                             for row in rows:
-                                cleaned_row: list = _db_remove_nulls(row)
+                                cleaned_row: list[Any] = _db_remove_nulls(row)
                                 # has the row been cleaned ?
                                 if cleaned_row:
                                     # yes, use it
                                     cleaned_rows.append(tuple(cleaned_row))
                                 else:
                                     # no, use original row
                                     cleaned_rows.append(row)
                             # insert the cleaned data
                             execute_values(cur=target_cursor,
                                            sql=insert_stmt,
                                            argslist=cleaned_rows)
                 case "sqlserver":
                     target_cursor.executemany(insert_stmt, rows)
 
+            # log partial result
+            row_count += 1
+            if row_count % 100000 == 0:
+                _db_log(logger=logger,
+                        engine=source_engine,
+                        stmt=(f"Migrated {row_count} tuples, "
+                              f"from {source_engine}.{source_table} "
+                              f"to {target_engine}.{target_table}"))
+
             # increment the tuple migration counter
             result += len(rows)
             # read the next batch
             if batch_size:
                 rows = source_cursor.fetchmany(size=batch_size)
             else:
                 rows = source_cursor.fetchall()
 
-            # log partial result
-            if rows:
-                _db_log(logger=logger,
-                        engine=source_engine,
-                        stmt=(f"Migrated {result} tuples, "
-                              f"from {source_engine}.{source_table} "
-                              f"to {target_engine}.{target_table}"))
-
         # close the cursors and commit the transactions
         source_cursor.close()
         curr_source_conn.commit()
         target_cursor.close()
         curr_target_conn.commit()
     except Exception as e:
         # rollback the transactions
@@ -315,16 +317,15 @@
                                       parameters=(*pk_vals, lob_var))
                 ora_lob = lob_var.getValue()
 
 
             # access the blob in chunks and write it to file
             offset: int = 1
             lob: Any = row[blob_index]
-            lob_data: bytes | str = lob.read(offset=offset,
-                                             amount=chunk_size)
+            lob_data: bytes | str = lob.read(offset=offset, amount=chunk_size) if lob else None
             while lob_data:
                 size: int = len(lob_data)
                 match target_engine:
                     case "mysql":
                         pass
                     case "oracle":
                         ora_lob.write(data=lob_data,
@@ -351,15 +352,15 @@
                 lob_data = lob.read(offset=offset,
                                     amount=chunk_size)
 
             # increment the LOB migration counter
             result += 1
 
             # log partial result at each 100000 LOBs migrated
-            if result % 1000000 == 0:
+            if result % 10000 == 0:
                 _db_log(logger=logger,
                         engine=source_engine,
                         stmt=(f"Migrated {result} LOBs, "
                               f"from {source_engine}.{source_table}.{source_lob_column} "
                               f"to {target_engine}.{target_table}.{target_lob_column}"))
 
         # close the cursors and commit the transactions
```

### Comparing `pypomes_db-0.7.9/src/pypomes_db/oracle_pomes.py` & `pypomes_db-0.8.0/src/pypomes_db/oracle_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.9/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.8.0/src/pypomes_db/postgres_pomes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # noinspection DuplicatedCode
 from logging import WARNING, Logger
 from pathlib import Path
 from psycopg2 import Binary, connect
 from psycopg2.extras import execute_values
 # noinspection PyProtectedMember
 from psycopg2._psycopg import connection
+from typing import Any
 
 from .db_common import (
     _db_assert_query_quota, _db_get_params,
     _db_log, _db_except_msg, _db_remove_nulls
 )
 
 
@@ -173,15 +174,15 @@
             _db_log(logger=logger,
                     engine="postgres",
                     level=WARNING,
                     stmt=f"Found NULLs in values for {insert_stmt}")
             # search for NULLs in input data
             cleaned_rows: list[tuple[int, list]] = []
             for inx, vals in enumerate(insert_vals):
-                cleaned_row: list = _db_remove_nulls(vals)
+                cleaned_row: list[Any] = _db_remove_nulls(vals)
                 # has the row been cleaned ?
                 if cleaned_row:
                     # yes, register it
                     cleaned_rows.append((inx, cleaned_row))
             # replace the cleaned rows
             for cleaned_row in cleaned_rows:
                 insert_vals[cleaned_row[0]] = tuple(cleaned_row[1])
```

### Comparing `pypomes_db-0.7.9/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.8.0/src/pypomes_db/sqlserver_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.9/LICENSE` & `pypomes_db-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.9/pyproject.toml` & `pypomes_db-0.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.7.9"
+version = "0.8.0"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -20,15 +20,15 @@
 ]
 dependencies = [
     "pip>=24.0",
 #   "mysql-connector-python>=8.4.0",
 #   "oracledb>=2.2.0",
 #   "psycopg2-binary>=2.9.9",
 #   "pyodbc>=5.1.0",
-    "pypomes_core>=1.0.3",
+    "pypomes_core>=1.0.4",
     "setuptools>=68.0.0",
     "wheel>=0.42.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/TheWiseCoder/PyPomes-DB"
 "Bug Tracker" = "https://github.com/TheWiseCoder/PyPomes-DB/issues"
```

### Comparing `pypomes_db-0.7.9/PKG-INFO` & `pypomes_db-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.3
 Name: pypomes_db
-Version: 0.7.9
+Version: 0.8.0
 Summary: A collection of Python pomes, pennyeach (database modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: pip>=24.0
-Requires-Dist: pypomes-core>=1.0.3
+Requires-Dist: pypomes-core>=1.0.4
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: wheel>=0.42.0
```

