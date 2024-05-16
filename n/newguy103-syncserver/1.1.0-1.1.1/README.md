# Comparing `tmp/newguy103-syncserver-1.1.0.tar.gz` & `tmp/newguy103-syncserver-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newguy103-syncserver-1.1.0.tar", last modified: Wed Feb 28 09:22:23 2024, max compression
+gzip compressed data, was "newguy103-syncserver-1.1.1.tar", last modified: Thu Feb 29 00:27:02 2024, max compression
```

## Comparing `newguy103-syncserver-1.1.0.tar` & `newguy103-syncserver-1.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 userc     (1000) userc     (1000)        0 2024-02-28 09:22:23.545409 newguy103-syncserver-1.1.0/
--rw-r--r--   0 userc     (1000) userc     (1000)     3334 2024-02-28 09:22:23.545409 newguy103-syncserver-1.1.0/PKG-INFO
--rw-rw-r--   0 userc     (1000) userc     (1000)     2852 2024-02-28 08:35:52.000000 newguy103-syncserver-1.1.0/README.md
-drwxrwxr-x   0 userc     (1000) userc     (1000)        0 2024-02-28 09:22:23.545409 newguy103-syncserver-1.1.0/newguy103_syncserver.egg-info/
--rw-r--r--   0 userc     (1000) userc     (1000)     3334 2024-02-28 09:22:23.000000 newguy103-syncserver-1.1.0/newguy103_syncserver.egg-info/PKG-INFO
--rw-rw-r--   0 userc     (1000) userc     (1000)      453 2024-02-28 09:22:23.000000 newguy103-syncserver-1.1.0/newguy103_syncserver.egg-info/SOURCES.txt
--rw-rw-r--   0 userc     (1000) userc     (1000)        1 2024-02-28 09:22:23.000000 newguy103-syncserver-1.1.0/newguy103_syncserver.egg-info/dependency_links.txt
--rw-rw-r--   0 userc     (1000) userc     (1000)      123 2024-02-28 09:22:23.000000 newguy103-syncserver-1.1.0/newguy103_syncserver.egg-info/entry_points.txt
--rw-rw-r--   0 userc     (1000) userc     (1000)       68 2024-02-28 09:22:23.000000 newguy103-syncserver-1.1.0/newguy103_syncserver.egg-info/requires.txt
--rw-rw-r--   0 userc     (1000) userc     (1000)       11 2024-02-28 09:22:23.000000 newguy103-syncserver-1.1.0/newguy103_syncserver.egg-info/top_level.txt
--rw-rw-r--   0 userc     (1000) userc     (1000)       38 2024-02-28 09:22:23.545409 newguy103-syncserver-1.1.0/setup.cfg
--rw-rw-r--   0 userc     (1000) userc     (1000)     1001 2024-02-28 09:21:48.000000 newguy103-syncserver-1.1.0/setup.py
-drwxrwxr-x   0 userc     (1000) userc     (1000)        0 2024-02-28 09:22:23.545409 newguy103-syncserver-1.1.0/syncserver/
--rw-rw-r--   0 userc     (1000) userc     (1000)       82 2024-02-28 08:50:53.000000 newguy103-syncserver-1.1.0/syncserver/__init__.py
-drwxrwxr-x   0 userc     (1000) userc     (1000)        0 2024-02-28 09:22:23.545409 newguy103-syncserver-1.1.0/syncserver/client/
--rw-rw-r--   0 userc     (1000) userc     (1000)      154 2024-02-28 08:35:52.000000 newguy103-syncserver-1.1.0/syncserver/client/__init__.py
--rw-rw-r--   0 userc     (1000) userc     (1000)    15598 2024-02-28 08:35:52.000000 newguy103-syncserver-1.1.0/syncserver/client/interface.py
-drwxrwxr-x   0 userc     (1000) userc     (1000)        0 2024-02-28 09:22:23.545409 newguy103-syncserver-1.1.0/syncserver/server/
--rw-rw-r--   0 userc     (1000) userc     (1000)       80 2024-02-28 08:35:52.000000 newguy103-syncserver-1.1.0/syncserver/server/__init__.py
--rw-rw-r--   0 userc     (1000) userc     (1000)    37142 2024-02-28 08:51:27.000000 newguy103-syncserver-1.1.0/syncserver/server/__main__.py
--rw-rw-r--   0 userc     (1000) userc     (1000)    67745 2024-02-28 08:58:19.000000 newguy103-syncserver-1.1.0/syncserver/server/_db.py
+drwxrwxr-x   0 userc     (1000) userc     (1000)        0 2024-02-29 00:27:02.948180 newguy103-syncserver-1.1.1/
+-rw-r--r--   0 userc     (1000) userc     (1000)     3334 2024-02-29 00:27:02.948180 newguy103-syncserver-1.1.1/PKG-INFO
+-rw-rw-r--   0 userc     (1000) userc     (1000)     2852 2024-02-28 08:35:52.000000 newguy103-syncserver-1.1.1/README.md
+drwxrwxr-x   0 userc     (1000) userc     (1000)        0 2024-02-29 00:27:02.944180 newguy103-syncserver-1.1.1/newguy103_syncserver.egg-info/
+-rw-r--r--   0 userc     (1000) userc     (1000)     3334 2024-02-29 00:27:02.000000 newguy103-syncserver-1.1.1/newguy103_syncserver.egg-info/PKG-INFO
+-rw-rw-r--   0 userc     (1000) userc     (1000)      453 2024-02-29 00:27:02.000000 newguy103-syncserver-1.1.1/newguy103_syncserver.egg-info/SOURCES.txt
+-rw-rw-r--   0 userc     (1000) userc     (1000)        1 2024-02-29 00:27:02.000000 newguy103-syncserver-1.1.1/newguy103_syncserver.egg-info/dependency_links.txt
+-rw-rw-r--   0 userc     (1000) userc     (1000)      123 2024-02-29 00:27:02.000000 newguy103-syncserver-1.1.1/newguy103_syncserver.egg-info/entry_points.txt
+-rw-rw-r--   0 userc     (1000) userc     (1000)       68 2024-02-29 00:27:02.000000 newguy103-syncserver-1.1.1/newguy103_syncserver.egg-info/requires.txt
+-rw-rw-r--   0 userc     (1000) userc     (1000)       11 2024-02-29 00:27:02.000000 newguy103-syncserver-1.1.1/newguy103_syncserver.egg-info/top_level.txt
+-rw-rw-r--   0 userc     (1000) userc     (1000)       38 2024-02-29 00:27:02.948180 newguy103-syncserver-1.1.1/setup.cfg
+-rw-rw-r--   0 userc     (1000) userc     (1000)     1001 2024-02-29 00:25:56.000000 newguy103-syncserver-1.1.1/setup.py
+drwxrwxr-x   0 userc     (1000) userc     (1000)        0 2024-02-29 00:27:02.944180 newguy103-syncserver-1.1.1/syncserver/
+-rw-rw-r--   0 userc     (1000) userc     (1000)       82 2024-02-28 08:50:53.000000 newguy103-syncserver-1.1.1/syncserver/__init__.py
+drwxrwxr-x   0 userc     (1000) userc     (1000)        0 2024-02-29 00:27:02.944180 newguy103-syncserver-1.1.1/syncserver/client/
+-rw-rw-r--   0 userc     (1000) userc     (1000)      154 2024-02-28 08:35:52.000000 newguy103-syncserver-1.1.1/syncserver/client/__init__.py
+-rw-rw-r--   0 userc     (1000) userc     (1000)    15604 2024-02-29 00:24:05.000000 newguy103-syncserver-1.1.1/syncserver/client/interface.py
+drwxrwxr-x   0 userc     (1000) userc     (1000)        0 2024-02-29 00:27:02.948180 newguy103-syncserver-1.1.1/syncserver/server/
+-rw-rw-r--   0 userc     (1000) userc     (1000)       80 2024-02-28 08:35:52.000000 newguy103-syncserver-1.1.1/syncserver/server/__init__.py
+-rw-rw-r--   0 userc     (1000) userc     (1000)    37142 2024-02-28 08:51:27.000000 newguy103-syncserver-1.1.1/syncserver/server/__main__.py
+-rw-rw-r--   0 userc     (1000) userc     (1000)    67745 2024-02-28 08:58:19.000000 newguy103-syncserver-1.1.1/syncserver/server/_db.py
```

### Comparing `newguy103-syncserver-1.1.0/PKG-INFO` & `newguy103-syncserver-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newguy103-syncserver
-Version: 1.1.0
+Version: 1.1.1
 Summary: newguy103-syncserver simplifies file synchronization using Flask-based server and client modules.
 Author: NewGuy103
 Author-email: userchouenthusiast@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Requires-Dist: cryptography
 Requires-Dist: newguy103-pycrypter
```

### Comparing `newguy103-syncserver-1.1.0/README.md` & `newguy103-syncserver-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `newguy103-syncserver-1.1.0/newguy103_syncserver.egg-info/PKG-INFO` & `newguy103-syncserver-1.1.1/newguy103_syncserver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newguy103-syncserver
-Version: 1.1.0
+Version: 1.1.1
 Summary: newguy103-syncserver simplifies file synchronization using Flask-based server and client modules.
 Author: NewGuy103
 Author-email: userchouenthusiast@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Requires-Dist: cryptography
 Requires-Dist: newguy103-pycrypter
```

### Comparing `newguy103-syncserver-1.1.0/setup.py` & `newguy103-syncserver-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='newguy103-syncserver',
-    version='1.1.0',
+    version='1.1.1',
     author='NewGuy103',
     author_email='userchouenthusiast@gmail.com',
     description='newguy103-syncserver simplifies file synchronization using Flask-based server and client modules.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     entry_points={
```

### Comparing `newguy103-syncserver-1.1.0/syncserver/client/interface.py` & `newguy103-syncserver-1.1.1/syncserver/client/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,22 +212,22 @@
             return json_data
         elif not is_batch:
             return json_data.get("delete-order")
 
     def remove_deleted(
         self,
         remote_path: bytes | str,
-        delete_which: int | Literal["all"],
+        delete_which: int | Literal[":all:"],
         endpoint: str = "/remove-deleted",
     ) -> int | dict:
         if not isinstance(remote_path, (bytes, str)):
             raise TypeError("remote path must be bytes/str")
 
-        if not (delete_which == "all" or isinstance(delete_which, int)):
-            raise TypeError("delete_which can only be 'all' or int")
+        if not (delete_which == ":all:" or isinstance(delete_which, int)):
+            raise TypeError("delete_which can only be ':all:' or int")
 
         data: dict = {"file-path": remote_path, "delete-which": delete_which}
         response = requests.post(
             url=self.server_url + endpoint, headers=self.headers, json=data, timeout=5
         )
         _check_code(response.status_code)
```

### Comparing `newguy103-syncserver-1.1.0/syncserver/server/__main__.py` & `newguy103-syncserver-1.1.1/syncserver/server/__main__.py`

 * *Files identical despite different names*

### Comparing `newguy103-syncserver-1.1.0/syncserver/server/_db.py` & `newguy103-syncserver-1.1.1/syncserver/server/_db.py`

 * *Files identical despite different names*

