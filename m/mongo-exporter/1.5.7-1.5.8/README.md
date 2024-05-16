# Comparing `tmp/mongo_exporter-1.5.7.tar.gz` & `tmp/mongo_exporter-1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongo_exporter-1.5.7.tar", last modified: Thu May 16 18:10:36 2024, max compression
+gzip compressed data, was "mongo_exporter-1.5.8.tar", last modified: Thu May 16 18:27:10 2024, max compression
```

## Comparing `mongo_exporter-1.5.7.tar` & `mongo_exporter-1.5.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 18:10:36.261131 mongo_exporter-1.5.7/
--rw-rw-rw-   0        0        0      193 2024-05-16 18:10:36.260131 mongo_exporter-1.5.7/PKG-INFO
--rw-rw-rw-   0        0        0      985 2024-05-14 15:11:07.000000 mongo_exporter-1.5.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 18:10:36.228129 mongo_exporter-1.5.7/mongo_exporter/
--rw-rw-rw-   0        0        0       20 2024-05-14 15:14:14.000000 mongo_exporter-1.5.7/mongo_exporter/__init__.py
--rw-rw-rw-   0        0        0     3725 2024-05-16 18:10:17.000000 mongo_exporter-1.5.7/mongo_exporter/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-16 18:10:36.252135 mongo_exporter-1.5.7/mongo_exporter.egg-info/
--rw-rw-rw-   0        0        0      193 2024-05-16 18:10:36.000000 mongo_exporter-1.5.7/mongo_exporter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2024-05-16 18:10:36.000000 mongo_exporter-1.5.7/mongo_exporter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 18:10:36.000000 mongo_exporter-1.5.7/mongo_exporter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-16 18:10:36.000000 mongo_exporter-1.5.7/mongo_exporter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-16 18:10:36.000000 mongo_exporter-1.5.7/mongo_exporter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 18:10:36.263139 mongo_exporter-1.5.7/setup.cfg
--rw-rw-rw-   0        0        0      330 2024-05-16 18:10:27.000000 mongo_exporter-1.5.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 18:27:10.104232 mongo_exporter-1.5.8/
+-rw-rw-rw-   0        0        0      193 2024-05-16 18:27:10.103230 mongo_exporter-1.5.8/PKG-INFO
+-rw-rw-rw-   0        0        0      985 2024-05-14 15:11:07.000000 mongo_exporter-1.5.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 18:27:10.073225 mongo_exporter-1.5.8/mongo_exporter/
+-rw-rw-rw-   0        0        0       20 2024-05-14 15:14:14.000000 mongo_exporter-1.5.8/mongo_exporter/__init__.py
+-rw-rw-rw-   0        0        0     3732 2024-05-16 18:26:46.000000 mongo_exporter-1.5.8/mongo_exporter/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-16 18:27:10.097228 mongo_exporter-1.5.8/mongo_exporter.egg-info/
+-rw-rw-rw-   0        0        0      193 2024-05-16 18:27:09.000000 mongo_exporter-1.5.8/mongo_exporter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2024-05-16 18:27:09.000000 mongo_exporter-1.5.8/mongo_exporter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 18:27:09.000000 mongo_exporter-1.5.8/mongo_exporter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-16 18:27:09.000000 mongo_exporter-1.5.8/mongo_exporter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-16 18:27:09.000000 mongo_exporter-1.5.8/mongo_exporter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 18:27:10.106232 mongo_exporter-1.5.8/setup.cfg
+-rw-rw-rw-   0        0        0      330 2024-05-16 18:25:54.000000 mongo_exporter-1.5.8/setup.py
```

### Comparing `mongo_exporter-1.5.7/README.md` & `mongo_exporter-1.5.8/README.md`

 * *Files identical despite different names*

### Comparing `mongo_exporter-1.5.7/mongo_exporter/tools.py` & `mongo_exporter-1.5.8/mongo_exporter/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,17 @@
 
     # Load the schema from a file
     with open('schema.json', 'r') as f:
         schema = json.load(f)
 
     # Create each collection with indexes and options
     for collection_name, info in schema.items():
+        if collection_name.startswith("system."):
+            continue
+
         try:
             # Create collection with options
             collection = db.create_collection(collection_name, **info['options'])
             print(f"Collection '{collection_name}' created successfully.")
         except errors.CollectionInvalid:
             collection = db.get_collection(collection_name)
             print(f"Collection '{collection_name}' already exists.")
@@ -81,15 +84,14 @@
 
             for field, specifier in index_keys:
                 if specifier not in [1, -1, '2d', '2dsphere', 'text', 'hashed']:
                     raise ValueError(f"Invalid index specifier '{specifier}' for field '{field}' in index '{index_name}' of collection '{collection_name}'.")
             
             index_options = {k: v for k, v in index_info.items() if k not in ['key', 'ns', 'v']}
             try:
-                print(f"Index '{index_name}' keys '{index_keys}'")
                 collection.create_index(index_keys, name=index_name, **index_options)
                 print(f"Index '{index_name}' created successfully in collection '{collection_name}'.")
             except errors.OperationFailure as e:
                 print(f"Error creating index '{index_name}' in collection '{collection_name}': {e}")
 
 if __name__ == "__main__":
     export_schema("mongodb://eatng:%40TczbhNCS5XaQKY%26@172.29.5.205:27017/sessiondb?authSource=sessiondb&readPreference=primary&directConnection=true&ssl=false","sessiondb")
```

