# Comparing `tmp/appmesh-0.9.8-py3-none-any.whl.zip` & `tmp/appmesh-0.9.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 16100 bytes, number of entries: 6
--rw-r--r--  2.0 unx       11 b- defN 24-May-16 06:19 appmesh/__init__.py
--rw-r--r--  2.0 unx    58878 b- defN 24-May-16 06:19 appmesh/appmesh_client.py
--rw-r--r--  2.0 unx    10786 b- defN 24-May-16 06:20 appmesh-0.9.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-16 06:20 appmesh-0.9.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-May-16 06:20 appmesh-0.9.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      455 b- defN 24-May-16 06:20 appmesh-0.9.8.dist-info/RECORD
-6 files, 70230 bytes uncompressed, 15278 bytes compressed:  78.2%
+Zip file size: 16113 bytes, number of entries: 6
+-rw-r--r--  2.0 unx       11 b- defN 24-May-16 07:05 appmesh/__init__.py
+-rw-r--r--  2.0 unx    58974 b- defN 24-May-16 07:05 appmesh/appmesh_client.py
+-rw-r--r--  2.0 unx    10786 b- defN 24-May-16 07:05 appmesh-0.9.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-16 07:05 appmesh-0.9.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-May-16 07:05 appmesh-0.9.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      455 b- defN 24-May-16 07:05 appmesh-0.9.9.dist-info/RECORD
+6 files, 70326 bytes uncompressed, 15291 bytes compressed:  78.3%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: appmesh/__init__.py
 Comment: 
 
 Filename: appmesh/appmesh_client.py
 Comment: 
 
-Filename: appmesh-0.9.8.dist-info/METADATA
+Filename: appmesh-0.9.9.dist-info/METADATA
 Comment: 
 
-Filename: appmesh-0.9.8.dist-info/WHEEL
+Filename: appmesh-0.9.9.dist-info/WHEEL
 Comment: 
 
-Filename: appmesh-0.9.8.dist-info/top_level.txt
+Filename: appmesh-0.9.9.dist-info/top_level.txt
 Comment: 
 
-Filename: appmesh-0.9.8.dist-info/RECORD
+Filename: appmesh-0.9.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## appmesh/appmesh_client.py

```diff
@@ -1170,15 +1170,18 @@
                 success, output, position, exit_code = self.app_output(app_name=run.app_name, stdout_position=output_position, stdout_index=0, process_uuid=run.proc_uid, timeout=interval)
                 if output and stdout_print:
                     print(output, end="")
                 if position is not None:
                     output_position = position
                 if exit_code is not None:
                     # success
-                    self.app_delete(run.app_name)
+                    try:
+                        self.app_delete(run.app_name)
+                    except Exception:
+                        pass
                     break
                 if not success:
                     # failed
                     break
                 if timeout > 0 and (datetime.now() - start).seconds > timeout:
                     # timeout
                     break
```

## Comparing `appmesh-0.9.8.dist-info/METADATA` & `appmesh-0.9.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appmesh
-Version: 0.9.8
+Version: 0.9.9
 Summary: Client SDK for App Mesh
 Home-page: https://github.com/laoshanxi/app-mesh
 Author: laoshanxi
 Author-email: 178029200@qq.com
 License: MIT
 Keywords: appmesh AppMesh app-mesh
 Classifier: Programming Language :: Python :: 3
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: appmesh Version: 0.9.8 Summary: Client SDK for App
+Metadata-Version: 2.1 Name: appmesh Version: 0.9.9 Summary: Client SDK for App
 Mesh Home-page: https://github.com/laoshanxi/app-mesh Author: laoshanxi Author-
 email: 178029200@qq.com License: MIT Keywords: appmesh AppMesh app-mesh
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown Requires-Dist:
 requests Requires-Dist: msgpack Requires-Dist: requests-toolbelt Requires-Dist:
 aniso8601 ï»¿[![language.badge]][language.url] [![standard.badge]]
```

