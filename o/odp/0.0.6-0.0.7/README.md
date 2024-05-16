# Comparing `tmp/odp-0.0.6.tar.gz` & `tmp/odp-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odp-0.0.6.tar", max compression
+gzip compressed data, was "odp-0.0.7.tar", max compression
```

## Comparing `odp-0.0.6.tar` & `odp-0.0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      582 2024-05-14 17:57:09.247221 odp-0.0.6/LICENSE
--rw-r--r--   0        0        0     2002 2024-05-14 17:57:09.841762 odp-0.0.6/README.md
--rw-r--r--   0        0        0        0 2024-05-13 16:35:32.352855 odp-0.0.6/odp/__init__.py
--rw-r--r--   0        0        0       67 2024-05-14 17:57:09.253889 odp-0.0.6/odp/__main__.py
--rw-r--r--   0        0        0        0 2024-05-13 16:35:32.353425 odp-0.0.6/odp/cli/__init__.py
--rw-r--r--   0        0        0     4049 2024-05-14 18:09:06.165941 odp-0.0.6/odp/cli/main.py
--rw-r--r--   0        0        0        0 2024-05-13 16:35:32.353850 odp-0.0.6/odp/core/__init__.py
--rw-r--r--   0        0        0     5525 2024-05-14 17:57:09.692111 odp-0.0.6/odp/core/detect_unused.py
--rw-r--r--   0        0        0     2770 2024-05-14 17:57:09.691865 odp-0.0.6/odp/core/snowflake.py
--rw-r--r--   0        0        0      994 2024-05-14 18:10:28.564415 odp-0.0.6/odp/core/types.py
--rw-r--r--   0        0        0     2046 2024-05-14 18:27:24.755570 odp-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2906 1970-01-01 00:00:00.000000 odp-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      582 2024-05-16 13:50:22.714107 odp-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2002 2024-05-16 13:50:22.714494 odp-0.0.7/README.md
+-rw-r--r--   0        0        0        0 2024-05-13 16:35:32.352855 odp-0.0.7/odp/__init__.py
+-rw-r--r--   0        0        0       67 2024-05-16 13:50:22.714853 odp-0.0.7/odp/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-13 16:35:32.353425 odp-0.0.7/odp/cli/__init__.py
+-rw-r--r--   0        0        0     4358 2024-05-16 13:58:56.864831 odp-0.0.7/odp/cli/main.py
+-rw-r--r--   0        0        0        0 2024-05-13 16:35:32.353850 odp-0.0.7/odp/core/__init__.py
+-rw-r--r--   0        0        0     8773 2024-05-16 13:58:56.865397 odp-0.0.7/odp/core/detect_unused.py
+-rw-r--r--   0        0        0     3121 2024-05-16 13:59:34.833764 odp-0.0.7/odp/core/snowflake.py
+-rw-r--r--   0        0        0     1049 2024-05-16 13:58:56.865903 odp-0.0.7/odp/core/types.py
+-rw-r--r--   0        0        0     2046 2024-05-16 14:00:15.859845 odp-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2906 1970-01-01 00:00:00.000000 odp-0.0.7/PKG-INFO
```

### Comparing `odp-0.0.6/LICENSE` & `odp-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `odp-0.0.6/README.md` & `odp-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `odp-0.0.6/odp/cli/main.py` & `odp-0.0.7/odp/cli/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 import click
 from dotenv import load_dotenv
 
-from odp.core.detect_unused import build_info_schema, detect_unused_columns, read_info_schema_from_file, read_queries
+from odp.core.detect_unused import (
+    build_info_schema,
+    detect_unused_columns,
+    detect_unused_tables,
+    read_info_schema_from_file,
+    read_queries,
+)
 from odp.core.snowflake import get_snowflake_queries, get_snowflake_schema, load_snowflake_credentials
 from odp.core.types import Dialect, Grain, validate_dialect, validate_grain
 
 load_dotenv()
 
 
 @click.group(name="odp")
@@ -17,83 +23,91 @@
     "detect-unused",
     help="""
 Detect unused columns in SQL queries.
 Requires two files: a query file and an information schema file.
 Run `show-queries` to see the SQL queries to run against your
 Snowflake instance to generate the two files.""",
 )
-@click.option("--queries_file", help="The SQL query file to analyze.")
-@click.option("--info_schema_file", help="The file containing the information schema for the database.")
+@click.option("--queries-file", help="The SQL query file to analyze.")
+@click.option("--info-schema-file", help="The file containing the information schema for the database.")
 @click.option(
     "--dialect",
     type=click.Choice([d.value for d in Dialect]),
     callback=validate_dialect,
     default="snowflake",
     help="The type of warehouse to connect to. Currently only snowflake is supported.",
 )
 @click.option(
     "--grain",
     type=click.Choice([g.value for g in Grain]),
     callback=validate_grain,
-    default="column",
-    help="the grain to search for, e.g. use --grain=table to search for unused tables. Default is column.",
+    default="table",
+    help="the grain to search for, e.g. use --grain=column to search for unused tables. Default is table.",
+)
+@click.option(
+    "--since-days",
+    type=click.INT,
+    default=60,
+    help="Count as 'unused' any asset that has not been queried in the last N days. Defaults to 60 days",
 )
 def cli_detect_unused_columns(
     queries_file: str | None,
     info_schema_file: str | None,
     dialect: Dialect,
     grain: Grain,
+    since_days: int,
 ):
     if queries_file and info_schema_file:
-        queries = read_queries(queries_file)
+        queries = read_queries(queries_file, since_days)
         print(f"Read {len(queries)} queries from {queries_file}")
 
         info_schema, info_schema_flat = read_info_schema_from_file(info_schema_file)
         print(f"Read {len(info_schema_flat)} information schema rows from {info_schema_file}")
         if grain == Grain.column:
             detect_unused_columns(queries, info_schema, info_schema_flat, dialect)
         elif grain == Grain.table:
-            raise NotImplementedError("Table grain is not yet supported")
+            detect_unused_tables(queries, info_schema, info_schema_flat, dialect)
         elif grain == Grain.schema:
             raise NotImplementedError("Schema grain is not yet supported")
 
         return
 
     if dialect == Dialect.snowflake:
         try:
             credentials = load_snowflake_credentials()
         except KeyError as e:
             raise ValueError(
                 f"""
 Missing or invalid parameters: {e}. Please provide either
 
-   1. both of --info_schema_file and --queries_file (use "odp show-queries" to generate these
+   1. both of --info_schema-file and --queries-file (use "odp show-queries" to learn how to generate these)
    2. valid crendentials via env, e.g. ODP_SNOWFLAKE_ACCOUNT, ODP_SNOWFLAKE_USER, etc
             """
             ) from e
 
         schema = get_snowflake_schema(credentials)
-        queries = get_snowflake_queries(credentials)
+        queries = get_snowflake_queries(credentials, since_days)
 
         info_schema, info_schema_flat = build_info_schema(schema)
         if grain == Grain.column:
             detect_unused_columns(queries, info_schema, info_schema_flat, dialect)
         elif grain == Grain.table:
-            raise NotImplementedError("Table grain is not yet supported")
+            detect_unused_tables(queries, info_schema, info_schema_flat, dialect)
         elif grain == Grain.schema:
             raise NotImplementedError("Schema grain is not yet supported")
     elif dialect == Dialect.bigquery:
         raise NotImplementedError("Loading BigQuery data via credentials is not yet supported")
     elif dialect == Dialect.redshift:
         raise NotImplementedError("Loading Redshift data via credentials is not yet supported")
 
 
 @cli.command("show-queries")
 def show_snowflake_queries():
-    print("Run the below against your snowflake instance to generate a dataset you can" "export to CSV for analysis")
+    print(
+        "Run the below against your snowflake instance to generate a dataset you can" "export to CSV for analysis")
     print(
         """
 -- query_file
 
 SELECT *
 FROM SNOWFLAKE.ACCOUNT_USAGE.QUERY_HISTORY
 WHERE QUERY_TEXT ILIKE 'select%'
```

### Comparing `odp-0.0.6/odp/core/snowflake.py` & `odp-0.0.7/odp/core/snowflake.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+from datetime import timedelta, datetime
 
 import snowflake.connector
 from pydantic import BaseModel
 
 from odp.core.types import QueryRow, SchemaRow
 
 
@@ -24,39 +25,55 @@
         snowflake_user=os.environ["ODP_SNOWFLAKE_USERNAME"],
         snowflake_password=os.environ["ODP_SNOWFLAKE_PASSWORD"],
         snowflake_database=os.environ["ODP_SNOWFLAKE_DATABASE"],
         snowflake_warehouse=os.environ.get("ODP_SNOWFLAKE_WAREHOUSE"),
         snowflake_role=os.environ.get("ODP_SNOWFLAKE_ROLE"),
     )
 
+def get_snowflake_queries(credentials: SnowflakeCredentials, since_days: int) -> list[QueryRow]:
+
+    start_datetime = datetime.now() - timedelta(days=since_days)
+
 
-def get_snowflake_queries(credentials: SnowflakeCredentials) -> list[QueryRow]:
     conn = snowflake.connector.connect(
         user=credentials.snowflake_user,
         password=credentials.snowflake_password,
         account=credentials.snowflake_account,
         database=credentials.snowflake_database,
         role=credentials.snowflake_role,
         warehouse=credentials.snowflake_warehouse,
     )
 
     # Create a cursor object.
     cur = conn.cursor()
 
+
     # Execute a statement that will generate a result set.
     sql = """
-SELECT QUERY_TEXT, DATABASE_NAME, SCHEMA_NAME
+SELECT QUERY_TEXT, DATABASE_NAME, SCHEMA_NAME, START_TIME
 FROM SNOWFLAKE.ACCOUNT_USAGE.QUERY_HISTORY
-WHERE QUERY_TEXT ILIKE 'select%'
+WHERE QUERY_TEXT ILIKE 'select%%'
+    AND DATABASE_NAME = %(database_name)s
+    AND START_TIME > %(start_datetime)s
 ORDER BY START_TIME DESC
-LIMIT 10000; -- or start_time > $SOME_DATE to get columns unused in the last N days
+LIMIT 10000; 
         """
-    cur.execute(sql)
-
-    return [QueryRow(QUERY_TEXT=row[0], DATABASE_NAME=row[1], SCHEMA_NAME=row[2]) for row in cur.fetchall()]
+    cur.execute(sql, {
+        "database_name": credentials.snowflake_database,
+        "start_datetime": start_datetime,
+    })
+
+    return [
+        QueryRow(
+            QUERY_TEXT=row[0],
+            DATABASE_NAME=row[1],
+            SCHEMA_NAME=row[2],
+            START_TIME=row[3],
+        ) for row in cur.fetchall()
+    ]
 
 
 def get_snowflake_schema(credentials: SnowflakeCredentials) -> list[SchemaRow]:
     conn = snowflake.connector.connect(
         user=credentials.snowflake_user,
         password=credentials.snowflake_password,
         account=credentials.snowflake_account,
```

### Comparing `odp-0.0.6/odp/core/types.py` & `odp-0.0.7/odp/core/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+from datetime import datetime
 from enum import Enum
 
 import click
 from pydantic import BaseModel
 
 
 class QueryRow(BaseModel):
     QUERY_TEXT: str
+    START_TIME: datetime
     DATABASE_NAME: str | None
     SCHEMA_NAME: str | None
 
 
 class SchemaRow(BaseModel):
     TABLE_CATALOG: str
     TABLE_SCHEMA: str
```

### Comparing `odp-0.0.6/pyproject.toml` & `odp-0.0.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "odp"
-version = "0.0.6"
+version = "0.0.7"
 description = "odp"
 authors = ["odp Authors <fdexter@metalytics.dev>"]
 repository = "https://github.com/open-data-products/odp"
 documentation = "https://open-data-products.github.io/odp/"
 readme = "README.md"
 packages = [
   {include = "odp"}
```

### Comparing `odp-0.0.6/PKG-INFO` & `odp-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odp
-Version: 0.0.6
+Version: 0.0.7
 Summary: odp
 Home-page: https://github.com/open-data-products/odp
 Author: odp Authors
 Author-email: fdexter@metalytics.dev
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

