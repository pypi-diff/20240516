# Comparing `tmp/Simplextep-0.2-py3-none-any.whl.zip` & `tmp/Simplextep-0.21-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 9538 bytes, number of entries: 7
+Zip file size: 9556 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat    40147 b- defN 24-May-16 08:16 Simplextep/Simplextep.py
--rw-rw-rw-  2.0 fat       24 b- defN 24-May-16 08:07 Simplextep/__init__.py
--rw-rw-rw-  2.0 fat     1090 b- defN 24-May-16 08:19 Simplextep-0.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      315 b- defN 24-May-16 08:19 Simplextep-0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-16 08:19 Simplextep-0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 24-May-16 08:19 Simplextep-0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      549 b- defN 24-May-16 08:19 Simplextep-0.2.dist-info/RECORD
-7 files, 42228 bytes uncompressed, 8564 bytes compressed:  79.7%
+-rw-rw-rw-  2.0 fat       52 b- defN 24-May-16 08:27 Simplextep/__init__.py
+-rw-rw-rw-  2.0 fat     1090 b- defN 24-May-16 08:27 Simplextep-0.21.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      316 b- defN 24-May-16 08:27 Simplextep-0.21.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-16 08:27 Simplextep-0.21.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 24-May-16 08:27 Simplextep-0.21.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      554 b- defN 24-May-16 08:27 Simplextep-0.21.dist-info/RECORD
+7 files, 42262 bytes uncompressed, 8572 bytes compressed:  79.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: Simplextep/Simplextep.py
 Comment: 
 
 Filename: Simplextep/__init__.py
 Comment: 
 
-Filename: Simplextep-0.2.dist-info/LICENSE
+Filename: Simplextep-0.21.dist-info/LICENSE
 Comment: 
 
-Filename: Simplextep-0.2.dist-info/METADATA
+Filename: Simplextep-0.21.dist-info/METADATA
 Comment: 
 
-Filename: Simplextep-0.2.dist-info/WHEEL
+Filename: Simplextep-0.21.dist-info/WHEEL
 Comment: 
 
-Filename: Simplextep-0.2.dist-info/top_level.txt
+Filename: Simplextep-0.21.dist-info/top_level.txt
 Comment: 
 
-Filename: Simplextep-0.2.dist-info/RECORD
+Filename: Simplextep-0.21.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Simplextep/__init__.py

```diff
@@ -1 +1,5 @@
-from Simplextep import *
+import Simplextep.Simplextep as Simplextep
+
+
+
+
```

## Comparing `Simplextep-0.2.dist-info/LICENSE` & `Simplextep-0.21.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `Simplextep-0.2.dist-info/RECORD` & `Simplextep-0.21.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 Simplextep/Simplextep.py,sha256=PqYgAThB7Cw0e54ZrrW9qkgXmtS01R3AO0FCO6cANZ4,40147
-Simplextep/__init__.py,sha256=5cJHsglKKi5MDuXaqoS3Fzb25gAifVQXs6rCe2iNkzU,24
-Simplextep-0.2.dist-info/LICENSE,sha256=b2VoRh9bDRx45zuP3PupJSUhXQs02fsqkTq12Zfvpgw,1090
-Simplextep-0.2.dist-info/METADATA,sha256=kIkGcCP2DsgiRU5tVvNgaOa6yh_-kSOBfB1tqfvcZK4,315
-Simplextep-0.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-Simplextep-0.2.dist-info/top_level.txt,sha256=cjFeBT4iM91GKp3ILfRMRHbovS0crlNrlJjUrqe07lQ,11
-Simplextep-0.2.dist-info/RECORD,,
+Simplextep/__init__.py,sha256=fBIZCjvXBlalyP6YJOM5TIv3tDDd_6YWRFJC-0a6ZMY,52
+Simplextep-0.21.dist-info/LICENSE,sha256=b2VoRh9bDRx45zuP3PupJSUhXQs02fsqkTq12Zfvpgw,1090
+Simplextep-0.21.dist-info/METADATA,sha256=4QP1F5AS--fdu8diCMQZhdeZ1l0x_ZFMz0_lETaKIU0,316
+Simplextep-0.21.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+Simplextep-0.21.dist-info/top_level.txt,sha256=cjFeBT4iM91GKp3ILfRMRHbovS0crlNrlJjUrqe07lQ,11
+Simplextep-0.21.dist-info/RECORD,,
```

