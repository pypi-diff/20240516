# Comparing `tmp/gwml-0.0.8-py3-none-any.whl.zip` & `tmp/gwml-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,11 @@
-Zip file size: 1858 bytes, number of entries: 7
--rw-r--r--  2.0 unx       22 b- defN 24-May-14 09:26 gwml/__init__.py
+Zip file size: 2299 bytes, number of entries: 9
+-rw-r--r--  2.0 unx       22 b- defN 24-May-14 09:31 gwml/__init__.py
 -rw-r--r--  2.0 unx      125 b- defN 24-May-08 00:38 gwml/example.py
--rw-r--r--  2.0 unx       28 b- defN 24-May-14 09:26 gwml-0.0.8.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      645 b- defN 24-May-14 09:26 gwml-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-14 09:26 gwml-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 24-May-14 09:26 gwml-0.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      513 b- defN 24-May-14 09:26 gwml-0.0.8.dist-info/RECORD
-7 files, 1430 bytes uncompressed, 946 bytes compressed:  33.8%
+-rw-r--r--  2.0 unx       22 b- defN 24-May-14 09:31 gwml/lib/__init__.py
+-rw-r--r--  2.0 unx      167 b- defN 24-May-14 09:16 gwml/lib/example.py
+-rw-r--r--  2.0 unx       28 b- defN 24-May-14 09:31 gwml-0.0.9.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      645 b- defN 24-May-14 09:31 gwml-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-14 09:31 gwml-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 24-May-14 09:31 gwml-0.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      663 b- defN 24-May-14 09:31 gwml-0.0.9.dist-info/RECORD
+9 files, 1769 bytes uncompressed, 1157 bytes compressed:  34.6%
```

## zipnote {}

```diff
@@ -1,22 +1,28 @@
 Filename: gwml/__init__.py
 Comment: 
 
 Filename: gwml/example.py
 Comment: 
 
-Filename: gwml-0.0.8.dist-info/LICENSE.txt
+Filename: gwml/lib/__init__.py
 Comment: 
 
-Filename: gwml-0.0.8.dist-info/METADATA
+Filename: gwml/lib/example.py
 Comment: 
 
-Filename: gwml-0.0.8.dist-info/WHEEL
+Filename: gwml-0.0.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: gwml-0.0.8.dist-info/top_level.txt
+Filename: gwml-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: gwml-0.0.8.dist-info/RECORD
+Filename: gwml-0.0.9.dist-info/WHEEL
+Comment: 
+
+Filename: gwml-0.0.9.dist-info/top_level.txt
+Comment: 
+
+Filename: gwml-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gwml/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "0.0.8"
+__version__ = "0.0.9"
```

## Comparing `gwml-0.0.8.dist-info/METADATA` & `gwml-0.0.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwml
-Version: 0.0.8
+Version: 0.0.9
 Summary: PYPI tutorial package creation written by TeddyNote
 Home-page: https://weda.kr
 Author: weda
 Author-email: dmshin@weda.kr
 Keywords: gw,weda,greenwhales,ml,dl,automl
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

