# Comparing `tmp/cryptoadvance.spectrum-0.6.6-py3-none-any.whl.zip` & `tmp/cryptoadvance.spectrum-0.6.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
-Zip file size: 38649 bytes, number of entries: 21
+Zip file size: 38688 bytes, number of entries: 21
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-27 10:47 cryptoadvance/spectrum/__init__.py
 -rw-r--r--  2.0 unx       90 b- defN 23-Apr-27 10:47 cryptoadvance/spectrum/__main__.py
--rw-r--r--  2.0 unx      411 b- defN 24-May-15 15:46 cryptoadvance/spectrum/_version.py
+-rw-r--r--  2.0 unx      411 b- defN 24-May-16 16:30 cryptoadvance/spectrum/_version.py
 -rw-r--r--  2.0 unx     2714 b- defN 23-Apr-27 10:47 cryptoadvance/spectrum/config.py
 -rw-r--r--  2.0 unx     9098 b- defN 23-Apr-27 10:47 cryptoadvance/spectrum/db.py
--rw-r--r--  2.0 unx    25701 b- defN 24-May-15 15:38 cryptoadvance/spectrum/elsock.py
+-rw-r--r--  2.0 unx    25814 b- defN 24-May-16 16:29 cryptoadvance/spectrum/elsock.py
 -rw-r--r--  2.0 unx     2584 b- defN 23-Apr-27 10:47 cryptoadvance/spectrum/server.py
 -rw-r--r--  2.0 unx    50876 b- defN 24-May-15 15:38 cryptoadvance/spectrum/spectrum.py
 -rw-r--r--  2.0 unx      336 b- defN 24-May-15 15:38 cryptoadvance/spectrum/spectrum_error.py
 -rw-r--r--  2.0 unx     3563 b- defN 23-Apr-27 10:47 cryptoadvance/spectrum/util.py
 -rw-r--r--  2.0 unx    11056 b- defN 23-Apr-27 10:47 cryptoadvance/spectrum/util_specter.py
 -rw-r--r--  2.0 unx     1602 b- defN 23-Apr-27 10:47 cryptoadvance/spectrum/cli/__init__.py
 -rw-r--r--  2.0 unx      931 b- defN 23-Apr-27 10:47 cryptoadvance/spectrum/cli/cli_server.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-27 10:47 cryptoadvance/spectrum/server_endpoints/__init__.py
 -rw-r--r--  2.0 unx     1123 b- defN 23-Apr-27 10:47 cryptoadvance/spectrum/server_endpoints/core_api.py
 -rw-r--r--  2.0 unx      578 b- defN 23-Apr-27 10:47 cryptoadvance/spectrum/server_endpoints/healthz.py
--rw-r--r--  2.0 unx     1073 b- defN 24-May-15 15:46 cryptoadvance.spectrum-0.6.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     4631 b- defN 24-May-15 15:46 cryptoadvance.spectrum-0.6.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-15 15:46 cryptoadvance.spectrum-0.6.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 24-May-15 15:46 cryptoadvance.spectrum-0.6.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1962 b- defN 24-May-15 15:46 cryptoadvance.spectrum-0.6.6.dist-info/RECORD
-21 files, 118435 bytes uncompressed, 35367 bytes compressed:  70.1%
+-rw-r--r--  2.0 unx     1073 b- defN 24-May-16 16:30 cryptoadvance.spectrum-0.6.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4631 b- defN 24-May-16 16:30 cryptoadvance.spectrum-0.6.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-16 16:30 cryptoadvance.spectrum-0.6.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 24-May-16 16:30 cryptoadvance.spectrum-0.6.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1962 b- defN 24-May-16 16:30 cryptoadvance.spectrum-0.6.7.dist-info/RECORD
+21 files, 118548 bytes uncompressed, 35406 bytes compressed:  70.1%
```

## zipnote {}

```diff
@@ -42,23 +42,23 @@
 
 Filename: cryptoadvance/spectrum/server_endpoints/core_api.py
 Comment: 
 
 Filename: cryptoadvance/spectrum/server_endpoints/healthz.py
 Comment: 
 
-Filename: cryptoadvance.spectrum-0.6.6.dist-info/LICENSE
+Filename: cryptoadvance.spectrum-0.6.7.dist-info/LICENSE
 Comment: 
 
-Filename: cryptoadvance.spectrum-0.6.6.dist-info/METADATA
+Filename: cryptoadvance.spectrum-0.6.7.dist-info/METADATA
 Comment: 
 
-Filename: cryptoadvance.spectrum-0.6.6.dist-info/WHEEL
+Filename: cryptoadvance.spectrum-0.6.7.dist-info/WHEEL
 Comment: 
 
-Filename: cryptoadvance.spectrum-0.6.6.dist-info/top_level.txt
+Filename: cryptoadvance.spectrum-0.6.7.dist-info/top_level.txt
 Comment: 
 
-Filename: cryptoadvance.spectrum-0.6.6.dist-info/RECORD
+Filename: cryptoadvance.spectrum-0.6.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cryptoadvance/spectrum/_version.py

```diff
@@ -8,9 +8,9 @@
     VERSION_TUPLE = object
 
 version: str
 __version__: str
 __version_tuple__: VERSION_TUPLE
 version_tuple: VERSION_TUPLE
 
-__version__ = version = '0.6.6'
-__version_tuple__ = version_tuple = (0, 6, 6)
+__version__ = version = '0.6.7'
+__version_tuple__ = version_tuple = (0, 6, 7)
```

## cryptoadvance/spectrum/elsock.py

```diff
@@ -555,21 +555,23 @@
             # time.sleep(1)
             time.sleep(0.01)
             if time.time() - start > self._call_timeout:
                 raise ElSockTimeoutException(
                     f"Timeout in call ({self._call_timeout} seconds) waiting for {method} on {self._socket}"
                 )
         res = self._results.pop(uid)
-        if "error" in res:
-            if "code" in res["error"] and "message" in res["error"]:
-                raise RPCError(res["error"]["message"], res["error"]["code"])
-            else:
-                raise SpectrumInternalException(res)
+        if isinstance(res, dict) and "error" in res:
+            error = res.get("error", {})
+            error_code = error.get("code")
+            error_message = error.get("message")
+            if error_code is not None and error_message is not None:
+                raise RPCError(error_message, error_code)
         if "result" in res:
             return res["result"]
+        raise SpectrumInternalException(res)
 
     def ping(self):
         start = time.time()
         self.call("server.ping")  # result None
         return time.time() - start
 
     def __del__(self):
```

## Comparing `cryptoadvance.spectrum-0.6.6.dist-info/LICENSE` & `cryptoadvance.spectrum-0.6.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cryptoadvance.spectrum-0.6.6.dist-info/METADATA` & `cryptoadvance.spectrum-0.6.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptoadvance.spectrum
-Version: 0.6.6
+Version: 0.6.7
 Summary: Implements A Bitcoin Core API which querying an Electrum
 Author: Stepan Snigirev, k9ert
 License: MIT License
         
         Copyright (c) 2023 specter.solutions
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

## Comparing `cryptoadvance.spectrum-0.6.6.dist-info/RECORD` & `cryptoadvance.spectrum-0.6.7.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 cryptoadvance/spectrum/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cryptoadvance/spectrum/__main__.py,sha256=ua1ZBtaBN4Npybshup8KeBF3-x3GIAZf4sTEb-QfxfE,90
-cryptoadvance/spectrum/_version.py,sha256=A5NOPsDJAvtNjXOWXcGEBcGThUtYnfklnJHouP0KaiU,411
+cryptoadvance/spectrum/_version.py,sha256=iLXz9haw4jSV4Xm2-5_V8999GBAYoJkXg9-YOwMJpLY,411
 cryptoadvance/spectrum/config.py,sha256=2lex_4qt2v1qnRbPM-EMGkuUEgzSrO0x_82D2qTNd60,2714
 cryptoadvance/spectrum/db.py,sha256=kZULtBJTAW-eYzazQAMoyT90IVAcGy1lU6Bgs-nRoBo,9098
-cryptoadvance/spectrum/elsock.py,sha256=R3AORBOEC2p1bJmmjPWQfjFYnM-XEFMa4ZsZTfFmWVw,25701
+cryptoadvance/spectrum/elsock.py,sha256=S8qzsZr-qP1v-WKhjsuzHezEk6bA7CnFLKPsV9C_DTA,25814
 cryptoadvance/spectrum/server.py,sha256=g9gmlYzaPlqHGuIQRaQ00ZPrnE7GKkpyUf0ikZT9Qo0,2584
 cryptoadvance/spectrum/spectrum.py,sha256=HyKhT5GXFHPd7z7SEYZCGgW5dg9BFXQIMIx9biOKoPM,50876
 cryptoadvance/spectrum/spectrum_error.py,sha256=rg3dL_TerwiV18YjVfD0xJacl-6RCFgubkJtObIImsg,336
 cryptoadvance/spectrum/util.py,sha256=sT_3Qo0xUZVrYQhYigSQZzdvNfp_3yIHjdWcEOkCbZY,3563
 cryptoadvance/spectrum/util_specter.py,sha256=cML3IBjuXG2bgcKWCKDyIvCXvi3S_-oltzAoylOE5sc,11056
 cryptoadvance/spectrum/cli/__init__.py,sha256=ppGRR2Jjs88hzqjmyONWoce5OGlb25oNUp5-kqDdSQk,1602
 cryptoadvance/spectrum/cli/cli_server.py,sha256=cRWc_W_EO8OyxuuT-_D4YZDRKutSQjeOpvgHenLN95I,931
 cryptoadvance/spectrum/server_endpoints/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cryptoadvance/spectrum/server_endpoints/core_api.py,sha256=g8MA1woimMcQpdXjU_YjdNdW7aJKxHu6FEHaEmOr56I,1123
 cryptoadvance/spectrum/server_endpoints/healthz.py,sha256=L3DeZfYvbElbODGU0iI-Pp9VyIG_qX7NLCDv0BGgIB4,578
-cryptoadvance.spectrum-0.6.6.dist-info/LICENSE,sha256=qngzYiQsYYQ2nbqrsUpi-CfOQzMi2vSOlvXztgpdy0I,1073
-cryptoadvance.spectrum-0.6.6.dist-info/METADATA,sha256=W7vMMagqTnvuYfmRN8s5ii-PBq0dull56u9mO9_YExI,4631
-cryptoadvance.spectrum-0.6.6.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-cryptoadvance.spectrum-0.6.6.dist-info/top_level.txt,sha256=9Kw9-7F8HXtLLY4ORa3axsbqwYNPCX2HPq9tiMrEEP8,14
-cryptoadvance.spectrum-0.6.6.dist-info/RECORD,,
+cryptoadvance.spectrum-0.6.7.dist-info/LICENSE,sha256=qngzYiQsYYQ2nbqrsUpi-CfOQzMi2vSOlvXztgpdy0I,1073
+cryptoadvance.spectrum-0.6.7.dist-info/METADATA,sha256=jvV3iriHtXdXbwU_NrQw-9-9VuiZjUg32tyX4dN3oyE,4631
+cryptoadvance.spectrum-0.6.7.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+cryptoadvance.spectrum-0.6.7.dist-info/top_level.txt,sha256=9Kw9-7F8HXtLLY4ORa3axsbqwYNPCX2HPq9tiMrEEP8,14
+cryptoadvance.spectrum-0.6.7.dist-info/RECORD,,
```

