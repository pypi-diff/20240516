# Comparing `tmp/mongo_exporter-1.5.4.tar.gz` & `tmp/mongo_exporter-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongo_exporter-1.5.4.tar", last modified: Thu May 16 17:28:59 2024, max compression
+gzip compressed data, was "mongo_exporter-1.5.5.tar", last modified: Thu May 16 17:47:27 2024, max compression
```

## Comparing `mongo_exporter-1.5.4.tar` & `mongo_exporter-1.5.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 17:28:59.865408 mongo_exporter-1.5.4/
--rw-rw-rw-   0        0        0      193 2024-05-16 17:28:59.863407 mongo_exporter-1.5.4/PKG-INFO
--rw-rw-rw-   0        0        0      985 2024-05-14 15:11:07.000000 mongo_exporter-1.5.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 17:28:59.832407 mongo_exporter-1.5.4/mongo_exporter/
--rw-rw-rw-   0        0        0       20 2024-05-14 15:14:14.000000 mongo_exporter-1.5.4/mongo_exporter/__init__.py
--rw-rw-rw-   0        0        0     3200 2024-05-16 17:28:41.000000 mongo_exporter-1.5.4/mongo_exporter/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-16 17:28:59.856406 mongo_exporter-1.5.4/mongo_exporter.egg-info/
--rw-rw-rw-   0        0        0      193 2024-05-16 17:28:59.000000 mongo_exporter-1.5.4/mongo_exporter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2024-05-16 17:28:59.000000 mongo_exporter-1.5.4/mongo_exporter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 17:28:59.000000 mongo_exporter-1.5.4/mongo_exporter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-16 17:28:59.000000 mongo_exporter-1.5.4/mongo_exporter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-16 17:28:59.000000 mongo_exporter-1.5.4/mongo_exporter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 17:28:59.867415 mongo_exporter-1.5.4/setup.cfg
--rw-rw-rw-   0        0        0      330 2024-05-16 17:28:48.000000 mongo_exporter-1.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 17:47:27.941054 mongo_exporter-1.5.5/
+-rw-rw-rw-   0        0        0      193 2024-05-16 17:47:27.939060 mongo_exporter-1.5.5/PKG-INFO
+-rw-rw-rw-   0        0        0      985 2024-05-14 15:11:07.000000 mongo_exporter-1.5.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 17:47:27.911051 mongo_exporter-1.5.5/mongo_exporter/
+-rw-rw-rw-   0        0        0       20 2024-05-14 15:14:14.000000 mongo_exporter-1.5.5/mongo_exporter/__init__.py
+-rw-rw-rw-   0        0        0     3523 2024-05-16 17:47:07.000000 mongo_exporter-1.5.5/mongo_exporter/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-16 17:47:27.933055 mongo_exporter-1.5.5/mongo_exporter.egg-info/
+-rw-rw-rw-   0        0        0      193 2024-05-16 17:47:27.000000 mongo_exporter-1.5.5/mongo_exporter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2024-05-16 17:47:27.000000 mongo_exporter-1.5.5/mongo_exporter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 17:47:27.000000 mongo_exporter-1.5.5/mongo_exporter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-16 17:47:27.000000 mongo_exporter-1.5.5/mongo_exporter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-16 17:47:27.000000 mongo_exporter-1.5.5/mongo_exporter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 17:47:27.943054 mongo_exporter-1.5.5/setup.cfg
+-rw-rw-rw-   0        0        0      330 2024-05-16 17:47:22.000000 mongo_exporter-1.5.5/setup.py
```

### Comparing `mongo_exporter-1.5.4/README.md` & `mongo_exporter-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `mongo_exporter-1.5.4/mongo_exporter/tools.py` & `mongo_exporter-1.5.5/mongo_exporter/tools.py`

 * *Files 13% similar despite different names*

```diff
@@ -73,16 +73,21 @@
             collection = db.get_collection(collection_name)
             print(f"Collection '{collection_name}' already exists.")
         
         collection = db[collection_name]
         
         for index_name, index_info in info['indexes'].items():
             index_keys = [tuple(key) for key in index_info['key']]
+
+            for field, specifier in index_keys:
+                if specifier not in [1, -1, '2d', '2dsphere', 'text', 'hashed']:
+                    raise ValueError(f"Invalid index specifier '{specifier}' for field '{field}' in index '{index_name}' of collection '{collection_name}'.")
+            
             index_options = {k: v for k, v in index_info.items() if k not in ['key', 'ns', 'v']}
             try:
-                collection.create_index(index_keys, **index_options)
+                collection.create_index(index_keys, name=index_name, **index_options)
                 print(f"Index '{index_name}' created successfully in collection '{collection_name}'.")
             except errors.OperationFailure as e:
                 print(f"Error creating index '{index_name}' in collection '{collection_name}': {e}")
 
 if __name__ == "__main__":
     export_schema("mongodb://eatng:%40TczbhNCS5XaQKY%26@172.29.5.205:27017/sessiondb?authSource=sessiondb&readPreference=primary&directConnection=true&ssl=false","sessiondb")
```

