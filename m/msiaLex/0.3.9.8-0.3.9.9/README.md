# Comparing `tmp/msiaLex-0.3.9.8-py3-none-any.whl.zip` & `tmp/msiaLex-0.3.9.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,17 @@
-Zip file size: 82493 bytes, number of entries: 12
+Zip file size: 94726 bytes, number of entries: 15
 -rw-rw-r--  2.0 unx    78880 b- defN 23-Apr-07 17:30 data/Emoji_Sentiment_Data_v1.0.csv
 -rw-rw-r--  2.0 unx   296053 b- defN 24-Apr-29 01:56 data/Emoji_Sentiment_Data_v2.0.csv
 -rw-rw-r--  2.0 unx        0 b- defN 22-Jan-06 14:14 data/__init__.py
+-rw-rw-r--  2.0 unx     1735 b- defN 23-Apr-07 17:30 data/emoticon.py
+-rw-rw-r--  2.0 unx    15137 b- defN 23-Apr-07 17:30 data/func.py
+-rw-rw-r--  2.0 unx    39932 b- defN 23-Aug-23 11:06 data/modifier.py
 -rw-rw-r--  2.0 unx        0 b- defN 22-Jan-06 14:14 msiaLex/__init__.py
 -rw-rw-r--  2.0 unx     1735 b- defN 23-Apr-07 17:30 msiaLex/emoticon.py
 -rw-rw-r--  2.0 unx    15137 b- defN 23-Apr-07 17:30 msiaLex/func.py
 -rw-rw-r--  2.0 unx    39932 b- defN 23-Aug-23 11:06 msiaLex/modifier.py
--rw-rw-r--  2.0 unx     1069 b- defN 24-May-15 08:16 msiaLex-0.3.9.8.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx     1334 b- defN 24-May-15 08:16 msiaLex-0.3.9.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-May-15 08:16 msiaLex-0.3.9.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx        5 b- defN 24-May-15 08:16 msiaLex-0.3.9.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      953 b- defN 24-May-15 08:16 msiaLex-0.3.9.8.dist-info/RECORD
-12 files, 435190 bytes uncompressed, 80901 bytes compressed:  81.4%
+-rw-rw-r--  2.0 unx     1069 b- defN 24-May-15 08:28 msiaLex-0.3.9.9.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx     1334 b- defN 24-May-15 08:28 msiaLex-0.3.9.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-15 08:28 msiaLex-0.3.9.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        5 b- defN 24-May-15 08:28 msiaLex-0.3.9.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1170 b- defN 24-May-15 08:28 msiaLex-0.3.9.9.dist-info/RECORD
+15 files, 492211 bytes uncompressed, 92818 bytes compressed:  81.1%
```

## zipnote {}

```diff
@@ -3,35 +3,44 @@
 
 Filename: data/Emoji_Sentiment_Data_v2.0.csv
 Comment: 
 
 Filename: data/__init__.py
 Comment: 
 
+Filename: data/emoticon.py
+Comment: 
+
+Filename: data/func.py
+Comment: 
+
+Filename: data/modifier.py
+Comment: 
+
 Filename: msiaLex/__init__.py
 Comment: 
 
 Filename: msiaLex/emoticon.py
 Comment: 
 
 Filename: msiaLex/func.py
 Comment: 
 
 Filename: msiaLex/modifier.py
 Comment: 
 
-Filename: msiaLex-0.3.9.8.dist-info/LICENSE.txt
+Filename: msiaLex-0.3.9.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: msiaLex-0.3.9.8.dist-info/METADATA
+Filename: msiaLex-0.3.9.9.dist-info/METADATA
 Comment: 
 
-Filename: msiaLex-0.3.9.8.dist-info/WHEEL
+Filename: msiaLex-0.3.9.9.dist-info/WHEEL
 Comment: 
 
-Filename: msiaLex-0.3.9.8.dist-info/top_level.txt
+Filename: msiaLex-0.3.9.9.dist-info/top_level.txt
 Comment: 
 
-Filename: msiaLex-0.3.9.8.dist-info/RECORD
+Filename: msiaLex-0.3.9.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `msiaLex-0.3.9.8.dist-info/LICENSE.txt` & `msiaLex-0.3.9.9.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `msiaLex-0.3.9.8.dist-info/METADATA` & `msiaLex-0.3.9.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msiaLex
-Version: 0.3.9.8
+Version: 0.3.9.9
 Summary: Malaysia Lexicon
 Home-page: https://github.com/yuenkeiwac/msialex
 Author: Khor Yuen Kei
 Author-email: khoryk1104@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

## Comparing `msiaLex-0.3.9.8.dist-info/RECORD` & `msiaLex-0.3.9.9.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 data/Emoji_Sentiment_Data_v1.0.csv,sha256=l0ZdTPfgOf3KP1ZzEKSpwiWqdeGUlFzNt1LfQVrGwgE,78880
 data/Emoji_Sentiment_Data_v2.0.csv,sha256=6ZKbSC35DGeXmx4Rj3BScv4mYhEq9yB2x93FasUn7EM,296053
 data/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+data/emoticon.py,sha256=zWQ_5G5akaoBq07gDCc6XqR2LMVc7G13lEgBkluwues,1735
+data/func.py,sha256=j69fvJkHw6A5magXYZIXOUOFmlCR_iS5MVfhn2AIbus,15137
+data/modifier.py,sha256=QFk2Xz3qSbpndEdSrbhE6qmfchsBpNEp1RymTnv35iU,39932
 msiaLex/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 msiaLex/emoticon.py,sha256=zWQ_5G5akaoBq07gDCc6XqR2LMVc7G13lEgBkluwues,1735
 msiaLex/func.py,sha256=j69fvJkHw6A5magXYZIXOUOFmlCR_iS5MVfhn2AIbus,15137
 msiaLex/modifier.py,sha256=QFk2Xz3qSbpndEdSrbhE6qmfchsBpNEp1RymTnv35iU,39932
-msiaLex-0.3.9.8.dist-info/LICENSE.txt,sha256=IOyL5CMXZVKnPxhRScNF2EGdn45X7CZ0J0FU5uyoX48,1069
-msiaLex-0.3.9.8.dist-info/METADATA,sha256=wi3gTtzV7euL5COdk8upUWm4DwCxrptJC1xpK7p_O14,1334
-msiaLex-0.3.9.8.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-msiaLex-0.3.9.8.dist-info/top_level.txt,sha256=Zmey0aq2oAyqWu5a-K2fFGXlZ6vxwgnRVyfVez6Pbl8,5
-msiaLex-0.3.9.8.dist-info/RECORD,,
+msiaLex-0.3.9.9.dist-info/LICENSE.txt,sha256=IOyL5CMXZVKnPxhRScNF2EGdn45X7CZ0J0FU5uyoX48,1069
+msiaLex-0.3.9.9.dist-info/METADATA,sha256=BSS_iRax1kuu5G7I5YRDKlnFsDJuBWVBaZxDJrHo-3g,1334
+msiaLex-0.3.9.9.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+msiaLex-0.3.9.9.dist-info/top_level.txt,sha256=Zmey0aq2oAyqWu5a-K2fFGXlZ6vxwgnRVyfVez6Pbl8,5
+msiaLex-0.3.9.9.dist-info/RECORD,,
```

