# Comparing `tmp/tdrpa.tdworker-1.1.4.8-py3-none-any.whl.zip` & `tmp/tdrpa.tdworker-1.1.4.9-py39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 430899 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat  1213952 b- defN 24-May-16 02:27 tdrpa/tdworker.cp38-win_amd64.pyd
+Zip file size: 428143 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat  1212928 b- defN 24-May-16 14:52 tdrpa/tdworker.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat      167 b- defN 24-May-16 02:23 tdrpa/tdworker/__init__.pyi
 -rw-rw-rw-  2.0 fat     4254 b- defN 24-May-16 02:23 tdrpa/tdworker/_w.pyi
 -rw-rw-rw-  2.0 fat    17361 b- defN 24-May-16 02:23 tdrpa/tdworker/_winE.pyi
 -rw-rw-rw-  2.0 fat     5395 b- defN 24-May-16 02:23 tdrpa/tdworker/_winK.pyi
 -rw-rw-rw-  2.0 fat     7908 b- defN 24-May-16 02:23 tdrpa/tdworker/_winM.pyi
--rw-rw-rw-  2.0 fat      663 b- defN 24-May-16 02:27 tdrpa.tdworker-1.1.4.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-16 02:27 tdrpa.tdworker-1.1.4.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 24-May-16 02:27 tdrpa.tdworker-1.1.4.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      830 b- defN 24-May-16 02:27 tdrpa.tdworker-1.1.4.8.dist-info/RECORD
-10 files, 1250628 bytes uncompressed, 429483 bytes compressed:  65.7%
+-rw-rw-rw-  2.0 fat      667 b- defN 24-May-16 14:52 tdrpa.tdworker-1.1.4.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-16 14:52 tdrpa.tdworker-1.1.4.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 24-May-16 14:52 tdrpa.tdworker-1.1.4.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      830 b- defN 24-May-16 14:52 tdrpa.tdworker-1.1.4.9.dist-info/RECORD
+10 files, 1249608 bytes uncompressed, 426727 bytes compressed:  65.9%
```

## zipnote {}

```diff
@@ -1,8 +1,8 @@
-Filename: tdrpa/tdworker.cp38-win_amd64.pyd
+Filename: tdrpa/tdworker.cp39-win_amd64.pyd
 Comment: 
 
 Filename: tdrpa/tdworker/__init__.pyi
 Comment: 
 
 Filename: tdrpa/tdworker/_w.pyi
 Comment: 
@@ -12,20 +12,20 @@
 
 Filename: tdrpa/tdworker/_winK.pyi
 Comment: 
 
 Filename: tdrpa/tdworker/_winM.pyi
 Comment: 
 
-Filename: tdrpa.tdworker-1.1.4.8.dist-info/METADATA
+Filename: tdrpa.tdworker-1.1.4.9.dist-info/METADATA
 Comment: 
 
-Filename: tdrpa.tdworker-1.1.4.8.dist-info/WHEEL
+Filename: tdrpa.tdworker-1.1.4.9.dist-info/WHEEL
 Comment: 
 
-Filename: tdrpa.tdworker-1.1.4.8.dist-info/top_level.txt
+Filename: tdrpa.tdworker-1.1.4.9.dist-info/top_level.txt
 Comment: 
 
-Filename: tdrpa.tdworker-1.1.4.8.dist-info/RECORD
+Filename: tdrpa.tdworker-1.1.4.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `tdrpa.tdworker-1.1.4.8.dist-info/METADATA` & `tdrpa.tdworker-1.1.4.9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdrpa.tdworker
-Version: 1.1.4.8
+Version: 1.1.4.9
 Summary: tdworker for tdrpa developers. supports python3.8+, windows x64
 Home-page: https://tdrpa.thingswell.cn
 Author: vx:RPA_CREATOR
 Author-email: oldplayerliu@gmail.com
 License: Apache 2.0
 Keywords: RPA,tdRPA,tdworker,rpaworker,worker,uiautomation,uia,creator,windows,python,bot,robot,aigc,ai
 Platform: Windows Only
@@ -12,7 +12,9 @@
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Dist: tdrpa.tdcore
 Requires-Dist: pyperclip
 Requires-Dist: WMI
 Requires-Dist: pycryptodome
 
 tdworker for tdrpa developers. supports python3.8+, windows x64
+
+
```

## Comparing `tdrpa.tdworker-1.1.4.8.dist-info/RECORD` & `tdrpa.tdworker-1.1.4.9.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-tdrpa/tdworker.cp38-win_amd64.pyd,sha256=W7Bv_RmiEHS-VPAAHR2l_l4PrkzTFyXEwkRosqvy-vw,1213952
+tdrpa/tdworker.cp39-win_amd64.pyd,sha256=MDnt8Ui_TFr-0-b2qUnLfSvGg8L61_Bgn4vVKh6r5E0,1212928
 tdrpa/tdworker/__init__.pyi,sha256=sGWR5Le0SWyHPKV5mYz_zRxr8X7zIQSF9cqOB8YUcnE,167
 tdrpa/tdworker/_w.pyi,sha256=ZXgV35kxk0kjX2mHu2vL_TnB3_5bGkacQJbnglNsRtE,4254
 tdrpa/tdworker/_winE.pyi,sha256=a2zzqjlm1HoOrZa-plIsaCKaVujz0QuC2F8H-dbv-i4,17361
 tdrpa/tdworker/_winK.pyi,sha256=22vDxBqR9ZdiUFjbtW-SZVZA2h44cOfbOZ3oX9SrDjk,5395
 tdrpa/tdworker/_winM.pyi,sha256=ifh5EvOjNCsOzsfIYvRbpyAWA1FU5lzlEPkGPbfuQgE,7908
-tdrpa.tdworker-1.1.4.8.dist-info/METADATA,sha256=4FQG-VbtWCrZFbnjh-aAj5FaG89tmDjjXygi16_iJFM,663
-tdrpa.tdworker-1.1.4.8.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-tdrpa.tdworker-1.1.4.8.dist-info/top_level.txt,sha256=S9UoqmC_cyGqKbGsBkLQPEeQLbDrWD0SRwbxPpQpyyU,6
-tdrpa.tdworker-1.1.4.8.dist-info/RECORD,,
+tdrpa.tdworker-1.1.4.9.dist-info/METADATA,sha256=0dlbVo8EP8w_bm1166QpaEHriiVAushaAVgb4bY04xM,667
+tdrpa.tdworker-1.1.4.9.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+tdrpa.tdworker-1.1.4.9.dist-info/top_level.txt,sha256=S9UoqmC_cyGqKbGsBkLQPEeQLbDrWD0SRwbxPpQpyyU,6
+tdrpa.tdworker-1.1.4.9.dist-info/RECORD,,
```

