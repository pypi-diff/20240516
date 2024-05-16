# Comparing `tmp/mongo_exporter-1.6.0.tar.gz` & `tmp/mongo_exporter-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongo_exporter-1.6.0.tar", last modified: Thu May 16 18:51:59 2024, max compression
+gzip compressed data, was "mongo_exporter-1.6.1.tar", last modified: Thu May 16 18:58:26 2024, max compression
```

## Comparing `mongo_exporter-1.6.0.tar` & `mongo_exporter-1.6.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 18:51:59.124663 mongo_exporter-1.6.0/
--rw-rw-rw-   0        0        0      193 2024-05-16 18:51:59.122663 mongo_exporter-1.6.0/PKG-INFO
--rw-rw-rw-   0        0        0      985 2024-05-14 15:11:07.000000 mongo_exporter-1.6.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 18:51:59.094657 mongo_exporter-1.6.0/mongo_exporter/
--rw-rw-rw-   0        0        0       20 2024-05-14 15:14:14.000000 mongo_exporter-1.6.0/mongo_exporter/__init__.py
--rw-rw-rw-   0        0        0     3797 2024-05-16 18:46:55.000000 mongo_exporter-1.6.0/mongo_exporter/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-16 18:51:59.115666 mongo_exporter-1.6.0/mongo_exporter.egg-info/
--rw-rw-rw-   0        0        0      193 2024-05-16 18:51:58.000000 mongo_exporter-1.6.0/mongo_exporter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2024-05-16 18:51:58.000000 mongo_exporter-1.6.0/mongo_exporter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 18:51:58.000000 mongo_exporter-1.6.0/mongo_exporter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-16 18:51:58.000000 mongo_exporter-1.6.0/mongo_exporter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-16 18:51:58.000000 mongo_exporter-1.6.0/mongo_exporter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 18:51:59.126664 mongo_exporter-1.6.0/setup.cfg
--rw-rw-rw-   0        0        0      330 2024-05-16 18:51:53.000000 mongo_exporter-1.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 18:58:26.898066 mongo_exporter-1.6.1/
+-rw-rw-rw-   0        0        0      193 2024-05-16 18:58:26.896057 mongo_exporter-1.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0      985 2024-05-14 15:11:07.000000 mongo_exporter-1.6.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 18:58:26.867061 mongo_exporter-1.6.1/mongo_exporter/
+-rw-rw-rw-   0        0        0       20 2024-05-14 15:14:14.000000 mongo_exporter-1.6.1/mongo_exporter/__init__.py
+-rw-rw-rw-   0        0        0     3370 2024-05-16 18:58:04.000000 mongo_exporter-1.6.1/mongo_exporter/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-16 18:58:26.889061 mongo_exporter-1.6.1/mongo_exporter.egg-info/
+-rw-rw-rw-   0        0        0      193 2024-05-16 18:58:26.000000 mongo_exporter-1.6.1/mongo_exporter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2024-05-16 18:58:26.000000 mongo_exporter-1.6.1/mongo_exporter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 18:58:26.000000 mongo_exporter-1.6.1/mongo_exporter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-16 18:58:26.000000 mongo_exporter-1.6.1/mongo_exporter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-16 18:58:26.000000 mongo_exporter-1.6.1/mongo_exporter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 18:58:26.900064 mongo_exporter-1.6.1/setup.cfg
+-rw-rw-rw-   0        0        0      330 2024-05-16 18:58:16.000000 mongo_exporter-1.6.1/setup.py
```

### Comparing `mongo_exporter-1.6.0/README.md` & `mongo_exporter-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `mongo_exporter-1.6.0/mongo_exporter/tools.py` & `mongo_exporter-1.6.1/mongo_exporter/tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,37 +61,29 @@
 
     # Load the schema from a file
     with open('schema.json', 'r') as f:
         schema = json.load(f)
 
     # Create each collection with indexes and options
     for collection_name, info in schema.items():
-        print(f"'{collection_name}'")
         if collection_name.startswith("system."):
-            print(f"Ok")
             continue
 
         try:
             # Create collection with options
             collection = db.create_collection(collection_name, **info['options'])
             print(f"Collection '{collection_name}' created successfully.")
         except errors.CollectionInvalid:
             collection = db.get_collection(collection_name)
             print(f"Collection '{collection_name}' already exists.")
         
         collection = db[collection_name]
         
         for index_name, index_info in info['indexes'].items():
             index_keys = index_keys = [(field, int(specifier) if specifier in [1, -1] else specifier) for field, specifier in index_info['key']]
-            #[tuple(key) for key in index_info['key']]
-
-            for field, specifier in index_keys:
-                if specifier not in [1, -1, '2d', '2dsphere', 'text', 'hashed']:
-                    raise ValueError(f"Invalid index specifier '{specifier}' for field '{field}' in index '{index_name}' of collection '{collection_name}'.")
-            
             index_options = {k: v for k, v in index_info.items() if k not in ['key', 'ns', 'v']}
             try:
                 collection.create_index(index_keys, name=index_name, **index_options)
                 print(f"Index '{index_name}' created successfully in collection '{collection_name}'.")
             except errors.OperationFailure as e:
                 print(f"Error creating index '{index_name}' in collection '{collection_name}': {e}")
```

