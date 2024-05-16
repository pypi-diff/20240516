# Comparing `tmp/almgroad-0.0.8-py3-none-any.whl.zip` & `tmp/almgroad-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,12 @@
-Zip file size: 23748 bytes, number of entries: 9
--rw-rw----  2.0 unx      105 b- defN 24-May-15 17:41 almgroad/__init__.py
+Zip file size: 24504 bytes, number of entries: 10
+-rw-rw----  2.0 unx      136 b- defN 24-May-16 06:56 almgroad/__init__.py
 -rw-rw----  2.0 unx      182 b- defN 24-May-15 18:03 almgroad/chat.py
+-rw-rw----  2.0 unx     1331 b- defN 24-May-16 06:55 almgroad/info_tik.py
 -rw-rw----  2.0 unx     1071 b- defN 24-May-15 04:51 almgroad/infoinsta.py
 -rw-rw----  2.0 unx    84898 b- defN 24-May-15 18:03 almgroad/ktkt.py
 -rw-rw----  2.0 unx      880 b- defN 24-May-15 18:02 almgroad/tik_tok.py
--rw-rw----  2.0 unx     1434 b- defN 24-May-15 18:04 almgroad-0.0.8.dist-info/METADATA
--rw-rw----  2.0 unx       92 b- defN 24-May-15 18:04 almgroad-0.0.8.dist-info/WHEEL
--rw-rw----  2.0 unx        9 b- defN 24-May-15 18:04 almgroad-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      676 b- defN 24-May-15 18:04 almgroad-0.0.8.dist-info/RECORD
-9 files, 89347 bytes uncompressed, 22594 bytes compressed:  74.7%
+-rw-rw----  2.0 unx     1434 b- defN 24-May-16 06:57 almgroad-0.0.9.dist-info/METADATA
+-rw-rw----  2.0 unx       92 b- defN 24-May-16 06:57 almgroad-0.0.9.dist-info/WHEEL
+-rw-rw----  2.0 unx        9 b- defN 24-May-16 06:57 almgroad-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      753 b- defN 24-May-16 06:57 almgroad-0.0.9.dist-info/RECORD
+10 files, 90786 bytes uncompressed, 23234 bytes compressed:  74.4%
```

## zipnote {}

```diff
@@ -1,28 +1,31 @@
 Filename: almgroad/__init__.py
 Comment: 
 
 Filename: almgroad/chat.py
 Comment: 
 
+Filename: almgroad/info_tik.py
+Comment: 
+
 Filename: almgroad/infoinsta.py
 Comment: 
 
 Filename: almgroad/ktkt.py
 Comment: 
 
 Filename: almgroad/tik_tok.py
 Comment: 
 
-Filename: almgroad-0.0.8.dist-info/METADATA
+Filename: almgroad-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: almgroad-0.0.8.dist-info/WHEEL
+Filename: almgroad-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: almgroad-0.0.8.dist-info/top_level.txt
+Filename: almgroad-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: almgroad-0.0.8.dist-info/RECORD
+Filename: almgroad-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## almgroad/__init__.py

```diff
@@ -1,4 +1,5 @@
 from .infoinsta import Info_Insta
 from .chat import GPT
 from .ktkt import kt
-from .tik_tok import Tik_Tok
+from .tik_tok import Tik_Tok
+from .info_tik import Info_Tik
```

## Comparing `almgroad-0.0.8.dist-info/METADATA` & `almgroad-0.0.9.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: almgroad
-Version: 0.0.8
+Version: 0.0.9
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Ibrahim Mohammed
 Author-email: ibrahom0780@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `almgroad-0.0.8.dist-info/RECORD` & `almgroad-0.0.9.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-almgroad/__init__.py,sha256=BdDcJepjYpi5eGH_-rPbrNsg0p8-GmuPMsfUOYCB3Ag,105
+almgroad/__init__.py,sha256=cnlunCObvYO7WptgahGKdIh_NxSELkqJbRg69toXlRo,136
 almgroad/chat.py,sha256=QOkrkf2gUrcjSstul9hqhPWkTREsasSilv5nMvp_sq4,182
+almgroad/info_tik.py,sha256=dURJKszAIWQPeuHpgVHADcNTz4sTpFWbkxqvwH0RAo4,1331
 almgroad/infoinsta.py,sha256=DzqhmwPWbeBrSXoSZp9DsZQiVC6Nlx8PnZn9wM8sNrM,1071
 almgroad/ktkt.py,sha256=CoUbwbOAd18fMb2fTVPr3BHt81DR43hnSvNuKywcSlU,84898
 almgroad/tik_tok.py,sha256=22laOxfsGV1NhHq7YCQqxl3ZDxIBoGQtP9FSNffgEpI,880
-almgroad-0.0.8.dist-info/METADATA,sha256=mlyCTYRog1xQYi8Eo10LjDZScyieK3cc8JlTudR8_Mo,1434
-almgroad-0.0.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-almgroad-0.0.8.dist-info/top_level.txt,sha256=Sp5hguX1HExRTUrSZFyTESQ8fyBMsW2XsjXu84UhJ-w,9
-almgroad-0.0.8.dist-info/RECORD,,
+almgroad-0.0.9.dist-info/METADATA,sha256=GEUneJkW7TGw1x4lHMcGUeLmdwYhFGSaFMYyNAIlv6A,1434
+almgroad-0.0.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+almgroad-0.0.9.dist-info/top_level.txt,sha256=Sp5hguX1HExRTUrSZFyTESQ8fyBMsW2XsjXu84UhJ-w,9
+almgroad-0.0.9.dist-info/RECORD,,
```

