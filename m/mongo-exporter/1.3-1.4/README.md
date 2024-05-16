# Comparing `tmp/mongo_exporter-1.3.tar.gz` & `tmp/mongo_exporter-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongo_exporter-1.3.tar", last modified: Thu May 16 16:11:56 2024, max compression
+gzip compressed data, was "mongo_exporter-1.4.tar", last modified: Thu May 16 16:19:39 2024, max compression
```

## Comparing `mongo_exporter-1.3.tar` & `mongo_exporter-1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 16:11:56.845839 mongo_exporter-1.3/
--rw-rw-rw-   0        0        0      191 2024-05-16 16:11:56.843838 mongo_exporter-1.3/PKG-INFO
--rw-rw-rw-   0        0        0      985 2024-05-14 15:11:07.000000 mongo_exporter-1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 16:11:56.807834 mongo_exporter-1.3/mongo_exporter/
--rw-rw-rw-   0        0        0       20 2024-05-14 15:14:14.000000 mongo_exporter-1.3/mongo_exporter/__init__.py
--rw-rw-rw-   0        0        0     2922 2024-05-16 16:11:16.000000 mongo_exporter-1.3/mongo_exporter/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-16 16:11:56.834838 mongo_exporter-1.3/mongo_exporter.egg-info/
--rw-rw-rw-   0        0        0      191 2024-05-16 16:11:56.000000 mongo_exporter-1.3/mongo_exporter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2024-05-16 16:11:56.000000 mongo_exporter-1.3/mongo_exporter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 16:11:56.000000 mongo_exporter-1.3/mongo_exporter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-16 16:11:56.000000 mongo_exporter-1.3/mongo_exporter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-16 16:11:56.000000 mongo_exporter-1.3/mongo_exporter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 16:11:56.848841 mongo_exporter-1.3/setup.cfg
--rw-rw-rw-   0        0        0      328 2024-05-16 16:11:41.000000 mongo_exporter-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 16:19:39.228738 mongo_exporter-1.4/
+-rw-rw-rw-   0        0        0      191 2024-05-16 16:19:39.226739 mongo_exporter-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      985 2024-05-14 15:11:07.000000 mongo_exporter-1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 16:19:39.200733 mongo_exporter-1.4/mongo_exporter/
+-rw-rw-rw-   0        0        0       20 2024-05-14 15:14:14.000000 mongo_exporter-1.4/mongo_exporter/__init__.py
+-rw-rw-rw-   0        0        0     2064 2024-05-16 16:19:15.000000 mongo_exporter-1.4/mongo_exporter/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-16 16:19:39.220736 mongo_exporter-1.4/mongo_exporter.egg-info/
+-rw-rw-rw-   0        0        0      191 2024-05-16 16:19:39.000000 mongo_exporter-1.4/mongo_exporter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2024-05-16 16:19:39.000000 mongo_exporter-1.4/mongo_exporter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 16:19:39.000000 mongo_exporter-1.4/mongo_exporter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-16 16:19:39.000000 mongo_exporter-1.4/mongo_exporter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-16 16:19:39.000000 mongo_exporter-1.4/mongo_exporter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 16:19:39.229739 mongo_exporter-1.4/setup.cfg
+-rw-rw-rw-   0        0        0      328 2024-05-16 16:19:23.000000 mongo_exporter-1.4/setup.py
```

### Comparing `mongo_exporter-1.3/README.md` & `mongo_exporter-1.4/README.md`

 * *Files identical despite different names*

### Comparing `mongo_exporter-1.3/mongo_exporter/tools.py` & `mongo_exporter-1.4/mongo_exporter/tools.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+from pymongo import MongoClient
 import json
-from pymongo import MongoClient, errors
 
-def export_schema(conn_str, db_name):
+
+def export_schema(conn_str,db_name):
     """
-    Export database schema including indexes and options.
+    Export database schema include indexes and options.
 
     Args:
         conn_str (string): connection string.
-        db_name (string): database name.
+        db_name (string): data base name.
 
     Returns:
-        json file: saves the schema to a schema.json file.
+        json file: save the schema to a schema.json file.
     """
+
     # Connect to MongoDB
     client = MongoClient(conn_str)
 
     # Select the database to export the schema from
     db = client[db_name]
 
     # Get the schema of the database including indexes
@@ -24,57 +26,42 @@
         collection = db[collection_name]
         index_info = collection.index_information()
         if '_id_' in index_info:
             # Remove the default _id_ index to reduce schema size
             del index_info['_id_']
         schema[collection_name] = {
             'indexes': index_info,
-            'options': db.command("collstats", collection_name).get('options', {}),
+            'options': collection.options(),
         }
 
     # Save the schema to a file
     with open('schema.json', 'w') as f:
-        json.dump(schema, f, indent=4)
+        f.write(json.dumps(schema))
+
 
-def import_schema(conn_str, db_name):
+def import_schema(conn_str,db_name):
     """
-    Import database schema including indexes and options.
+    Import database schema include indexes and options.
 
     Args:
         conn_str (string): connection string.
-        db_name (string): database name.
+        db_name (string): data base name.
     """
     # Connect to MongoDB
     client = MongoClient(conn_str)
 
     # Select the database to import the schema to
     db = client[db_name]
 
     # Load the schema from a file
     with open('schema.json', 'r') as f:
         schema = json.load(f)
 
     # Create each collection with indexes and options
     for collection_name, info in schema.items():
-        try:
-            # Create collection with options
-            db.create_collection(collection_name, **info['options'])
-            print(f"Collection '{collection_name}' created successfully.")
-        except errors.CollectionInvalid:
-            print(f"Collection '{collection_name}' already exists.")
-        
-        collection = db[collection_name]
-        
-        # Create indexes
-        for index_name, index_info in info['indexes'].items():
-            index_keys = index_info['key']
-            index_options = {k: v for k, v in index_info.items() if k != 'key'}
-            try:
-                collection.create_index(index_keys, **index_options)
-                print(f"Index '{index_name}' created successfully in collection '{collection_name}'.")
-            except errors.OperationFailure as e:
-                print(f"Error creating index '{index_name}' in collection '{collection_name}': {e}")
-
-        print("Collections and indexes setup completed.")
+        collection = db.create_collection(collection_name, **info['options'])
+        indexes = info['indexes']
+        for index in indexes:
+            collection.create_index(**index)
 
 if __name__ == "__main__":
     export_schema("mongodb://eatng:%40TczbhNCS5XaQKY%26@172.29.5.205:27017/sessiondb?authSource=sessiondb&readPreference=primary&directConnection=true&ssl=false","sessiondb")
```

