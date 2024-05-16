# Comparing `tmp/recom-0.0.2.tar.gz` & `tmp/recom-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recom-0.0.2.tar", last modified: Wed May 15 00:39:03 2024, max compression
+gzip compressed data, was "recom-0.0.3.tar", last modified: Thu May 16 16:59:40 2024, max compression
```

## Comparing `recom-0.0.2.tar` & `recom-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2024-05-15 00:39:03.057713 recom-0.0.2/
--rw-r--r--   0 adrian    (1000) adrian    (1000)      395 2024-05-15 00:39:03.057713 recom-0.0.2/PKG-INFO
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2024-05-15 00:39:03.057713 recom-0.0.2/recom/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      258 2024-05-15 00:37:17.000000 recom-0.0.2/recom/__init__.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      424 2024-03-29 21:20:09.000000 recom-0.0.2/recom/__main__.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2024-05-15 00:39:03.057713 recom-0.0.2/recom/backend/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      938 2024-05-15 00:37:17.000000 recom-0.0.2/recom/backend/__init__.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      743 2024-05-15 00:37:17.000000 recom-0.0.2/recom/backend/backend.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      691 2024-05-15 00:37:17.000000 recom-0.0.2/recom/backend/uart.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     9296 2024-05-15 00:37:17.000000 recom-0.0.2/recom/backend/usb.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     7239 2024-05-15 00:37:17.000000 recom-0.0.2/recom/cli.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     6267 2024-05-15 00:37:17.000000 recom-0.0.2/recom/device.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1793 2024-05-15 00:37:17.000000 recom-0.0.2/recom/interface.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1981 2024-05-15 00:37:17.000000 recom-0.0.2/recom/util.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2024-05-15 00:39:03.057713 recom-0.0.2/recom.egg-info/
--rw-r--r--   0 adrian    (1000) adrian    (1000)      395 2024-05-15 00:39:03.000000 recom-0.0.2/recom.egg-info/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      386 2024-05-15 00:39:03.000000 recom-0.0.2/recom.egg-info/SOURCES.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2024-05-15 00:39:03.000000 recom-0.0.2/recom.egg-info/dependency_links.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       46 2024-05-15 00:39:03.000000 recom-0.0.2/recom.egg-info/entry_points.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       31 2024-05-15 00:39:03.000000 recom-0.0.2/recom.egg-info/requires.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)        6 2024-05-15 00:39:03.000000 recom-0.0.2/recom.egg-info/top_level.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      122 2024-05-15 00:39:03.057713 recom-0.0.2/setup.cfg
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      800 2024-05-15 00:37:17.000000 recom-0.0.2/setup.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2024-05-16 16:59:40.814135 recom-0.0.3/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      395 2024-05-16 16:59:40.814135 recom-0.0.3/PKG-INFO
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2024-05-16 16:59:40.814135 recom-0.0.3/recom/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      258 2024-05-16 16:57:41.000000 recom-0.0.3/recom/__init__.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      424 2024-03-23 19:16:06.000000 recom-0.0.3/recom/__main__.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2024-05-16 16:59:40.814135 recom-0.0.3/recom/backend/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      938 2024-05-16 16:54:56.000000 recom-0.0.3/recom/backend/__init__.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      857 2024-05-16 16:54:56.000000 recom-0.0.3/recom/backend/backend.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      849 2024-05-16 16:54:56.000000 recom-0.0.3/recom/backend/uart.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     9298 2024-05-16 16:54:56.000000 recom-0.0.3/recom/backend/usb.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     7239 2024-05-16 16:54:56.000000 recom-0.0.3/recom/cli.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     6335 2024-05-16 16:54:56.000000 recom-0.0.3/recom/device.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1793 2024-05-16 16:54:56.000000 recom-0.0.3/recom/interface.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1981 2024-05-16 16:54:56.000000 recom-0.0.3/recom/util.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2024-05-16 16:59:40.814135 recom-0.0.3/recom.egg-info/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      395 2024-05-16 16:59:40.000000 recom-0.0.3/recom.egg-info/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      386 2024-05-16 16:59:40.000000 recom-0.0.3/recom.egg-info/SOURCES.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2024-05-16 16:59:40.000000 recom-0.0.3/recom.egg-info/dependency_links.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       46 2024-05-16 16:59:40.000000 recom-0.0.3/recom.egg-info/entry_points.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       31 2024-05-16 16:59:40.000000 recom-0.0.3/recom.egg-info/requires.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)        6 2024-05-16 16:59:40.000000 recom-0.0.3/recom.egg-info/top_level.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      122 2024-05-16 16:59:40.814135 recom-0.0.3/setup.cfg
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      800 2024-05-16 16:57:41.000000 recom-0.0.3/setup.py
```

### Comparing `recom-0.0.2/recom/backend/__init__.py` & `recom-0.0.3/recom/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `recom-0.0.2/recom/backend/usb.py` & `recom-0.0.3/recom/backend/usb.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,16 +139,16 @@
                 if dev.getProductID() != descriptor.dev_id[1]:
                     continue
                 return dev
             except Exception:
                 pass
         return None
 
-    @property
-    def type(self):
+    @classmethod
+    def type(cls):
         return "usb"
 
     @classmethod
     def find(cls, **kwargs) -> list:
         """Returns a list of all USB devices matching the provided constraings.
 
         If no constraints are provided, all USB devices will be returned.
```

### Comparing `recom-0.0.2/recom/cli.py` & `recom-0.0.3/recom/cli.py`

 * *Files identical despite different names*

### Comparing `recom-0.0.2/recom/device.py` & `recom-0.0.3/recom/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,18 +45,19 @@
 
     def __init__(self, device_descriptor: RecomDeviceDescriptor):
         self._interfaces = []
 
         # Loop through all backends and see if one can find a device based on
         # the provided device descriptor
         for be in backends:
-            cbe = be(device_descriptor)
-            if cbe is not None:
-                self._comsBackend = cbe
-                break
+            if be.type() == device_descriptor.type:
+                cbe = be(device_descriptor)
+                if cbe is not None:
+                    self._comsBackend = cbe
+                    break
         if self._comsBackend is None:
             raise RecomDeviceException.NoDeviceFound()
         self._comsBackend.open()
 
     def __del__(self):
         if self._comsBackend:
             self._comsBackend.close()
```

### Comparing `recom-0.0.2/recom/interface.py` & `recom-0.0.3/recom/interface.py`

 * *Files identical despite different names*

### Comparing `recom-0.0.2/recom/util.py` & `recom-0.0.3/recom/util.py`

 * *Files identical despite different names*

### Comparing `recom-0.0.2/setup.py` & `recom-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='recom',
-    version="0.0.2",
+    version="0.0.3",
     packages=find_packages(),
     setup_requires=['setuptools_scm'],
     license='MIT',
     author='Adrian Rothenbuhler',
     author_email='adrian@redhill-embedded.com',
     description='Embedded communication backend',
     keywords='embedded communication backedn usb serial',
```

