# Comparing `tmp/mongo_exporter-1.5.9.tar.gz` & `tmp/mongo_exporter-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongo_exporter-1.5.9.tar", last modified: Thu May 16 18:35:53 2024, max compression
+gzip compressed data, was "mongo_exporter-1.6.0.tar", last modified: Thu May 16 18:51:59 2024, max compression
```

## Comparing `mongo_exporter-1.5.9.tar` & `mongo_exporter-1.6.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 18:35:53.054507 mongo_exporter-1.5.9/
--rw-rw-rw-   0        0        0      193 2024-05-16 18:35:53.053516 mongo_exporter-1.5.9/PKG-INFO
--rw-rw-rw-   0        0        0      985 2024-05-14 15:11:07.000000 mongo_exporter-1.5.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 18:35:53.021504 mongo_exporter-1.5.9/mongo_exporter/
--rw-rw-rw-   0        0        0       20 2024-05-14 15:14:14.000000 mongo_exporter-1.5.9/mongo_exporter/__init__.py
--rw-rw-rw-   0        0        0     3814 2024-05-16 18:34:10.000000 mongo_exporter-1.5.9/mongo_exporter/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-16 18:35:53.046503 mongo_exporter-1.5.9/mongo_exporter.egg-info/
--rw-rw-rw-   0        0        0      193 2024-05-16 18:35:52.000000 mongo_exporter-1.5.9/mongo_exporter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2024-05-16 18:35:52.000000 mongo_exporter-1.5.9/mongo_exporter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 18:35:52.000000 mongo_exporter-1.5.9/mongo_exporter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-16 18:35:52.000000 mongo_exporter-1.5.9/mongo_exporter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-16 18:35:52.000000 mongo_exporter-1.5.9/mongo_exporter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 18:35:53.056509 mongo_exporter-1.5.9/setup.cfg
--rw-rw-rw-   0        0        0      330 2024-05-16 18:35:41.000000 mongo_exporter-1.5.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 18:51:59.124663 mongo_exporter-1.6.0/
+-rw-rw-rw-   0        0        0      193 2024-05-16 18:51:59.122663 mongo_exporter-1.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0      985 2024-05-14 15:11:07.000000 mongo_exporter-1.6.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 18:51:59.094657 mongo_exporter-1.6.0/mongo_exporter/
+-rw-rw-rw-   0        0        0       20 2024-05-14 15:14:14.000000 mongo_exporter-1.6.0/mongo_exporter/__init__.py
+-rw-rw-rw-   0        0        0     3797 2024-05-16 18:46:55.000000 mongo_exporter-1.6.0/mongo_exporter/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-16 18:51:59.115666 mongo_exporter-1.6.0/mongo_exporter.egg-info/
+-rw-rw-rw-   0        0        0      193 2024-05-16 18:51:58.000000 mongo_exporter-1.6.0/mongo_exporter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2024-05-16 18:51:58.000000 mongo_exporter-1.6.0/mongo_exporter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 18:51:58.000000 mongo_exporter-1.6.0/mongo_exporter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-16 18:51:58.000000 mongo_exporter-1.6.0/mongo_exporter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-16 18:51:58.000000 mongo_exporter-1.6.0/mongo_exporter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 18:51:59.126664 mongo_exporter-1.6.0/setup.cfg
+-rw-rw-rw-   0        0        0      330 2024-05-16 18:51:53.000000 mongo_exporter-1.6.0/setup.py
```

### Comparing `mongo_exporter-1.5.9/README.md` & `mongo_exporter-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `mongo_exporter-1.5.9/mongo_exporter/tools.py` & `mongo_exporter-1.6.0/mongo_exporter/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,16 +61,17 @@
 
     # Load the schema from a file
     with open('schema.json', 'r') as f:
         schema = json.load(f)
 
     # Create each collection with indexes and options
     for collection_name, info in schema.items():
-        print(f"'{collection_name}' | '{collection_name.startswith("system.")}")
+        print(f"'{collection_name}'")
         if collection_name.startswith("system."):
+            print(f"Ok")
             continue
 
         try:
             # Create collection with options
             collection = db.create_collection(collection_name, **info['options'])
             print(f"Collection '{collection_name}' created successfully.")
         except errors.CollectionInvalid:
```

