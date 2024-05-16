# Comparing `tmp/easyntp-0.0.0-py3-none-any.whl.zip` & `tmp/easyntp-0.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 1831 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat      832 b- defN 24-May-16 09:04 easyntp/__init__.py
--rw-rw-rw-  2.0 fat      753 b- defN 24-May-16 09:06 easyntp-0.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-16 09:06 easyntp-0.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 24-May-16 09:06 easyntp-0.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      371 b- defN 24-May-16 09:06 easyntp-0.0.0.dist-info/RECORD
-5 files, 2056 bytes uncompressed, 1135 bytes compressed:  44.8%
+Zip file size: 1829 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat      832 b- defN 24-May-16 09:07 easyntp/__init__.py
+-rw-rw-rw-  2.0 fat      727 b- defN 24-May-16 09:08 easyntp-0.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-16 09:08 easyntp-0.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 24-May-16 09:08 easyntp-0.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      371 b- defN 24-May-16 09:08 easyntp-0.0.1.dist-info/RECORD
+5 files, 2030 bytes uncompressed, 1133 bytes compressed:  44.2%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: easyntp/__init__.py
 Comment: 
 
-Filename: easyntp-0.0.0.dist-info/METADATA
+Filename: easyntp-0.0.1.dist-info/METADATA
 Comment: 
 
-Filename: easyntp-0.0.0.dist-info/WHEEL
+Filename: easyntp-0.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: easyntp-0.0.0.dist-info/top_level.txt
+Filename: easyntp-0.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: easyntp-0.0.0.dist-info/RECORD
+Filename: easyntp-0.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## easyntp/__init__.py

```diff
@@ -1,14 +1,14 @@
 import datetime
 from time import ctime
 import sys
 import ntplib
 
 __copyright__    = 'Copyright (C) 2024 JavaCommons Technologies'
-__version__      = '0.0.0'
+__version__      = '0.0.1'
 __license__      = 'MIT'
 __author__       = 'JavaCommons Technologies'
 __author_email__ = 'javacommmons@gmail.com'
 __url__          = 'https://github.com/lang-library/py-easyntp'
 __all__ = ['EasyNTPClient']
```

## Comparing `easyntp-0.0.0.dist-info/METADATA` & `easyntp-0.0.1.dist-info/METADATA`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyntp
-Version: 0.0.0
+Version: 0.0.1
 Summary: Easy NTP library
 Home-page: https://github.com/lang-library/py-easyntp
 Author: JavaCommons Technologies
 Author-email: javacommmons@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -12,32 +12,19 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 Requires-Dist: ntplib
 
 # py-easyntp
 
-
-
 ```
-
 from easyntp import *
 
-
-
 ntp_client = EasyNTPClient()
-
 print(ntp_client.now())
-
 print(ntp_client.format_now('%Y/%m/%d'))
 
-
-
 """
-
 2024-05-16 18:03:10
-
 2024/05/16
-
 """
-
 ```
```

