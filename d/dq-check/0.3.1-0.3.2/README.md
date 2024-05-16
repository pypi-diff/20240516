# Comparing `tmp/dq_check-0.3.1.tar.gz` & `tmp/dq_check-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dq_check-0.3.1.tar", last modified: Tue May 14 04:21:11 2024, max compression
+gzip compressed data, was "dq_check-0.3.2.tar", last modified: Thu May 16 03:48:34 2024, max compression
```

## Comparing `dq_check-0.3.1.tar` & `dq_check-0.3.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 rohan.goel   (502) staff       (20)        0 2024-05-14 04:21:11.802461 dq_check-0.3.1/
--rw-r--r--   0 rohan.goel   (502) staff       (20)     2679 2024-05-14 04:21:11.802191 dq_check-0.3.1/PKG-INFO
--rw-r--r--   0 rohan.goel   (502) staff       (20)     2440 2024-05-12 21:16:29.000000 dq_check-0.3.1/README.md
--rw-r--r--   0 rohan.goel   (502) staff       (20)      327 2024-05-14 04:20:39.000000 dq_check-0.3.1/pyproject.toml
--rw-r--r--   0 rohan.goel   (502) staff       (20)      131 2024-05-14 04:21:11.803377 dq_check-0.3.1/setup.cfg
-drwxr-xr-x   0 rohan.goel   (502) staff       (20)        0 2024-05-14 04:21:11.793110 dq_check-0.3.1/src/
-drwxr-xr-x   0 rohan.goel   (502) staff       (20)        0 2024-05-14 04:21:11.796614 dq_check-0.3.1/src/dq_check/
--rw-r--r--   0 rohan.goel   (502) staff       (20)       29 2024-05-05 04:45:50.000000 dq_check-0.3.1/src/dq_check/__init__.py
--rw-r--r--   0 rohan.goel   (502) staff       (20)    15934 2024-05-14 04:19:45.000000 dq_check-0.3.1/src/dq_check/dq_check.py
-drwxr-xr-x   0 rohan.goel   (502) staff       (20)        0 2024-05-14 04:21:11.801270 dq_check-0.3.1/src/dq_check.egg-info/
--rw-r--r--   0 rohan.goel   (502) staff       (20)     2679 2024-05-14 04:21:11.000000 dq_check-0.3.1/src/dq_check.egg-info/PKG-INFO
--rw-r--r--   0 rohan.goel   (502) staff       (20)      263 2024-05-14 04:21:11.000000 dq_check-0.3.1/src/dq_check.egg-info/SOURCES.txt
--rw-r--r--   0 rohan.goel   (502) staff       (20)        1 2024-05-14 04:21:11.000000 dq_check-0.3.1/src/dq_check.egg-info/dependency_links.txt
--rw-r--r--   0 rohan.goel   (502) staff       (20)       15 2024-05-14 04:21:11.000000 dq_check-0.3.1/src/dq_check.egg-info/requires.txt
--rw-r--r--   0 rohan.goel   (502) staff       (20)        9 2024-05-14 04:21:11.000000 dq_check-0.3.1/src/dq_check.egg-info/top_level.txt
+drwxr-xr-x   0 rohan.goel   (502) staff       (20)        0 2024-05-16 03:48:34.389885 dq_check-0.3.2/
+-rw-r--r--   0 rohan.goel   (502) staff       (20)     2679 2024-05-16 03:48:34.389465 dq_check-0.3.2/PKG-INFO
+-rw-r--r--   0 rohan.goel   (502) staff       (20)     2440 2024-05-12 21:16:29.000000 dq_check-0.3.2/README.md
+-rw-r--r--   0 rohan.goel   (502) staff       (20)      327 2024-05-16 03:47:54.000000 dq_check-0.3.2/pyproject.toml
+-rw-r--r--   0 rohan.goel   (502) staff       (20)      131 2024-05-16 03:48:34.390942 dq_check-0.3.2/setup.cfg
+drwxr-xr-x   0 rohan.goel   (502) staff       (20)        0 2024-05-16 03:48:34.381247 dq_check-0.3.2/src/
+drwxr-xr-x   0 rohan.goel   (502) staff       (20)        0 2024-05-16 03:48:34.384051 dq_check-0.3.2/src/dq_check/
+-rw-r--r--   0 rohan.goel   (502) staff       (20)       29 2024-05-05 04:45:50.000000 dq_check-0.3.2/src/dq_check/__init__.py
+-rw-r--r--   0 rohan.goel   (502) staff       (20)    16289 2024-05-16 03:40:41.000000 dq_check-0.3.2/src/dq_check/dq_check.py
+drwxr-xr-x   0 rohan.goel   (502) staff       (20)        0 2024-05-16 03:48:34.388420 dq_check-0.3.2/src/dq_check.egg-info/
+-rw-r--r--   0 rohan.goel   (502) staff       (20)     2679 2024-05-16 03:48:34.000000 dq_check-0.3.2/src/dq_check.egg-info/PKG-INFO
+-rw-r--r--   0 rohan.goel   (502) staff       (20)      263 2024-05-16 03:48:34.000000 dq_check-0.3.2/src/dq_check.egg-info/SOURCES.txt
+-rw-r--r--   0 rohan.goel   (502) staff       (20)        1 2024-05-16 03:48:34.000000 dq_check-0.3.2/src/dq_check.egg-info/dependency_links.txt
+-rw-r--r--   0 rohan.goel   (502) staff       (20)       15 2024-05-16 03:48:34.000000 dq_check-0.3.2/src/dq_check.egg-info/requires.txt
+-rw-r--r--   0 rohan.goel   (502) staff       (20)        9 2024-05-16 03:48:34.000000 dq_check-0.3.2/src/dq_check.egg-info/top_level.txt
```

### Comparing `dq_check-0.3.1/PKG-INFO` & `dq_check-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dq_check
-Version: 0.3.1
+Version: 0.3.2
 Summary: A data quality check module for Spark
 Author-email: rohan goel <rohan.goel@databricks.com>
 Description-Content-Type: text/markdown
 Requires-Dist: pyspark
 Requires-Dist: pandas
 
 ## dq_check
```

### Comparing `dq_check-0.3.1/README.md` & `dq_check-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `dq_check-0.3.1/src/dq_check/dq_check.py` & `dq_check-0.3.2/src/dq_check/dq_check.py`

 * *Files 3% similar despite different names*

```diff
@@ -219,16 +219,16 @@
 
         
         #validate sql
 
         table_cols,sql_tables = self.parse_sql_query(sql_query)
 
         # table validation
-        if table_name_only not in sql_tables:
-            raise ValueError(f"table {table_name_only} not in sql from clause {sql_tables}")
+        if table_name_only not in sql_query:
+            raise ValueError(f"table {table_name_only} not in sql from clause {sql_query}")
         
         if '*' not in table_cols:
           #primary key validation
           if set(primary_keys) - set(table_cols):
                   if not agg_ind:
                       agg_without_pk_ind = 'n'
                       raise ValueError(f"primary key {primary_keys} not in sql select clause {table_cols}")
@@ -243,22 +243,26 @@
 
         #### DQ check logic     
 
         #get total count from table for batch id
         total_count_sql = f"with sql_sample as ({sql_stmt}) select count(*) as tot_cnt from sql_sample"
         print(F"total count sql:{total_count_sql}")
         #create dq check sql
-        dq_sql = f"with sql_sample as ({sql_stmt}) " + sql_query.replace(table_name,'sql_sample')
+        #dq_sql = f"with sql_sample as ({sql_stmt}) " + sql_query.replace(table_name,'sql_sample')
+        dq_sql_pre = f"with sql_sample as ({sql_stmt}) ," + "dq_check  as " + "(" + sql_query.replace(table_name,'sql_sample') + ")"
+        dq_sql = dq_sql_pre + " select * from dq_check"
         print(F"dq_sql:{dq_sql}")
         #get count of records failing dq check
-        dq_count_sql = f"select count(*) as dq_cnt from ({dq_sql})"
+        #dq_count_sql = f"select count(*) as dq_cnt from ({dq_sql})"
+        dq_count_sql = dq_sql_pre + " select count(*) as dq_cnt from dq_check"
         print(F"dq_count_sql:{dq_count_sql}")
         #create primary keys for select expression
         primary_keys_str = ','.join(primary_keys)
-        dq_primary_key_sql = F"(select {primary_keys_str} from ({dq_sql}))"
+        #dq_primary_key_sql = F"(select {primary_keys_str} from ({dq_sql}))"
+        dq_primary_key_sql = dq_sql_pre + F" select {primary_keys_str} from dq_check"
         print(F"dq_primary_key_sql:{dq_primary_key_sql}")
 
         df_dq_count = client.read_sql(dq_count_sql)
         df_total_count = client.read_sql(total_count_sql)
         dq_count = list(df_dq_count.first().asDict().values())[0]
         total_count = list(df_total_count.first().asDict().values())[0]
```

### Comparing `dq_check-0.3.1/src/dq_check.egg-info/PKG-INFO` & `dq_check-0.3.2/src/dq_check.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dq_check
-Version: 0.3.1
+Version: 0.3.2
 Summary: A data quality check module for Spark
 Author-email: rohan goel <rohan.goel@databricks.com>
 Description-Content-Type: text/markdown
 Requires-Dist: pyspark
 Requires-Dist: pandas
 
 ## dq_check
```

