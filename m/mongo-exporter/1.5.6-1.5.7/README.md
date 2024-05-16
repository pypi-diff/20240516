# Comparing `tmp/mongo_exporter-1.5.6.tar.gz` & `tmp/mongo_exporter-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongo_exporter-1.5.6.tar", last modified: Thu May 16 17:57:29 2024, max compression
+gzip compressed data, was "mongo_exporter-1.5.7.tar", last modified: Thu May 16 18:10:36 2024, max compression
```

## Comparing `mongo_exporter-1.5.6.tar` & `mongo_exporter-1.5.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 17:57:29.390854 mongo_exporter-1.5.6/
--rw-rw-rw-   0        0        0      193 2024-05-16 17:57:29.388857 mongo_exporter-1.5.6/PKG-INFO
--rw-rw-rw-   0        0        0      985 2024-05-14 15:11:07.000000 mongo_exporter-1.5.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 17:57:29.358854 mongo_exporter-1.5.6/mongo_exporter/
--rw-rw-rw-   0        0        0       20 2024-05-14 15:14:14.000000 mongo_exporter-1.5.6/mongo_exporter/__init__.py
--rw-rw-rw-   0        0        0     3591 2024-05-16 17:57:04.000000 mongo_exporter-1.5.6/mongo_exporter/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-16 17:57:29.382861 mongo_exporter-1.5.6/mongo_exporter.egg-info/
--rw-rw-rw-   0        0        0      193 2024-05-16 17:57:29.000000 mongo_exporter-1.5.6/mongo_exporter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2024-05-16 17:57:29.000000 mongo_exporter-1.5.6/mongo_exporter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 17:57:29.000000 mongo_exporter-1.5.6/mongo_exporter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-16 17:57:29.000000 mongo_exporter-1.5.6/mongo_exporter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-16 17:57:29.000000 mongo_exporter-1.5.6/mongo_exporter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 17:57:29.391857 mongo_exporter-1.5.6/setup.cfg
--rw-rw-rw-   0        0        0      330 2024-05-16 17:57:13.000000 mongo_exporter-1.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 18:10:36.261131 mongo_exporter-1.5.7/
+-rw-rw-rw-   0        0        0      193 2024-05-16 18:10:36.260131 mongo_exporter-1.5.7/PKG-INFO
+-rw-rw-rw-   0        0        0      985 2024-05-14 15:11:07.000000 mongo_exporter-1.5.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 18:10:36.228129 mongo_exporter-1.5.7/mongo_exporter/
+-rw-rw-rw-   0        0        0       20 2024-05-14 15:14:14.000000 mongo_exporter-1.5.7/mongo_exporter/__init__.py
+-rw-rw-rw-   0        0        0     3725 2024-05-16 18:10:17.000000 mongo_exporter-1.5.7/mongo_exporter/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-16 18:10:36.252135 mongo_exporter-1.5.7/mongo_exporter.egg-info/
+-rw-rw-rw-   0        0        0      193 2024-05-16 18:10:36.000000 mongo_exporter-1.5.7/mongo_exporter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2024-05-16 18:10:36.000000 mongo_exporter-1.5.7/mongo_exporter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 18:10:36.000000 mongo_exporter-1.5.7/mongo_exporter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-16 18:10:36.000000 mongo_exporter-1.5.7/mongo_exporter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-16 18:10:36.000000 mongo_exporter-1.5.7/mongo_exporter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 18:10:36.263139 mongo_exporter-1.5.7/setup.cfg
+-rw-rw-rw-   0        0        0      330 2024-05-16 18:10:27.000000 mongo_exporter-1.5.7/setup.py
```

### Comparing `mongo_exporter-1.5.6/README.md` & `mongo_exporter-1.5.7/README.md`

 * *Files identical despite different names*

### Comparing `mongo_exporter-1.5.6/mongo_exporter/tools.py` & `mongo_exporter-1.5.7/mongo_exporter/tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,15 +72,16 @@
         except errors.CollectionInvalid:
             collection = db.get_collection(collection_name)
             print(f"Collection '{collection_name}' already exists.")
         
         collection = db[collection_name]
         
         for index_name, index_info in info['indexes'].items():
-            index_keys = [tuple(key) for key in index_info['key']]
+            index_keys = index_keys = [(field, int(specifier) if specifier in [1, -1] else specifier) for field, specifier in index_info['key']]
+            #[tuple(key) for key in index_info['key']]
 
             for field, specifier in index_keys:
                 if specifier not in [1, -1, '2d', '2dsphere', 'text', 'hashed']:
                     raise ValueError(f"Invalid index specifier '{specifier}' for field '{field}' in index '{index_name}' of collection '{collection_name}'.")
             
             index_options = {k: v for k, v in index_info.items() if k not in ['key', 'ns', 'v']}
             try:
```

