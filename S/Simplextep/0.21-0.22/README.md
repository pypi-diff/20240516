# Comparing `tmp/Simplextep-0.21-py3-none-any.whl.zip` & `tmp/Simplextep-0.22-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 9556 bytes, number of entries: 7
+Zip file size: 9620 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat    40147 b- defN 24-May-16 08:16 Simplextep/Simplextep.py
--rw-rw-rw-  2.0 fat       52 b- defN 24-May-16 08:27 Simplextep/__init__.py
--rw-rw-rw-  2.0 fat     1090 b- defN 24-May-16 08:27 Simplextep-0.21.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      316 b- defN 24-May-16 08:27 Simplextep-0.21.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-16 08:27 Simplextep-0.21.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 24-May-16 08:27 Simplextep-0.21.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      554 b- defN 24-May-16 08:27 Simplextep-0.21.dist-info/RECORD
-7 files, 42262 bytes uncompressed, 8572 bytes compressed:  79.7%
+-rw-rw-rw-  2.0 fat      162 b- defN 24-May-16 08:35 Simplextep/__init__.py
+-rw-rw-rw-  2.0 fat     1090 b- defN 24-May-16 08:35 Simplextep-0.22.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      316 b- defN 24-May-16 08:35 Simplextep-0.22.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-16 08:35 Simplextep-0.22.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 24-May-16 08:35 Simplextep-0.22.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      555 b- defN 24-May-16 08:35 Simplextep-0.22.dist-info/RECORD
+7 files, 42373 bytes uncompressed, 8636 bytes compressed:  79.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: Simplextep/Simplextep.py
 Comment: 
 
 Filename: Simplextep/__init__.py
 Comment: 
 
-Filename: Simplextep-0.21.dist-info/LICENSE
+Filename: Simplextep-0.22.dist-info/LICENSE
 Comment: 
 
-Filename: Simplextep-0.21.dist-info/METADATA
+Filename: Simplextep-0.22.dist-info/METADATA
 Comment: 
 
-Filename: Simplextep-0.21.dist-info/WHEEL
+Filename: Simplextep-0.22.dist-info/WHEEL
 Comment: 
 
-Filename: Simplextep-0.21.dist-info/top_level.txt
+Filename: Simplextep-0.22.dist-info/top_level.txt
 Comment: 
 
-Filename: Simplextep-0.21.dist-info/RECORD
+Filename: Simplextep-0.22.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Simplextep/__init__.py

```diff
@@ -1,5 +1,7 @@
-import Simplextep.Simplextep as Simplextep
+import Simplextep
+from Simplextep import Simplextep
+from Simplextep.Simplextep import Simplex, Problem_Prepration, Dual, Me_Plot, Sensitivity_Analysis
```

## Comparing `Simplextep-0.21.dist-info/LICENSE` & `Simplextep-0.22.dist-info/LICENSE`

 * *Files identical despite different names*

