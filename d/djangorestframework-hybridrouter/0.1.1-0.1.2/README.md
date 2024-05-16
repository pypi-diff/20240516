# Comparing `tmp/djangorestframework_hybridrouter-0.1.1.tar.gz` & `tmp/djangorestframework_hybridrouter-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangorestframework_hybridrouter-0.1.1.tar", last modified: Wed May 15 20:45:29 2024, max compression
+gzip compressed data, was "djangorestframework_hybridrouter-0.1.2.tar", last modified: Wed May 15 21:21:48 2024, max compression
```

## Comparing `djangorestframework_hybridrouter-0.1.1.tar` & `djangorestframework_hybridrouter-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:45:29.517597 djangorestframework_hybridrouter-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-15 20:45:25.000000 djangorestframework_hybridrouter-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-15 20:45:29.517597 djangorestframework_hybridrouter-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-15 20:45:25.000000 djangorestframework_hybridrouter-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:45:29.513597 djangorestframework_hybridrouter-0.1.1/djangorestframework_hybridrouter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-15 20:45:29.000000 djangorestframework_hybridrouter-0.1.1/djangorestframework_hybridrouter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-15 20:45:29.000000 djangorestframework_hybridrouter-0.1.1/djangorestframework_hybridrouter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 20:45:29.000000 djangorestframework_hybridrouter-0.1.1/djangorestframework_hybridrouter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-15 20:45:29.000000 djangorestframework_hybridrouter-0.1.1/djangorestframework_hybridrouter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-15 20:45:29.000000 djangorestframework_hybridrouter-0.1.1/djangorestframework_hybridrouter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:45:29.513597 djangorestframework_hybridrouter-0.1.1/hybridrouter/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 20:45:25.000000 djangorestframework_hybridrouter-0.1.1/hybridrouter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-15 20:45:25.000000 djangorestframework_hybridrouter-0.1.1/hybridrouter/hybridrouter.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 20:45:29.517597 djangorestframework_hybridrouter-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-15 20:45:25.000000 djangorestframework_hybridrouter-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:21:48.427538 djangorestframework_hybridrouter-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-15 21:21:44.000000 djangorestframework_hybridrouter-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-15 21:21:48.427538 djangorestframework_hybridrouter-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-15 21:21:44.000000 djangorestframework_hybridrouter-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:21:48.427538 djangorestframework_hybridrouter-0.1.2/djangorestframework_hybridrouter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-15 21:21:48.000000 djangorestframework_hybridrouter-0.1.2/djangorestframework_hybridrouter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-15 21:21:48.000000 djangorestframework_hybridrouter-0.1.2/djangorestframework_hybridrouter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 21:21:48.000000 djangorestframework_hybridrouter-0.1.2/djangorestframework_hybridrouter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-15 21:21:48.000000 djangorestframework_hybridrouter-0.1.2/djangorestframework_hybridrouter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-15 21:21:48.000000 djangorestframework_hybridrouter-0.1.2/djangorestframework_hybridrouter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:21:48.427538 djangorestframework_hybridrouter-0.1.2/hybridrouter/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 21:21:44.000000 djangorestframework_hybridrouter-0.1.2/hybridrouter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5079 2024-05-15 21:21:44.000000 djangorestframework_hybridrouter-0.1.2/hybridrouter/hybridrouter.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 21:21:48.427538 djangorestframework_hybridrouter-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-15 21:21:44.000000 djangorestframework_hybridrouter-0.1.2/setup.py
```

### Comparing `djangorestframework_hybridrouter-0.1.1/LICENSE` & `djangorestframework_hybridrouter-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `djangorestframework_hybridrouter-0.1.1/hybridrouter/hybridrouter.py` & `djangorestframework_hybridrouter-0.1.2/hybridrouter/hybridrouter.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,17 +12,17 @@
         
     def register_view(self,  url, view, name):
         path = re_path(url, view.as_view(), name=name)
         self._api_view_urls[name] = path
         
     def register_viewset(self, prefix, viewset, basename=None):
         super().register(prefix, viewset, basename)
-        
+    
     def register(self, prefix, viewset, basename=None):
-        raise NotImplementedError("Use register_viewset or register_view instead.")
+        raise NotImplementedError("The 'register' method is deprecated. Use 'register_viewset' instead.")
 
     def remove_api_view(self, name):
         if name in self._api_view_urls:
             del self._api_view_urls[name]
 
     @property
     def api_view_urls(self):
```

### Comparing `djangorestframework_hybridrouter-0.1.1/setup.py` & `djangorestframework_hybridrouter-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='djangorestframework-hybridrouter',
-    version='0.1.1',
+    version='0.1.2',
     packages=[
         'hybridrouter',
     ],
     install_requires=[
         'Django',
         'djangorestframework',
     ],
```

