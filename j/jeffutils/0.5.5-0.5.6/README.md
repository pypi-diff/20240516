# Comparing `tmp/jeffutils-0.5.5.tar.gz` & `tmp/jeffutils-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeffutils-0.5.5.tar", last modified: Wed May 15 16:58:49 2024, max compression
+gzip compressed data, was "jeffutils-0.5.6.tar", last modified: Wed May 15 19:00:20 2024, max compression
```

## Comparing `jeffutils-0.5.5.tar` & `jeffutils-0.5.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-15 16:58:49.214716 jeffutils-0.5.5/
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     1070 2024-03-16 21:55:37.000000 jeffutils-0.5.5/LICENSE.txt
--rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-05-15 16:58:49.210716 jeffutils-0.5.5/PKG-INFO
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       12 2024-03-16 21:29:21.000000 jeffutils-0.5.5/README.md
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       84 2024-03-16 21:54:38.000000 jeffutils-0.5.5/pyproject.toml
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       38 2024-05-15 16:58:49.214716 jeffutils-0.5.5/setup.cfg
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      559 2024-05-15 16:58:45.000000 jeffutils-0.5.5/setup.py
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-15 16:58:49.210716 jeffutils-0.5.5/src/
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-15 16:58:49.210716 jeffutils-0.5.5/src/jeffutils/
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        0 2024-03-16 21:50:41.000000 jeffutils-0.5.5/src/jeffutils/__init__.py
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)    21865 2024-05-15 16:46:43.000000 jeffutils-0.5.5/src/jeffutils/utils.py
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-15 16:58:49.210716 jeffutils-0.5.5/src/jeffutils.egg-info/
--rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-05-15 16:58:49.000000 jeffutils-0.5.5/src/jeffutils.egg-info/PKG-INFO
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      242 2024-05-15 16:58:49.000000 jeffutils-0.5.5/src/jeffutils.egg-info/SOURCES.txt
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        1 2024-05-15 16:58:49.000000 jeffutils-0.5.5/src/jeffutils.egg-info/dependency_links.txt
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       10 2024-05-15 16:58:49.000000 jeffutils-0.5.5/src/jeffutils.egg-info/top_level.txt
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-15 19:00:20.659960 jeffutils-0.5.6/
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     1070 2024-03-16 21:55:37.000000 jeffutils-0.5.6/LICENSE.txt
+-rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-05-15 19:00:20.659960 jeffutils-0.5.6/PKG-INFO
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       12 2024-03-16 21:29:21.000000 jeffutils-0.5.6/README.md
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       84 2024-03-16 21:54:38.000000 jeffutils-0.5.6/pyproject.toml
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       38 2024-05-15 19:00:20.659960 jeffutils-0.5.6/setup.cfg
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      559 2024-05-15 19:00:16.000000 jeffutils-0.5.6/setup.py
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-15 19:00:20.659960 jeffutils-0.5.6/src/
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-15 19:00:20.659960 jeffutils-0.5.6/src/jeffutils/
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        0 2024-03-16 21:50:41.000000 jeffutils-0.5.6/src/jeffutils/__init__.py
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)    22577 2024-05-15 18:59:55.000000 jeffutils-0.5.6/src/jeffutils/utils.py
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-15 19:00:20.659960 jeffutils-0.5.6/src/jeffutils.egg-info/
+-rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-05-15 19:00:20.000000 jeffutils-0.5.6/src/jeffutils.egg-info/PKG-INFO
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      242 2024-05-15 19:00:20.000000 jeffutils-0.5.6/src/jeffutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        1 2024-05-15 19:00:20.000000 jeffutils-0.5.6/src/jeffutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       10 2024-05-15 19:00:20.000000 jeffutils-0.5.6/src/jeffutils.egg-info/top_level.txt
```

### Comparing `jeffutils-0.5.5/LICENSE.txt` & `jeffutils-0.5.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jeffutils-0.5.5/setup.py` & `jeffutils-0.5.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='jeffutils',
-    version='0.5.5',
+    version='0.5.6',
     author='Jeff Hansen',
     author_email='jeffxhansen@gmail.com',
     description='A series of useful functions and decorators I use in most of my projects. Feel free to use them as well :)',
     package_dir={"": "src"},
     packages = find_packages(where="src"),
     classifiers=[
         'Programming Language :: Python :: 3',
```

### Comparing `jeffutils-0.5.5/src/jeffutils/utils.py` & `jeffutils-0.5.6/src/jeffutils/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -637,7 +637,29 @@
             )
             res_df = pd.read_sql_query(query, conn)
     finally:
         conn.close()
         
     return res_df
 
+def get_sql_table_as_df(db_path, table_name):
+    """ Get the table as a pandas DataFrame
+    
+    Args:
+    db_path (str): The path to the database file
+    table_name (str): The name of the table
+    
+    Returns:
+    pd.DataFrame: The table as a DataFrame
+    """
+    # validate the input
+    if not os.path.exists(db_path):
+        raise FileNotFoundError(f"Database file {db_path} does not exist")
+    if not db_path.endswith(".db"):
+        raise ValueError(f"Table name {table_name} should end with .db")
+    
+    # get the table as a DataFrame
+    try:
+        with sql.connect(db_path) as conn:
+            return pd.read_sql_query(f"SELECT * FROM {table_name}", conn)
+    finally:
+        conn.close()
```

