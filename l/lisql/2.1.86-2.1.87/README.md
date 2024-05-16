# Comparing `tmp/lisql-2.1.86.tar.gz` & `tmp/lisql-2.1.87.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lisql-2.1.86.tar", last modified: Wed May 15 19:34:15 2024, max compression
+gzip compressed data, was "lisql-2.1.87.tar", last modified: Wed May 15 19:55:58 2024, max compression
```

## Comparing `lisql-2.1.86.tar` & `lisql-2.1.87.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 li         (501) staff       (20)        0 2024-05-15 19:34:15.568587 lisql-2.1.86/
--rw-r--r--   0 li         (501) staff       (20)     1068 2024-05-15 03:29:18.000000 lisql-2.1.86/LICENSE
--rw-r--r--   0 li         (501) staff       (20)    18997 2024-05-15 19:34:15.568484 lisql-2.1.86/PKG-INFO
--rw-r--r--   0 li         (501) staff       (20)    18214 2024-05-15 03:29:18.000000 lisql-2.1.86/README.md
--rw-r--r--   0 li         (501) staff       (20)      103 2024-05-14 14:30:06.000000 lisql-2.1.86/pyproject.toml
--rw-r--r--   0 li         (501) staff       (20)      645 2024-05-15 19:34:15.568831 lisql-2.1.86/setup.cfg
--rw-r--r--   0 li         (501) staff       (20)      726 2024-05-15 19:34:07.000000 lisql-2.1.86/setup.py
-drwxr-xr-x   0 li         (501) staff       (20)        0 2024-05-15 19:34:15.567598 lisql-2.1.86/src/
-drwxr-xr-x   0 li         (501) staff       (20)        0 2024-05-15 19:34:15.568238 lisql-2.1.86/src/lisql.egg-info/
--rw-r--r--   0 li         (501) staff       (20)    18997 2024-05-15 19:34:15.000000 lisql-2.1.86/src/lisql.egg-info/PKG-INFO
--rw-r--r--   0 li         (501) staff       (20)      196 2024-05-15 19:34:15.000000 lisql-2.1.86/src/lisql.egg-info/SOURCES.txt
--rw-r--r--   0 li         (501) staff       (20)        1 2024-05-15 19:34:15.000000 lisql-2.1.86/src/lisql.egg-info/dependency_links.txt
--rw-r--r--   0 li         (501) staff       (20)        6 2024-05-15 19:34:15.000000 lisql-2.1.86/src/lisql.egg-info/top_level.txt
--rw-r--r--   0 li         (501) staff       (20)    28248 2024-05-15 19:29:47.000000 lisql-2.1.86/src/lisql.py
+drwxr-xr-x   0 li         (501) staff       (20)        0 2024-05-15 19:55:58.756763 lisql-2.1.87/
+-rw-r--r--   0 li         (501) staff       (20)     1068 2024-05-15 03:29:18.000000 lisql-2.1.87/LICENSE
+-rw-r--r--   0 li         (501) staff       (20)    18997 2024-05-15 19:55:58.756665 lisql-2.1.87/PKG-INFO
+-rw-r--r--   0 li         (501) staff       (20)    18214 2024-05-15 03:29:18.000000 lisql-2.1.87/README.md
+-rw-r--r--   0 li         (501) staff       (20)      103 2024-05-14 14:30:06.000000 lisql-2.1.87/pyproject.toml
+-rw-r--r--   0 li         (501) staff       (20)      645 2024-05-15 19:55:58.756999 lisql-2.1.87/setup.cfg
+-rw-r--r--   0 li         (501) staff       (20)      726 2024-05-15 19:55:41.000000 lisql-2.1.87/setup.py
+drwxr-xr-x   0 li         (501) staff       (20)        0 2024-05-15 19:55:58.755898 lisql-2.1.87/src/
+drwxr-xr-x   0 li         (501) staff       (20)        0 2024-05-15 19:55:58.756443 lisql-2.1.87/src/lisql.egg-info/
+-rw-r--r--   0 li         (501) staff       (20)    18997 2024-05-15 19:55:58.000000 lisql-2.1.87/src/lisql.egg-info/PKG-INFO
+-rw-r--r--   0 li         (501) staff       (20)      196 2024-05-15 19:55:58.000000 lisql-2.1.87/src/lisql.egg-info/SOURCES.txt
+-rw-r--r--   0 li         (501) staff       (20)        1 2024-05-15 19:55:58.000000 lisql-2.1.87/src/lisql.egg-info/dependency_links.txt
+-rw-r--r--   0 li         (501) staff       (20)        6 2024-05-15 19:55:58.000000 lisql-2.1.87/src/lisql.egg-info/top_level.txt
+-rw-r--r--   0 li         (501) staff       (20)    26560 2024-05-15 19:54:54.000000 lisql-2.1.87/src/lisql.py
```

### Comparing `lisql-2.1.86/LICENSE` & `lisql-2.1.87/LICENSE`

 * *Files identical despite different names*

### Comparing `lisql-2.1.86/PKG-INFO` & `lisql-2.1.87/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lisql
-Version: 2.1.86
+Version: 2.1.87
 Summary: Provides simple funtions to interact with MySQL databases and tables.
 Home-page: https://github.com/li812/lisql
 Author: Ali Ahammad
 Author-email: aliahammad0812@outlook.com
 Project-URL: Bug Tracker, https://github.com/li812/lisql/issues
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lisql-2.1.86/README.md` & `lisql-2.1.87/README.md`

 * *Files identical despite different names*

### Comparing `lisql-2.1.86/setup.cfg` & `lisql-2.1.87/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lisql
-version = 2.1.86
+version = 2.1.87
 author = Ali Ahammad
 author_email = aliahammad0812@outlook.com
 description = Provides a simple interface to interact with MySQL databases.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/li812/lisql
 project_urls =
```

### Comparing `lisql-2.1.86/setup.py` & `lisql-2.1.87/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='lisql',
-    version='2.1.86',
+    version='2.1.87',
     py_modules=['lisql'],
     description='Provides simple funtions to interact with MySQL databases and tables.',
     author='Ali Ahammad',
     author_email='aliahammad0812@outlook.com',
     url='https://github.com/li812/lisql',
     classifiers=[
         'License :: OSI Approved :: MIT License',
```

### Comparing `lisql-2.1.86/src/lisql.egg-info/PKG-INFO` & `lisql-2.1.87/src/lisql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lisql
-Version: 2.1.86
+Version: 2.1.87
 Summary: Provides simple funtions to interact with MySQL databases and tables.
 Home-page: https://github.com/li812/lisql
 Author: Ali Ahammad
 Author-email: aliahammad0812@outlook.com
 Project-URL: Bug Tracker, https://github.com/li812/lisql/issues
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lisql-2.1.86/src/lisql.py` & `lisql-2.1.87/src/lisql.py`

 * *Files 5% similar despite different names*

```diff
@@ -366,119 +366,76 @@
                 print(info)
     except mysql.connector.Error as e:
         print(f"Error describing database: {e}")
 
 
 ########################   Start of Aggregate functions     #######################
 
-def select_count(mydb, table, column, transaction=True):
+def select_count(mydb, table, column):
     cursor = mydb.cursor()
     query = f"SELECT COUNT({column}) FROM {table}"
     try:
-        if transaction:
-            mydb.start_transaction()  # Start the transaction explicitly
-        
         cursor.execute(query)
         result = cursor.fetchone()[0]
-        
-        if transaction:
-            mydb.commit()  # Commit the transaction if transaction=True
-        
         return result
     except mysql.connector.Error as e:
-        if transaction:
-            mydb.rollback()  # Roll back the transaction if an error occurs
         print(f"Error executing query: {e}")
         return None
 
 
-def select_sum(mydb, table, column, transaction=True):
+def select_sum(mydb, table, column):
     cursor = mydb.cursor()
     query = f"SELECT SUM({column}) FROM {table}"
     try:
-        if transaction:
-            mydb.start_transaction()  # Start the transaction explicitly
-        
         cursor.execute(query)
         result = cursor.fetchone()[0]
-        
-        if transaction:
-            mydb.commit()  # Commit the transaction if transaction=True
-        
         return result
     except mysql.connector.Error as e:
-        if transaction:
-            mydb.rollback()  # Roll back the transaction if an error occurs
         print(f"Error executing query: {e}")
         return None
 
 
-def select_avg(mydb, table, column, transaction=True):
+def select_avg(mydb, table, column):
     cursor = mydb.cursor()
     query = f"SELECT AVG({column}) FROM {table}"
     try:
-        if transaction:
-            mydb.start_transaction()  # Start the transaction explicitly
-        
         cursor.execute(query)
         result = cursor.fetchone()[0]
-        
-        if transaction:
-            mydb.commit()  # Commit the transaction if transaction=True
-        
         return result
     except mysql.connector.Error as e:
-        if transaction:
-            mydb.rollback()  # Roll back the transaction if an error occurs
         print(f"Error executing query: {e}")
         return None
 
 
-def select_min(mydb, table, column, transaction=True):
+def select_min(mydb, table, column):
     cursor = mydb.cursor()
     query = f"SELECT MIN({column}) FROM {table}"
     try:
-        if transaction:
-            mydb.start_transaction()  # Start the transaction explicitly
-        
         cursor.execute(query)
         result = cursor.fetchone()[0]
-        
-        if transaction:
-            mydb.commit()  # Commit the transaction if transaction=True
-        
         return result
     except mysql.connector.Error as e:
-        if transaction:
-            mydb.rollback()  # Roll back the transaction if an error occurs
         print(f"Error executing query: {e}")
         return None
 
 
-def select_max(mydb, table, column, transaction=True):
+def select_max(mydb, table, column):
     cursor = mydb.cursor()
     query = f"SELECT MAX({column}) FROM {table}"
     try:
-        if transaction:
-            mydb.start_transaction()  # Start the transaction explicitly
-        
         cursor.execute(query)
         result = cursor.fetchone()[0]
-        
-        if transaction:
-            mydb.commit()  # Commit the transaction if transaction=True
-        
         return result
     except mysql.connector.Error as e:
-        if transaction:
-            mydb.rollback()  # Roll back the transaction if an error occurs
         print(f"Error executing query: {e}")
         return None
 
 
+
+
 ########################   End of Aggregate functions     #######################
 
 
 ########################   Start of help    #######################
 def help(func=None):
     if func is None:
         print("LiSQL Package - Python Package for Interacting with MySQL Databases")
```

