# Comparing `tmp/funcnodes_umap-0.1.0.tar.gz` & `tmp/funcnodes_umap-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcnodes_umap-0.1.0.tar", max compression
+gzip compressed data, was "funcnodes_umap-0.1.1.tar", max compression
```

## Comparing `funcnodes_umap-0.1.0.tar` & `funcnodes_umap-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     3134 2024-05-16 14:02:02.909217 funcnodes_umap-0.1.0/funcnodes_umap/__init__.py
--rw-r--r--   0        0        0      476 2024-05-16 15:04:01.714140 funcnodes_umap-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-24 11:32:57.575895 funcnodes_umap-0.1.0/README.md
--rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 funcnodes_umap-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3291 2024-05-16 15:27:43.057378 funcnodes_umap-0.1.1/funcnodes_umap/__init__.py
+-rw-r--r--   0        0        0      476 2024-05-16 15:27:33.212532 funcnodes_umap-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-24 11:32:57.575895 funcnodes_umap-0.1.1/README.md
+-rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 funcnodes_umap-0.1.1/PKG-INFO
```

### Comparing `funcnodes_umap-0.1.0/funcnodes_umap/__init__.py` & `funcnodes_umap-0.1.1/funcnodes_umap/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -116,7 +116,17 @@
         innerscaler = scaler
 
     if innerscaler:
         data = innerscaler.fit_transform(data)
     embedding = reducer.fit_transform(data)
 
     return embedding, reducer, innerscaler
+
+
+NODE_SHELF = fn.Shelf(
+    name="UMAP",
+    nodes=[reducer, umap_fit_transform],
+    subshelves=[],
+    description="UMAP nodes",
+)
+
+__version__ = "0.1.1"
```

### Comparing `funcnodes_umap-0.1.0/PKG-INFO` & `funcnodes_umap-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcnodes-umap
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Julian Kimmig
 Author-email: julian.kimmig@gmx.net
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

