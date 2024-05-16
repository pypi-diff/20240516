# Comparing `tmp/mongo_exporter-1.5.3.tar.gz` & `tmp/mongo_exporter-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongo_exporter-1.5.3.tar", last modified: Thu May 16 16:51:03 2024, max compression
+gzip compressed data, was "mongo_exporter-1.5.4.tar", last modified: Thu May 16 17:28:59 2024, max compression
```

## Comparing `mongo_exporter-1.5.3.tar` & `mongo_exporter-1.5.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 16:51:03.749707 mongo_exporter-1.5.3/
--rw-rw-rw-   0        0        0      193 2024-05-16 16:51:03.748707 mongo_exporter-1.5.3/PKG-INFO
--rw-rw-rw-   0        0        0      985 2024-05-14 15:11:07.000000 mongo_exporter-1.5.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 16:51:03.719703 mongo_exporter-1.5.3/mongo_exporter/
--rw-rw-rw-   0        0        0       20 2024-05-14 15:14:14.000000 mongo_exporter-1.5.3/mongo_exporter/__init__.py
--rw-rw-rw-   0        0        0     3159 2024-05-16 16:50:38.000000 mongo_exporter-1.5.3/mongo_exporter/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-16 16:51:03.741706 mongo_exporter-1.5.3/mongo_exporter.egg-info/
--rw-rw-rw-   0        0        0      193 2024-05-16 16:51:03.000000 mongo_exporter-1.5.3/mongo_exporter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2024-05-16 16:51:03.000000 mongo_exporter-1.5.3/mongo_exporter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 16:51:03.000000 mongo_exporter-1.5.3/mongo_exporter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-16 16:51:03.000000 mongo_exporter-1.5.3/mongo_exporter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-16 16:51:03.000000 mongo_exporter-1.5.3/mongo_exporter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 16:51:03.750707 mongo_exporter-1.5.3/setup.cfg
--rw-rw-rw-   0        0        0      330 2024-05-16 16:50:57.000000 mongo_exporter-1.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 17:28:59.865408 mongo_exporter-1.5.4/
+-rw-rw-rw-   0        0        0      193 2024-05-16 17:28:59.863407 mongo_exporter-1.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0      985 2024-05-14 15:11:07.000000 mongo_exporter-1.5.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 17:28:59.832407 mongo_exporter-1.5.4/mongo_exporter/
+-rw-rw-rw-   0        0        0       20 2024-05-14 15:14:14.000000 mongo_exporter-1.5.4/mongo_exporter/__init__.py
+-rw-rw-rw-   0        0        0     3200 2024-05-16 17:28:41.000000 mongo_exporter-1.5.4/mongo_exporter/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-16 17:28:59.856406 mongo_exporter-1.5.4/mongo_exporter.egg-info/
+-rw-rw-rw-   0        0        0      193 2024-05-16 17:28:59.000000 mongo_exporter-1.5.4/mongo_exporter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2024-05-16 17:28:59.000000 mongo_exporter-1.5.4/mongo_exporter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 17:28:59.000000 mongo_exporter-1.5.4/mongo_exporter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-16 17:28:59.000000 mongo_exporter-1.5.4/mongo_exporter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-16 17:28:59.000000 mongo_exporter-1.5.4/mongo_exporter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 17:28:59.867415 mongo_exporter-1.5.4/setup.cfg
+-rw-rw-rw-   0        0        0      330 2024-05-16 17:28:48.000000 mongo_exporter-1.5.4/setup.py
```

### Comparing `mongo_exporter-1.5.3/README.md` & `mongo_exporter-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `mongo_exporter-1.5.3/mongo_exporter/tools.py` & `mongo_exporter-1.5.4/mongo_exporter/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,16 +72,16 @@
         except errors.CollectionInvalid:
             collection = db.get_collection(collection_name)
             print(f"Collection '{collection_name}' already exists.")
         
         collection = db[collection_name]
         
         for index_name, index_info in info['indexes'].items():
-            index_keys = index_info['key']
-            index_options = {k: v for k, v in index_info.items() if k != 'key'}
+            index_keys = [tuple(key) for key in index_info['key']]
+            index_options = {k: v for k, v in index_info.items() if k not in ['key', 'ns', 'v']}
             try:
                 collection.create_index(index_keys, **index_options)
                 print(f"Index '{index_name}' created successfully in collection '{collection_name}'.")
             except errors.OperationFailure as e:
                 print(f"Error creating index '{index_name}' in collection '{collection_name}': {e}")
 
 if __name__ == "__main__":
```

