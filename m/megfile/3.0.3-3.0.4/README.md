# Comparing `tmp/megfile-3.0.3-py3-none-any.whl.zip` & `tmp/megfile-3.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,32 +1,32 @@
-Zip file size: 127262 bytes, number of entries: 52
+Zip file size: 127324 bytes, number of entries: 52
 -rw-rw-r--  2.0 unx     6534 b- defN 23-Oct-16 09:18 megfile/__init__.py
 -rw-rw-r--  2.0 unx    21880 b- defN 24-Apr-24 09:19 megfile/cli.py
 -rw-rw-r--  2.0 unx      658 b- defN 24-May-06 06:31 megfile/config.py
 -rw-rw-r--  2.0 unx    13323 b- defN 24-Apr-24 07:04 megfile/errors.py
 -rw-rw-r--  2.0 unx    11547 b- defN 24-Jan-22 05:53 megfile/fs.py
 -rw-rw-r--  2.0 unx    38237 b- defN 24-Jan-22 05:18 megfile/fs_path.py
 -rw-rw-r--  2.0 unx     9156 b- defN 24-Jan-22 05:53 megfile/hdfs.py
 -rw-rw-r--  2.0 unx    26859 b- defN 24-May-07 05:44 megfile/hdfs_path.py
 -rw-rw-r--  2.0 unx     2032 b- defN 24-Jan-22 05:53 megfile/http.py
 -rw-rw-r--  2.0 unx    11593 b- defN 24-May-07 05:44 megfile/http_path.py
 -rw-rw-r--  2.0 unx     6219 b- defN 23-Jul-07 04:07 megfile/interfaces.py
 -rw-rw-r--  2.0 unx    29487 b- defN 23-Oct-16 09:18 megfile/pathlike.py
 -rw-rw-r--  2.0 unx    12352 b- defN 24-Jan-22 05:53 megfile/s3.py
--rw-rw-r--  2.0 unx    91067 b- defN 24-May-07 05:44 megfile/s3_path.py
+-rw-rw-r--  2.0 unx    91305 b- defN 24-May-16 07:03 megfile/s3_path.py
 -rw-rw-r--  2.0 unx    12524 b- defN 24-Jan-22 05:53 megfile/sftp.py
 -rw-rw-r--  2.0 unx    51666 b- defN 24-Apr-24 08:36 megfile/sftp_path.py
 -rw-rw-r--  2.0 unx    33725 b- defN 24-Apr-25 01:39 megfile/smart.py
 -rw-rw-r--  2.0 unx     6749 b- defN 23-Sep-19 01:59 megfile/smart_path.py
 -rw-rw-r--  2.0 unx      707 b- defN 24-Jan-22 05:53 megfile/stdio.py
 -rw-rw-r--  2.0 unx     2873 b- defN 23-Aug-18 08:55 megfile/stdio_path.py
--rw-rw-r--  2.0 unx       19 b- defN 24-May-10 02:12 megfile/version.py
+-rw-rw-r--  2.0 unx       19 b- defN 24-May-16 07:18 megfile/version.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-May-25 06:42 megfile/lib/__init__.py
 -rw-rw-r--  2.0 unx    13185 b- defN 24-May-06 07:42 megfile/lib/base_prefetch_reader.py
--rw-rw-r--  2.0 unx     4546 b- defN 24-May-07 05:17 megfile/lib/combine_reader.py
+-rw-rw-r--  2.0 unx     4546 b- defN 24-May-15 02:05 megfile/lib/combine_reader.py
 -rw-rw-r--  2.0 unx     2233 b- defN 23-Nov-09 02:49 megfile/lib/compare.py
 -rw-rw-r--  2.0 unx      234 b- defN 24-Jan-22 05:18 megfile/lib/compat.py
 -rw-rw-r--  2.0 unx     4054 b- defN 23-Nov-17 02:51 megfile/lib/fnmatch.py
 -rw-rw-r--  2.0 unx     9732 b- defN 23-Jul-07 05:32 megfile/lib/glob.py
 -rw-rw-r--  2.0 unx     2040 b- defN 23-Dec-12 08:15 megfile/lib/hdfs_prefetch_reader.py
 -rw-rw-r--  2.0 unx      442 b- defN 23-Oct-16 09:18 megfile/lib/hdfs_tools.py
 -rw-rw-r--  2.0 unx     3352 b- defN 23-Dec-12 08:15 megfile/lib/http_prefetch_reader.py
@@ -34,21 +34,21 @@
 -rw-rw-r--  2.0 unx     1915 b- defN 23-May-25 06:42 megfile/lib/lazy_handler.py
 -rw-rw-r--  2.0 unx     7017 b- defN 24-May-06 06:31 megfile/lib/s3_buffered_writer.py
 -rw-rw-r--  2.0 unx     1412 b- defN 23-Sep-20 08:59 megfile/lib/s3_cached_handler.py
 -rw-rw-r--  2.0 unx     6150 b- defN 23-Dec-12 08:15 megfile/lib/s3_limited_seekable_writer.py
 -rw-rw-r--  2.0 unx     3971 b- defN 23-Sep-20 08:59 megfile/lib/s3_memory_handler.py
 -rw-rw-r--  2.0 unx     3557 b- defN 23-Sep-20 08:59 megfile/lib/s3_pipe_handler.py
 -rw-rw-r--  2.0 unx     4249 b- defN 23-Dec-12 08:15 megfile/lib/s3_prefetch_reader.py
--rw-rw-r--  2.0 unx     3564 b- defN 24-May-07 05:17 megfile/lib/s3_share_cache_reader.py
+-rw-rw-r--  2.0 unx     3564 b- defN 24-May-15 02:05 megfile/lib/s3_share_cache_reader.py
 -rw-rw-r--  2.0 unx     2683 b- defN 23-May-25 06:42 megfile/lib/shadow_handler.py
 -rw-rw-r--  2.0 unx     2044 b- defN 23-May-25 06:42 megfile/lib/stdio_handler.py
 -rw-rw-r--  2.0 unx      103 b- defN 23-Jun-16 02:18 megfile/lib/url.py
 -rw-rw-r--  2.0 unx     9531 b- defN 24-May-07 05:44 megfile/utils/__init__.py
 -rw-rw-r--  2.0 unx     2538 b- defN 23-Jul-13 03:47 megfile/utils/mutex.py
--rw-rw-r--  2.0 unx    11357 b- defN 24-May-10 02:12 megfile-3.0.3.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1080 b- defN 24-May-10 02:12 megfile-3.0.3.dist-info/LICENSE.pyre
--rw-rw-r--  2.0 unx     8916 b- defN 24-May-10 02:12 megfile-3.0.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-May-10 02:12 megfile-3.0.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx       49 b- defN 24-May-10 02:12 megfile-3.0.3.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        8 b- defN 24-May-10 02:12 megfile-3.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     4182 b- defN 24-May-10 02:12 megfile-3.0.3.dist-info/RECORD
-52 files, 504372 bytes uncompressed, 120736 bytes compressed:  76.1%
+-rw-rw-r--  2.0 unx    11357 b- defN 24-May-16 07:19 megfile-3.0.4.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1080 b- defN 24-May-16 07:19 megfile-3.0.4.dist-info/LICENSE.pyre
+-rw-rw-r--  2.0 unx     8963 b- defN 24-May-16 07:19 megfile-3.0.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-16 07:19 megfile-3.0.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       49 b- defN 24-May-16 07:19 megfile-3.0.4.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        8 b- defN 24-May-16 07:19 megfile-3.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     4182 b- defN 24-May-16 07:19 megfile-3.0.4.dist-info/RECORD
+52 files, 504657 bytes uncompressed, 120798 bytes compressed:  76.1%
```

## zipnote {}

```diff
@@ -129,29 +129,29 @@
 
 Filename: megfile/utils/__init__.py
 Comment: 
 
 Filename: megfile/utils/mutex.py
 Comment: 
 
-Filename: megfile-3.0.3.dist-info/LICENSE
+Filename: megfile-3.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: megfile-3.0.3.dist-info/LICENSE.pyre
+Filename: megfile-3.0.4.dist-info/LICENSE.pyre
 Comment: 
 
-Filename: megfile-3.0.3.dist-info/METADATA
+Filename: megfile-3.0.4.dist-info/METADATA
 Comment: 
 
-Filename: megfile-3.0.3.dist-info/WHEEL
+Filename: megfile-3.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: megfile-3.0.3.dist-info/entry_points.txt
+Filename: megfile-3.0.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: megfile-3.0.3.dist-info/top_level.txt
+Filename: megfile-3.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: megfile-3.0.3.dist-info/RECORD
+Filename: megfile-3.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## megfile/s3_path.py

```diff
@@ -134,23 +134,28 @@
 
 
 def get_endpoint_url(profile_name: Optional[str] = None) -> str:
     '''Get the endpoint url of S3
 
     :returns: S3 endpoint url
     '''
-    environ_key = f'{profile_name}__OSS_ENDPOINT'.upper(
-    ) if profile_name else 'OSS_ENDPOINT'
-    environ_endpoint_url = os.environ.get(environ_key)
-    if environ_endpoint_url:
-        warning_endpoint_url(environ_key, environ_endpoint_url)
-        return environ_endpoint_url
+    if profile_name:
+        environ_keys = (f'{profile_name}__OSS_ENDPOINT'.upper(),)
+    else:
+        environ_keys = (
+            'OSS_ENDPOINT', 'AWS_ENDPOINT_URL_S3', 'AWS_ENDPOINT_URL')
+    for environ_key in environ_keys:
+        environ_endpoint_url = os.environ.get(environ_key)
+        if environ_endpoint_url:
+            warning_endpoint_url(environ_key, environ_endpoint_url)
+            return environ_endpoint_url
     try:
-        config_endpoint_url = get_scoped_config(profile_name=profile_name).get(
-            's3', {}).get('endpoint_url')
+        config = get_scoped_config(profile_name=profile_name)
+        config_endpoint_url = config.get('s3', {}).get('endpoint_url')
+        config_endpoint_url = config_endpoint_url or config.get('endpoint_url')
         if config_endpoint_url:
             warning_endpoint_url('~/.aws/config', config_endpoint_url)
             return config_endpoint_url
     except botocore.exceptions.ProfileNotFound:
         pass
     return endpoint_url
```

## megfile/version.py

```diff
@@ -1 +1 @@
-VERSION = "3.0.3"
+VERSION = "3.0.4"
```

## Comparing `megfile-3.0.3.dist-info/LICENSE` & `megfile-3.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `megfile-3.0.3.dist-info/LICENSE.pyre` & `megfile-3.0.4.dist-info/LICENSE.pyre`

 * *Files identical despite different names*

## Comparing `megfile-3.0.3.dist-info/METADATA` & `megfile-3.0.4.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: megfile
-Version: 3.0.3
+Version: 3.0.4
 Summary: Megvii file operation library
 Home-page: https://github.com/megvii-research/megfile
 Author: megvii
 Author-email: megfile@megvii.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -156,18 +156,18 @@
 ## Configuration
 
 Using `s3` as an example, the following describes the configuration methods. For more details, please refer to [Configuration](https://megvii-research.github.io/megfile/configuration.html).
 
 You can use environments and configuration file for configuration, and priority is that environment variables take precedence over configuration file.
 
 ### Use environments
-You can use environments to setup authentication credentials for your s3 account:
+You can use environments to setup authentication credentials for your `s3` account:
 - `AWS_ACCESS_KEY_ID`: access key
 - `AWS_SECRET_ACCESS_KEY`: secret key
-- `OSS_ENDPOINT`: endpoint url of s3
+- `OSS_ENDPOINT` / `AWS_ENDPOINT_URL_S3` / `AWS_ENDPOINT_URL`: endpoint url of s3
 - `AWS_S3_ADDRESSING_STYLE`: addressing style
 
 ### Use command
 You can update config file with `megfile` command easyly:
 [megfile config s3 [OPTIONS] AWS_ACCESS_KEY_ID AWS_SECRET_ACCESS_KEY](https://megvii-research.github.io/megfile/cli.html#megfile-config-s3) 
 
 ```
```

## Comparing `megfile-3.0.3.dist-info/RECORD` & `megfile-3.0.4.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 megfile/hdfs.py,sha256=aAkHobOO0nDcLoqj0tx_1tvgoLOCooTWuukq0pO-nQA,9156
 megfile/hdfs_path.py,sha256=obfMMKSuBcSGgtEN18jXhEldm4hawMhxk8QoRv4k790,26859
 megfile/http.py,sha256=a3oAuARSSaIU8VMx86Mui0N5Vh-EI0AoHnwxRU5DSMU,2032
 megfile/http_path.py,sha256=WJd8-s_xsF71rC2QtXikH--FCsqn2u-e83YF8OarKeY,11593
 megfile/interfaces.py,sha256=h3tWE8hVt5S-HopaMAX6lunPJ97vzhv6jH_2HubcDNc,6219
 megfile/pathlike.py,sha256=Ere6tMf2nsI7bDsZo0WBzl_2HRrS_4iKOpYp0zZltAU,29487
 megfile/s3.py,sha256=siBZfveWX1TDA4Mp41UvugcG3zlrhl_iPUbixUp1TmI,12352
-megfile/s3_path.py,sha256=vypCpnNzkObng6BVcq4j3Y_W3J2btq16B8154bWVPjg,91067
+megfile/s3_path.py,sha256=spksQesniQOYWmfIPfJeU4kMSiFAIlB8v2yIHVRLliA,91305
 megfile/sftp.py,sha256=JCkF2v1ZbHuIy_Bg3l85AesjFDimDzx9Gh1gRoMsahc,12524
 megfile/sftp_path.py,sha256=ErPKmwgaCOvvhp3aKhqX9WKIAGbWR30QUWvptQWtag8,51666
 megfile/smart.py,sha256=y5Dzr7_f0jS2FJDF4tWbEO4SPf39zqYftqkVgMhiJds,33725
 megfile/smart_path.py,sha256=Y0UFh4J2ccydRY2W-wX2ubaf9zzJx1M2nf-VLBGe4mk,6749
 megfile/stdio.py,sha256=yRhlfUA2DHi3bq-9cXsSlbLCnHvS_zvglO2IYYyPsGc,707
 megfile/stdio_path.py,sha256=eQulTXUwHvUKA-5PKCGfVNiEPkJhG9YtVhtU58OcmoM,2873
-megfile/version.py,sha256=UE7hhbkRaCCOli6ABmNbLoQp1rQZubN3Q_YGWfVH4sY,19
+megfile/version.py,sha256=DnboapDM00MYgi1PslOAcm9O5A6fEv0tG12NA4yH9TI,19
 megfile/lib/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 megfile/lib/base_prefetch_reader.py,sha256=WKwrpuniO8a1iU2k5mIHEpuBP8caLtIeqLrpKbmqX_A,13185
 megfile/lib/combine_reader.py,sha256=XFSqEY5A5X5Uf7eQ6AXAzrvNteESSXvKNVPktGjo3KY,4546
 megfile/lib/compare.py,sha256=yG2fZve_gMg32rQVCdwixBdqgYRsjn-24TqhALQaOrA,2233
 megfile/lib/compat.py,sha256=0wt3_atcYhSLCxUj_WuDlQa3E1atjZfwJQ12thiFh5Q,234
 megfile/lib/fnmatch.py,sha256=HgdlnEWBsdFUOZqnW_v1kj1jeH_9lMcCqW85pyMu4vM,4054
 megfile/lib/glob.py,sha256=7i9dIput9rI9JIPyTZX-JDmFS7IP_THlX1k-35foAfw,9732
@@ -39,14 +39,14 @@
 megfile/lib/s3_prefetch_reader.py,sha256=ol_gS0J3Yr4lMBkmok3JNuhzFfTthVzmZy5z94NFGeM,4249
 megfile/lib/s3_share_cache_reader.py,sha256=ecx-62wGqgTn5vHIpKhNACCHdYWm6oc1_xwy3vkV4m0,3564
 megfile/lib/shadow_handler.py,sha256=IbFyTw107t-yWH0cGrDjAJX-CS3xeEr77_PTGsnSgk4,2683
 megfile/lib/stdio_handler.py,sha256=QDWtcZxz-hzi-rqQUiSlR3NrihX1fjK_Rj9T2mdTFEg,2044
 megfile/lib/url.py,sha256=VbQLjo0s4AaV0iSk66BcjI68aUTcN9zBZ5x6-cM4Qvs,103
 megfile/utils/__init__.py,sha256=xrBIJcVJTb_yR68ekAyd9u4HQ46s3xgIjUZoH_Lx7hU,9531
 megfile/utils/mutex.py,sha256=-2KH3bNovKRd9zvsXq9n3bWM7rQdoG9hO7tUPxVG_Po,2538
-megfile-3.0.3.dist-info/LICENSE,sha256=WNHhf_5RCaeuKWyq_K39vmp9F28LxKsB4SpomwSZ2L0,11357
-megfile-3.0.3.dist-info/LICENSE.pyre,sha256=9lf5nT-5ZH25JijpYAequ0bl8E8z5JmZB1qrjiUMp84,1080
-megfile-3.0.3.dist-info/METADATA,sha256=icEVsbrmXVTDGlH9axr1walAIB0pHrCPb6Jj0FpPAhA,8916
-megfile-3.0.3.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-megfile-3.0.3.dist-info/entry_points.txt,sha256=M6ZWSSv5_5_QtIpZafy3vq7WuOJ_5dSGQQnEZbByt2Q,49
-megfile-3.0.3.dist-info/top_level.txt,sha256=i3rMgdU1ZAJekAceojhA-bkm3749PzshtRmLTbeLUPQ,8
-megfile-3.0.3.dist-info/RECORD,,
+megfile-3.0.4.dist-info/LICENSE,sha256=WNHhf_5RCaeuKWyq_K39vmp9F28LxKsB4SpomwSZ2L0,11357
+megfile-3.0.4.dist-info/LICENSE.pyre,sha256=9lf5nT-5ZH25JijpYAequ0bl8E8z5JmZB1qrjiUMp84,1080
+megfile-3.0.4.dist-info/METADATA,sha256=ULNUWUSidVxRQfUIJquDdSrV87Os1OQByXqRhO-7TPw,8963
+megfile-3.0.4.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+megfile-3.0.4.dist-info/entry_points.txt,sha256=M6ZWSSv5_5_QtIpZafy3vq7WuOJ_5dSGQQnEZbByt2Q,49
+megfile-3.0.4.dist-info/top_level.txt,sha256=i3rMgdU1ZAJekAceojhA-bkm3749PzshtRmLTbeLUPQ,8
+megfile-3.0.4.dist-info/RECORD,,
```

