# Comparing `tmp/pyvelop-2024.4.1.tar.gz` & `tmp/pyvelop-2024.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvelop-2024.4.1.tar", last modified: Tue Apr  9 19:47:53 2024, max compression
+gzip compressed data, was "pyvelop-2024.5.1.tar", last modified: Sun May  5 19:27:45 2024, max compression
```

## Comparing `pyvelop-2024.4.1.tar` & `pyvelop-2024.5.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 19:47:53.328832 pyvelop-2024.4.1/
--rw-rw-rw-   0        0        0     1696 2024-04-09 19:47:53.327847 pyvelop-2024.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     1426 2024-04-09 19:21:23.000000 pyvelop-2024.4.1/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-09 19:47:53.316844 pyvelop-2024.4.1/pyvelop/
--rw-rw-rw-   0        0        0      716 2023-09-15 10:51:10.000000 pyvelop-2024.4.1/pyvelop/__init__.py
--rw-rw-rw-   0        0        0    37881 2024-04-09 19:23:12.000000 pyvelop-2024.4.1/pyvelop/__main__.py
--rw-rw-rw-   0        0        0     7204 2024-04-09 19:23:12.000000 pyvelop-2024.4.1/pyvelop/base.py
--rw-rw-rw-   0        0        0      226 2024-04-09 19:41:32.000000 pyvelop-2024.4.1/pyvelop/const.py
--rw-rw-rw-   0        0        0      598 2023-09-15 10:51:10.000000 pyvelop-2024.4.1/pyvelop/decorators.py
--rw-rw-rw-   0        0        0    12640 2023-09-15 10:51:10.000000 pyvelop-2024.4.1/pyvelop/device.py
--rw-rw-rw-   0        0        0     3139 2023-09-15 15:41:47.000000 pyvelop-2024.4.1/pyvelop/exceptions.py
--rw-rw-rw-   0        0        0    12421 2023-09-15 15:41:47.000000 pyvelop-2024.4.1/pyvelop/jnap.py
--rw-rw-rw-   0        0        0      788 2023-09-15 10:51:10.000000 pyvelop-2024.4.1/pyvelop/logger.py
--rw-rw-rw-   0        0        0    63755 2024-04-09 19:23:12.000000 pyvelop-2024.4.1/pyvelop/mesh.py
--rw-rw-rw-   0        0        0     6059 2024-04-09 19:23:12.000000 pyvelop-2024.4.1/pyvelop/node.py
-drwxrwxrwx   0        0        0        0 2024-04-09 19:47:53.325832 pyvelop-2024.4.1/pyvelop.egg-info/
--rw-rw-rw-   0        0        0     1696 2024-04-09 19:47:53.000000 pyvelop-2024.4.1/pyvelop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2024-04-09 19:47:53.000000 pyvelop-2024.4.1/pyvelop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 19:47:53.000000 pyvelop-2024.4.1/pyvelop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-09 19:47:53.000000 pyvelop-2024.4.1/pyvelop.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-09 19:47:53.000000 pyvelop-2024.4.1/pyvelop.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 19:47:53.328832 pyvelop-2024.4.1/setup.cfg
--rw-rw-rw-   0        0        0      738 2023-09-15 10:51:10.000000 pyvelop-2024.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 19:27:45.005392 pyvelop-2024.5.1/
+-rw-rw-rw-   0        0        0     1720 2024-05-05 19:27:45.004384 pyvelop-2024.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1426 2024-05-05 18:37:29.000000 pyvelop-2024.5.1/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-05 19:27:44.999127 pyvelop-2024.5.1/pyvelop/
+-rw-rw-rw-   0        0        0      716 2024-05-05 18:37:29.000000 pyvelop-2024.5.1/pyvelop/__init__.py
+-rw-rw-rw-   0        0        0    37881 2024-05-05 18:37:29.000000 pyvelop-2024.5.1/pyvelop/__main__.py
+-rw-rw-rw-   0        0        0     7204 2024-05-05 18:37:29.000000 pyvelop-2024.5.1/pyvelop/base.py
+-rw-rw-rw-   0        0        0      226 2024-05-05 19:12:50.000000 pyvelop-2024.5.1/pyvelop/const.py
+-rw-rw-rw-   0        0        0      598 2024-05-05 18:37:29.000000 pyvelop-2024.5.1/pyvelop/decorators.py
+-rw-rw-rw-   0        0        0    12640 2024-05-05 18:37:29.000000 pyvelop-2024.5.1/pyvelop/device.py
+-rw-rw-rw-   0        0        0     3139 2024-05-05 18:37:29.000000 pyvelop-2024.5.1/pyvelop/exceptions.py
+-rw-rw-rw-   0        0        0    12421 2024-05-05 18:37:29.000000 pyvelop-2024.5.1/pyvelop/jnap.py
+-rw-rw-rw-   0        0        0      788 2024-05-05 18:37:29.000000 pyvelop-2024.5.1/pyvelop/logger.py
+-rw-rw-rw-   0        0        0    63596 2024-05-05 19:12:36.000000 pyvelop-2024.5.1/pyvelop/mesh.py
+-rw-rw-rw-   0        0        0     6258 2024-05-05 19:12:36.000000 pyvelop-2024.5.1/pyvelop/node.py
+drwxrwxrwx   0        0        0        0 2024-05-05 19:27:45.003027 pyvelop-2024.5.1/pyvelop.egg-info/
+-rw-rw-rw-   0        0        0     1720 2024-05-05 19:27:44.000000 pyvelop-2024.5.1/pyvelop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2024-05-05 19:27:44.000000 pyvelop-2024.5.1/pyvelop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 19:27:44.000000 pyvelop-2024.5.1/pyvelop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-05 19:27:44.000000 pyvelop-2024.5.1/pyvelop.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-05 19:27:44.000000 pyvelop-2024.5.1/pyvelop.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-05 19:27:45.005392 pyvelop-2024.5.1/setup.cfg
+-rw-rw-rw-   0        0        0      738 2024-05-05 18:37:29.000000 pyvelop-2024.5.1/setup.py
```

### Comparing `pyvelop-2024.4.1/PKG-INFO` & `pyvelop-2024.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: pyvelop
-Version: 2024.4.1
+Version: 2024.5.1
 Summary: A Python library for the Linksys Velop Mesh system
 Home-page: https://github.com/uvjim/pyvelop
 Author: uvjim
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
+Requires-Dist: aiohttp
 
 pyvelop
 =======
 
 A Python library for the Linksys Velop Mesh system
 
 Purpose
```

### Comparing `pyvelop-2024.4.1/README.rst` & `pyvelop-2024.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `pyvelop-2024.4.1/pyvelop/__init__.py` & `pyvelop-2024.5.1/pyvelop/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvelop-2024.4.1/pyvelop/__main__.py` & `pyvelop-2024.5.1/pyvelop/__main__.py`

 * *Files identical despite different names*

### Comparing `pyvelop-2024.4.1/pyvelop/base.py` & `pyvelop-2024.5.1/pyvelop/base.py`

 * *Files identical despite different names*

### Comparing `pyvelop-2024.4.1/pyvelop/decorators.py` & `pyvelop-2024.5.1/pyvelop/decorators.py`

 * *Files identical despite different names*

### Comparing `pyvelop-2024.4.1/pyvelop/device.py` & `pyvelop-2024.5.1/pyvelop/device.py`

 * *Files identical despite different names*

### Comparing `pyvelop-2024.4.1/pyvelop/exceptions.py` & `pyvelop-2024.5.1/pyvelop/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyvelop-2024.4.1/pyvelop/jnap.py` & `pyvelop-2024.5.1/pyvelop/jnap.py`

 * *Files identical despite different names*

### Comparing `pyvelop-2024.4.1/pyvelop/logger.py` & `pyvelop-2024.5.1/pyvelop/logger.py`

 * *Files identical despite different names*

### Comparing `pyvelop-2024.4.1/pyvelop/mesh.py` & `pyvelop-2024.5.1/pyvelop/mesh.py`

 * *Files 0% similar despite different names*

```diff
@@ -830,19 +830,14 @@
         ]
         if not node_details:
             raise MeshDeviceNotFoundResponse
 
         if node_details[0].type == NodeType.PRIMARY and not force:
             raise MeshInvalidInput(f"{node_name} is a primary node. Use the force.")
 
-        # node_ip = [
-        #     adapter.get("ip")
-        #     for adapter in node_details[0].network
-        #     if adapter.get("ip")
-        # ]
         node_ip: List[str] | None = [
             adapter.get("ip")
             for adapter in node_details[0].connected_adapters
             if adapter.get("ip") and adapter.get("primary")
         ]
 
         if not node_ip:
```

### Comparing `pyvelop-2024.4.1/pyvelop/node.py` & `pyvelop-2024.5.1/pyvelop/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,19 +63,24 @@
 
         :return: a list of dictionaries that contain the MAC, IP and Guest Network status of the adapter
         """
 
         ret: List[dict[str, Any]] = []
         super_adapters: List[dict] = super().connected_adapters
         backhaul = self._attribs.get("backhaul", {})
-        for adapter in super_adapters:
-            adapter["primary"] = (
-                True if adapter.get("ip") == backhaul.get("ipAddress") else False
-            )
-            ret += [adapter]
+        if self.type == NodeType.PRIMARY:
+            for adapter in super_adapters:
+                adapter["primary"] = True
+                ret += [adapter]
+        else:
+            for adapter in super_adapters:
+                adapter["primary"] = (
+                    True if adapter.get("ip") == backhaul.get("ipAddress") else False
+                )
+                ret += [adapter]
         return ret
 
     @property
     def connected_devices(self) -> List:
         """List of the devices that are connected to the node.
 
         :return: List of connected devices in alphabetical order sorted by device name
```

### Comparing `pyvelop-2024.4.1/pyvelop.egg-info/PKG-INFO` & `pyvelop-2024.5.1/pyvelop.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: pyvelop
-Version: 2024.4.1
+Version: 2024.5.1
 Summary: A Python library for the Linksys Velop Mesh system
 Home-page: https://github.com/uvjim/pyvelop
 Author: uvjim
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
+Requires-Dist: aiohttp
 
 pyvelop
 =======
 
 A Python library for the Linksys Velop Mesh system
 
 Purpose
```

### Comparing `pyvelop-2024.4.1/setup.py` & `pyvelop-2024.5.1/setup.py`

 * *Files identical despite different names*

