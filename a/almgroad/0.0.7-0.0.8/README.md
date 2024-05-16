# Comparing `tmp/almgroad-0.0.7-py3-none-any.whl.zip` & `tmp/almgroad-0.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 23581 bytes, number of entries: 9
+Zip file size: 23748 bytes, number of entries: 9
 -rw-rw----  2.0 unx      105 b- defN 24-May-15 17:41 almgroad/__init__.py
--rw-rw----  2.0 unx      128 b- defN 24-May-15 03:17 almgroad/chat.py
+-rw-rw----  2.0 unx      182 b- defN 24-May-15 18:03 almgroad/chat.py
 -rw-rw----  2.0 unx     1071 b- defN 24-May-15 04:51 almgroad/infoinsta.py
--rw-rw----  2.0 unx    84842 b- defN 24-May-15 08:45 almgroad/ktkt.py
--rw-rw----  2.0 unx      829 b- defN 24-May-15 17:40 almgroad/tik_tok.py
--rw-rw----  2.0 unx     1434 b- defN 24-May-15 17:42 almgroad-0.0.7.dist-info/METADATA
--rw-rw----  2.0 unx       92 b- defN 24-May-15 17:42 almgroad-0.0.7.dist-info/WHEEL
--rw-rw----  2.0 unx        9 b- defN 24-May-15 17:42 almgroad-0.0.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      676 b- defN 24-May-15 17:42 almgroad-0.0.7.dist-info/RECORD
-9 files, 89186 bytes uncompressed, 22427 bytes compressed:  74.9%
+-rw-rw----  2.0 unx    84898 b- defN 24-May-15 18:03 almgroad/ktkt.py
+-rw-rw----  2.0 unx      880 b- defN 24-May-15 18:02 almgroad/tik_tok.py
+-rw-rw----  2.0 unx     1434 b- defN 24-May-15 18:04 almgroad-0.0.8.dist-info/METADATA
+-rw-rw----  2.0 unx       92 b- defN 24-May-15 18:04 almgroad-0.0.8.dist-info/WHEEL
+-rw-rw----  2.0 unx        9 b- defN 24-May-15 18:04 almgroad-0.0.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      676 b- defN 24-May-15 18:04 almgroad-0.0.8.dist-info/RECORD
+9 files, 89347 bytes uncompressed, 22594 bytes compressed:  74.7%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: almgroad/ktkt.py
 Comment: 
 
 Filename: almgroad/tik_tok.py
 Comment: 
 
-Filename: almgroad-0.0.7.dist-info/METADATA
+Filename: almgroad-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: almgroad-0.0.7.dist-info/WHEEL
+Filename: almgroad-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: almgroad-0.0.7.dist-info/top_level.txt
+Filename: almgroad-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: almgroad-0.0.7.dist-info/RECORD
+Filename: almgroad-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## almgroad/chat.py

```diff
@@ -1,4 +1,4 @@
 import requests
 def GPT(q):
 	r = requests.get(f"https://chatgpt.apinepdev.workers.dev/?question={q}").json()["answer"]
-	return r
+	return {"answer":r,"PROGRAMMER":"IBRAHIM : TELEGRAM :@q3oooo"}
```

## almgroad/ktkt.py

```diff
@@ -2440,8 +2440,8 @@
             "• كم عدد اللي معطيهم بلوك؟",
 
             "• أجمل سنة ميلادية مرت عليك ؟",
 
             "• أوصف نفسك بكلمة؟",
 ]
 	rand = random.choice(ran)
-	return rand
+	return {"question":rand,"PROGRAMMER":"IBRAHIM : TELEGRAM :@q3oooo"}
```

## almgroad/tik_tok.py

```diff
@@ -14,10 +14,10 @@
     		'user-agent': 'Mozilla/5.0 (Windows NT 6.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/103.0.5060.114 Safari/537.36',
     		'x-requested-with': 'XMLHttpRequest',
     	}
 	data = {
     		'query': url}
 	try:
 		result = requests.post('https://lovetik.com/api/ajax/search', headers=headers, data=data).json()["links"][0]["a"]
-		return result
+		return {"url":result,"PROGRAMMER":"IBRAHIM : TELEGRAM :@q3oooo"}
 	except Exception as e:
 		return f"error : {e}"
```

## Comparing `almgroad-0.0.7.dist-info/METADATA` & `almgroad-0.0.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: almgroad
-Version: 0.0.7
+Version: 0.0.8
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Ibrahim Mohammed
 Author-email: ibrahom0780@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `almgroad-0.0.7.dist-info/RECORD` & `almgroad-0.0.8.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 almgroad/__init__.py,sha256=BdDcJepjYpi5eGH_-rPbrNsg0p8-GmuPMsfUOYCB3Ag,105
-almgroad/chat.py,sha256=hUyCJzd5TaS-x1Y92c9Q5hCFMVnpKKg-nSvysy_KN30,128
+almgroad/chat.py,sha256=QOkrkf2gUrcjSstul9hqhPWkTREsasSilv5nMvp_sq4,182
 almgroad/infoinsta.py,sha256=DzqhmwPWbeBrSXoSZp9DsZQiVC6Nlx8PnZn9wM8sNrM,1071
-almgroad/ktkt.py,sha256=I8OIFV7YRzewNBcxn-ap_32KEbe5oCuq_ghCRwdMLbM,84842
-almgroad/tik_tok.py,sha256=AZif213v-AxlYF2nyToPEp59y3ioMwlQaUim1d5GNUM,829
-almgroad-0.0.7.dist-info/METADATA,sha256=7peefZ2_gIpZBYvYFYuu_UndTXYgpCkWyf7sL9XMaY4,1434
-almgroad-0.0.7.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-almgroad-0.0.7.dist-info/top_level.txt,sha256=Sp5hguX1HExRTUrSZFyTESQ8fyBMsW2XsjXu84UhJ-w,9
-almgroad-0.0.7.dist-info/RECORD,,
+almgroad/ktkt.py,sha256=CoUbwbOAd18fMb2fTVPr3BHt81DR43hnSvNuKywcSlU,84898
+almgroad/tik_tok.py,sha256=22laOxfsGV1NhHq7YCQqxl3ZDxIBoGQtP9FSNffgEpI,880
+almgroad-0.0.8.dist-info/METADATA,sha256=mlyCTYRog1xQYi8Eo10LjDZScyieK3cc8JlTudR8_Mo,1434
+almgroad-0.0.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+almgroad-0.0.8.dist-info/top_level.txt,sha256=Sp5hguX1HExRTUrSZFyTESQ8fyBMsW2XsjXu84UhJ-w,9
+almgroad-0.0.8.dist-info/RECORD,,
```

