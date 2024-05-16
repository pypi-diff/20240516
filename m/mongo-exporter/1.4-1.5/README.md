# Comparing `tmp/mongo_exporter-1.4.tar.gz` & `tmp/mongo_exporter-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongo_exporter-1.4.tar", last modified: Thu May 16 16:19:39 2024, max compression
+gzip compressed data, was "mongo_exporter-1.5.tar", last modified: Thu May 16 16:26:46 2024, max compression
```

## Comparing `mongo_exporter-1.4.tar` & `mongo_exporter-1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 16:19:39.228738 mongo_exporter-1.4/
--rw-rw-rw-   0        0        0      191 2024-05-16 16:19:39.226739 mongo_exporter-1.4/PKG-INFO
--rw-rw-rw-   0        0        0      985 2024-05-14 15:11:07.000000 mongo_exporter-1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 16:19:39.200733 mongo_exporter-1.4/mongo_exporter/
--rw-rw-rw-   0        0        0       20 2024-05-14 15:14:14.000000 mongo_exporter-1.4/mongo_exporter/__init__.py
--rw-rw-rw-   0        0        0     2064 2024-05-16 16:19:15.000000 mongo_exporter-1.4/mongo_exporter/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-16 16:19:39.220736 mongo_exporter-1.4/mongo_exporter.egg-info/
--rw-rw-rw-   0        0        0      191 2024-05-16 16:19:39.000000 mongo_exporter-1.4/mongo_exporter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2024-05-16 16:19:39.000000 mongo_exporter-1.4/mongo_exporter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 16:19:39.000000 mongo_exporter-1.4/mongo_exporter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-16 16:19:39.000000 mongo_exporter-1.4/mongo_exporter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-16 16:19:39.000000 mongo_exporter-1.4/mongo_exporter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 16:19:39.229739 mongo_exporter-1.4/setup.cfg
--rw-rw-rw-   0        0        0      328 2024-05-16 16:19:23.000000 mongo_exporter-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 16:26:46.699588 mongo_exporter-1.5/
+-rw-rw-rw-   0        0        0      191 2024-05-16 16:26:46.697591 mongo_exporter-1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      985 2024-05-14 15:11:07.000000 mongo_exporter-1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 16:26:46.669580 mongo_exporter-1.5/mongo_exporter/
+-rw-rw-rw-   0        0        0       20 2024-05-14 15:14:14.000000 mongo_exporter-1.5/mongo_exporter/__init__.py
+-rw-rw-rw-   0        0        0     2754 2024-05-16 16:26:27.000000 mongo_exporter-1.5/mongo_exporter/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-16 16:26:46.691586 mongo_exporter-1.5/mongo_exporter.egg-info/
+-rw-rw-rw-   0        0        0      191 2024-05-16 16:26:46.000000 mongo_exporter-1.5/mongo_exporter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2024-05-16 16:26:46.000000 mongo_exporter-1.5/mongo_exporter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 16:26:46.000000 mongo_exporter-1.5/mongo_exporter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-16 16:26:46.000000 mongo_exporter-1.5/mongo_exporter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-16 16:26:46.000000 mongo_exporter-1.5/mongo_exporter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 16:26:46.700581 mongo_exporter-1.5/setup.cfg
+-rw-rw-rw-   0        0        0      328 2024-05-16 16:26:40.000000 mongo_exporter-1.5/setup.py
```

### Comparing `mongo_exporter-1.4/README.md` & `mongo_exporter-1.5/README.md`

 * *Files identical despite different names*

### Comparing `mongo_exporter-1.4/mongo_exporter/tools.py` & `mongo_exporter-1.5/mongo_exporter/tools.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pymongo import MongoClient
+from pymongo import MongoClient,errors
 import json
 
 
 def export_schema(conn_str,db_name):
     """
     Export database schema include indexes and options.
 
@@ -54,14 +54,25 @@
 
     # Load the schema from a file
     with open('schema.json', 'r') as f:
         schema = json.load(f)
 
     # Create each collection with indexes and options
     for collection_name, info in schema.items():
-        collection = db.create_collection(collection_name, **info['options'])
-        indexes = info['indexes']
-        for index in indexes:
-            collection.create_index(**index)
+        try:
+            # Create collection with options
+            collection = db.create_collection(collection_name, **info['options'])
+            print(f"Collection '{collection_name}' created successfully.")
+        except errors.CollectionInvalid:
+            print(f"Collection '{collection_name}' already exists.")
+        
+        for index_name, index_info in info['indexes'].items():
+            index_keys = index_info['key']
+            index_options = {k: v for k, v in index_info.items() if k != 'key'}
+            try:
+                collection.create_index(index_keys, **index_options)
+                print(f"Index '{index_name}' created successfully in collection '{collection_name}'.")
+            except errors.OperationFailure as e:
+                print(f"Error creating index '{index_name}' in collection '{collection_name}': {e}")
 
 if __name__ == "__main__":
     export_schema("mongodb://eatng:%40TczbhNCS5XaQKY%26@172.29.5.205:27017/sessiondb?authSource=sessiondb&readPreference=primary&directConnection=true&ssl=false","sessiondb")
```

