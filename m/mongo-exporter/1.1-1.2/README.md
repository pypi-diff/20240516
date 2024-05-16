# Comparing `tmp/mongo_exporter-1.1.tar.gz` & `tmp/mongo_exporter-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongo_exporter-1.1.tar", last modified: Wed Mar 15 21:07:53 2023, max compression
+gzip compressed data, was "mongo_exporter-1.2.tar", last modified: Thu May 16 15:53:36 2024, max compression
```

## Comparing `mongo_exporter-1.1.tar` & `mongo_exporter-1.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-03-15 21:07:53.961275 mongo_exporter-1.1/
--rw-rw-rw-   0        0        0      191 2023-03-15 21:07:53.959278 mongo_exporter-1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-15 21:07:53.921279 mongo_exporter-1.1/mongo_exporter/
--rw-rw-rw-   0        0        0       20 2023-03-15 21:03:53.000000 mongo_exporter-1.1/mongo_exporter/__init__.py
--rw-rw-rw-   0        0        0     1800 2023-03-15 20:01:21.000000 mongo_exporter-1.1/mongo_exporter/tools.py
-drwxrwxrwx   0        0        0        0 2023-03-15 21:07:53.953276 mongo_exporter-1.1/mongo_exporter.egg-info/
--rw-rw-rw-   0        0        0      191 2023-03-15 21:07:53.000000 mongo_exporter-1.1/mongo_exporter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2023-03-15 21:07:53.000000 mongo_exporter-1.1/mongo_exporter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-15 21:07:53.000000 mongo_exporter-1.1/mongo_exporter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-03-15 21:07:53.000000 mongo_exporter-1.1/mongo_exporter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-03-15 21:07:53.000000 mongo_exporter-1.1/mongo_exporter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-15 21:07:53.962281 mongo_exporter-1.1/setup.cfg
--rw-rw-rw-   0        0        0      328 2023-03-15 21:07:39.000000 mongo_exporter-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 15:53:36.984686 mongo_exporter-1.2/
+-rw-rw-rw-   0        0        0      191 2024-05-16 15:53:36.981700 mongo_exporter-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      985 2024-05-14 15:11:07.000000 mongo_exporter-1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 15:53:36.943678 mongo_exporter-1.2/mongo_exporter/
+-rw-rw-rw-   0        0        0       20 2024-05-14 15:14:14.000000 mongo_exporter-1.2/mongo_exporter/__init__.py
+-rw-rw-rw-   0        0        0     2064 2024-05-16 15:22:12.000000 mongo_exporter-1.2/mongo_exporter/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-16 15:53:36.973687 mongo_exporter-1.2/mongo_exporter.egg-info/
+-rw-rw-rw-   0        0        0      191 2024-05-16 15:53:36.000000 mongo_exporter-1.2/mongo_exporter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2024-05-16 15:53:36.000000 mongo_exporter-1.2/mongo_exporter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 15:53:36.000000 mongo_exporter-1.2/mongo_exporter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-16 15:53:36.000000 mongo_exporter-1.2/mongo_exporter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-16 15:53:36.000000 mongo_exporter-1.2/mongo_exporter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 15:53:36.985684 mongo_exporter-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      328 2024-05-16 15:24:01.000000 mongo_exporter-1.2/setup.py
```

### Comparing `mongo_exporter-1.1/mongo_exporter/tools.py` & `mongo_exporter-1.2/mongo_exporter/tools.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,8 +55,13 @@
     # Load the schema from a file
     with open('schema.json', 'r') as f:
         schema = json.load(f)
 
     # Create each collection with indexes and options
     for collection_name, info in schema.items():
         collection = db.create_collection(collection_name, **info['options'])
-        collection.create_indexes(info['indexes'])
+        indexes = info['indexes']
+        for index in indexes:
+            collection.create_index(**index)
+
+if __name__ == "__main__":
+    export_schema("mongodb://eatng:%40TczbhNCS5XaQKY%26@172.29.5.205:27017/sessiondb?authSource=sessiondb&readPreference=primary&directConnection=true&ssl=false","sessiondb")
```

