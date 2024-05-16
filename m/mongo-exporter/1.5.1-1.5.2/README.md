# Comparing `tmp/mongo_exporter-1.5.1.tar.gz` & `tmp/mongo_exporter-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongo_exporter-1.5.1.tar", last modified: Thu May 16 16:33:42 2024, max compression
+gzip compressed data, was "mongo_exporter-1.5.2.tar", last modified: Thu May 16 16:43:03 2024, max compression
```

## Comparing `mongo_exporter-1.5.1.tar` & `mongo_exporter-1.5.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 16:33:42.551607 mongo_exporter-1.5.1/
--rw-rw-rw-   0        0        0      193 2024-05-16 16:33:42.549599 mongo_exporter-1.5.1/PKG-INFO
--rw-rw-rw-   0        0        0      985 2024-05-14 15:11:07.000000 mongo_exporter-1.5.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 16:33:42.502593 mongo_exporter-1.5.1/mongo_exporter/
--rw-rw-rw-   0        0        0       20 2024-05-14 15:14:14.000000 mongo_exporter-1.5.1/mongo_exporter/__init__.py
--rw-rw-rw-   0        0        0     2815 2024-05-16 16:32:45.000000 mongo_exporter-1.5.1/mongo_exporter/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-16 16:33:42.541600 mongo_exporter-1.5.1/mongo_exporter.egg-info/
--rw-rw-rw-   0        0        0      193 2024-05-16 16:33:42.000000 mongo_exporter-1.5.1/mongo_exporter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2024-05-16 16:33:42.000000 mongo_exporter-1.5.1/mongo_exporter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 16:33:42.000000 mongo_exporter-1.5.1/mongo_exporter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-16 16:33:42.000000 mongo_exporter-1.5.1/mongo_exporter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-16 16:33:42.000000 mongo_exporter-1.5.1/mongo_exporter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 16:33:42.553600 mongo_exporter-1.5.1/setup.cfg
--rw-rw-rw-   0        0        0      330 2024-05-16 16:33:32.000000 mongo_exporter-1.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 16:43:03.917925 mongo_exporter-1.5.2/
+-rw-rw-rw-   0        0        0      193 2024-05-16 16:43:03.916927 mongo_exporter-1.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0      985 2024-05-14 15:11:07.000000 mongo_exporter-1.5.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 16:43:03.884928 mongo_exporter-1.5.2/mongo_exporter/
+-rw-rw-rw-   0        0        0       20 2024-05-14 15:14:14.000000 mongo_exporter-1.5.2/mongo_exporter/__init__.py
+-rw-rw-rw-   0        0        0     2837 2024-05-16 16:42:43.000000 mongo_exporter-1.5.2/mongo_exporter/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-16 16:43:03.909923 mongo_exporter-1.5.2/mongo_exporter.egg-info/
+-rw-rw-rw-   0        0        0      193 2024-05-16 16:43:03.000000 mongo_exporter-1.5.2/mongo_exporter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2024-05-16 16:43:03.000000 mongo_exporter-1.5.2/mongo_exporter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 16:43:03.000000 mongo_exporter-1.5.2/mongo_exporter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-16 16:43:03.000000 mongo_exporter-1.5.2/mongo_exporter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-16 16:43:03.000000 mongo_exporter-1.5.2/mongo_exporter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 16:43:03.919929 mongo_exporter-1.5.2/setup.cfg
+-rw-rw-rw-   0        0        0      330 2024-05-16 16:42:51.000000 mongo_exporter-1.5.2/setup.py
```

### Comparing `mongo_exporter-1.5.1/README.md` & `mongo_exporter-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `mongo_exporter-1.5.1/mongo_exporter/tools.py` & `mongo_exporter-1.5.2/mongo_exporter/tools.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         collection = db[collection_name]
         index_info = collection.index_information()
         if '_id_' in index_info:
             # Remove the default _id_ index to reduce schema size
             del index_info['_id_']
         schema[collection_name] = {
             'indexes': index_info,
-            'options': collection.options(),
+            'options': db.command("collstats", collection_name).get('options', {}),
         }
 
     # Save the schema to a file
     with open('schema.json', 'w') as f:
         f.write(json.dumps(schema))
 
 
@@ -59,17 +59,18 @@
     # Create each collection with indexes and options
     for collection_name, info in schema.items():
         try:
             # Create collection with options
             collection = db.create_collection(collection_name, **info['options'])
             print(f"Collection '{collection_name}' created successfully.")
         except errors.CollectionInvalid:
-            collection = db.get_collection(collection_name)
             print(f"Collection '{collection_name}' already exists.")
         
+        collection = db[collection_name]
+
         for index_name, index_info in info['indexes'].items():
             index_keys = index_info['key']
             index_options = {k: v for k, v in index_info.items() if k != 'key'}
             try:
                 collection.create_index(index_keys, **index_options)
                 print(f"Index '{index_name}' created successfully in collection '{collection_name}'.")
             except errors.OperationFailure as e:
```

