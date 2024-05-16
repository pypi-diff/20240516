# Comparing `tmp/appmesh-1.0.3-py3-none-any.whl.zip` & `tmp/appmesh-1.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 16110 bytes, number of entries: 6
--rw-r--r--  2.0 unx       11 b- defN 24-May-16 09:42 appmesh/__init__.py
--rw-r--r--  2.0 unx    58974 b- defN 24-May-16 09:42 appmesh/appmesh_client.py
--rw-r--r--  2.0 unx    10786 b- defN 24-May-16 09:42 appmesh-1.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-16 09:42 appmesh-1.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-May-16 09:42 appmesh-1.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      455 b- defN 24-May-16 09:42 appmesh-1.0.3.dist-info/RECORD
-6 files, 70326 bytes uncompressed, 15288 bytes compressed:  78.3%
+Zip file size: 16156 bytes, number of entries: 6
+-rw-r--r--  2.0 unx       11 b- defN 24-May-16 13:28 appmesh/__init__.py
+-rw-r--r--  2.0 unx    58981 b- defN 24-May-16 13:28 appmesh/appmesh_client.py
+-rw-r--r--  2.0 unx    10786 b- defN 24-May-16 13:29 appmesh-1.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-16 13:29 appmesh-1.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-May-16 13:29 appmesh-1.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      455 b- defN 24-May-16 13:29 appmesh-1.0.4.dist-info/RECORD
+6 files, 70333 bytes uncompressed, 15334 bytes compressed:  78.2%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: appmesh/__init__.py
 Comment: 
 
 Filename: appmesh/appmesh_client.py
 Comment: 
 
-Filename: appmesh-1.0.3.dist-info/METADATA
+Filename: appmesh-1.0.4.dist-info/METADATA
 Comment: 
 
-Filename: appmesh-1.0.3.dist-info/WHEEL
+Filename: appmesh-1.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: appmesh-1.0.3.dist-info/top_level.txt
+Filename: appmesh-1.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: appmesh-1.0.3.dist-info/RECORD
+Filename: appmesh-1.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## appmesh/appmesh_client.py

```diff
@@ -604,20 +604,23 @@
     def app_delete(self, app_name: str) -> bool:
         """Remove an application.
 
         Args:
             app_name (str): the application name.
 
         Returns:
-            bool: success or failure.
+            bool: True for delete success, Flase for not exist anymore.
         """
         resp = self._request_http(AppMeshClient.Method.DELETE, path=f"/appmesh/app/{app_name}")
-        if resp.status_code != HTTPStatus.OK:
+        if resp.status_code == HTTPStatus.OK:
+            return True
+        elif resp.status_code == HTTPStatus.NOT_FOUND:
+            return False
+        else:
             raise Exception(resp.text)
-        return resp.status_code == HTTPStatus.OK
 
     def app_enable(self, app_name: str) -> bool:
         """Enable an application
 
         Args:
             app_name (str): the application name.
 
@@ -1170,18 +1173,15 @@
                 success, output, position, exit_code = self.app_output(app_name=run.app_name, stdout_position=output_position, stdout_index=0, process_uuid=run.proc_uid, timeout=interval)
                 if output and stdout_print:
                     print(output, end="")
                 if position is not None:
                     output_position = position
                 if exit_code is not None:
                     # success
-                    try:
-                        self.app_delete(run.app_name)
-                    except Exception:
-                        pass
+                    self.app_delete(run.app_name)
                     break
                 if not success:
                     # failed
                     break
                 if timeout > 0 and (datetime.now() - start).seconds > timeout:
                     # timeout
                     break
```

## Comparing `appmesh-1.0.3.dist-info/METADATA` & `appmesh-1.0.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appmesh
-Version: 1.0.3
+Version: 1.0.4
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
-Metadata-Version: 2.1 Name: appmesh Version: 1.0.3 Summary: Client SDK for App
+Metadata-Version: 2.1 Name: appmesh Version: 1.0.4 Summary: Client SDK for App
 Mesh Home-page: https://github.com/laoshanxi/app-mesh Author: laoshanxi Author-
 email: 178029200@qq.com License: MIT Keywords: appmesh AppMesh app-mesh
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown Requires-Dist:
 requests Requires-Dist: msgpack Requires-Dist: requests-toolbelt Requires-Dist:
 aniso8601 ï»¿[![language.badge]][language.url] [![standard.badge]]
```

