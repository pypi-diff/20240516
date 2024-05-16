# Comparing `tmp/pycomposefile-0.0.8.tar.gz` & `tmp/pycomposefile-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycomposefile-0.0.8.tar", last modified: Wed Apr 20 17:12:23 2022, max compression
+gzip compressed data, was "pycomposefile-0.0.9.tar", last modified: Mon Apr 25 20:31:13 2022, max compression
```

## Comparing `pycomposefile-0.0.8.tar` & `pycomposefile-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 17:12:23.121185 pycomposefile-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)      353 2022-04-20 17:12:23.121185 pycomposefile-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-04-20 17:12:02.000000 pycomposefile-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 17:12:23.121185 pycomposefile-0.0.8/pycomposefile/
--rw-r--r--   0 runner    (1001) docker     (121)      600 2022-04-20 17:12:02.000000 pycomposefile-0.0.8/pycomposefile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5402 2022-04-20 17:12:02.000000 pycomposefile-0.0.8/pycomposefile/compose_element.py
--rw-r--r--   0 runner    (1001) docker     (121)     4614 2022-04-20 17:12:02.000000 pycomposefile-0.0.8/pycomposefile/service.py
--rw-r--r--   0 runner    (1001) docker     (121)     1998 2022-04-20 17:12:02.000000 pycomposefile-0.0.8/pycomposefile/service_blkio_config.py
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-04-20 17:12:02.000000 pycomposefile-0.0.8/pycomposefile/service_credential_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     2478 2022-04-20 17:12:02.000000 pycomposefile-0.0.8/pycomposefile/service_deploy.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 17:12:23.121185 pycomposefile-0.0.8/pycomposefile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      353 2022-04-20 17:12:22.000000 pycomposefile-0.0.8/pycomposefile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      397 2022-04-20 17:12:23.000000 pycomposefile-0.0.8/pycomposefile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-20 17:12:22.000000 pycomposefile-0.0.8/pycomposefile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-04-20 17:12:22.000000 pycomposefile-0.0.8/pycomposefile.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-04-20 17:12:23.000000 pycomposefile-0.0.8/pycomposefile.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-20 17:12:23.121185 pycomposefile-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      692 2022-04-20 17:12:02.000000 pycomposefile-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 20:31:13.889715 pycomposefile-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      353 2022-04-25 20:31:13.889715 pycomposefile-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-04-25 20:30:56.000000 pycomposefile-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 20:31:13.889715 pycomposefile-0.0.9/pycomposefile/
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-25 20:30:56.000000 pycomposefile-0.0.9/pycomposefile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5881 2022-04-25 20:30:56.000000 pycomposefile-0.0.9/pycomposefile/compose_element.py
+-rw-r--r--   0 runner    (1001) docker     (121)      600 2022-04-25 20:30:56.000000 pycomposefile-0.0.9/pycomposefile/compose_file.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 20:31:13.889715 pycomposefile-0.0.9/pycomposefile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      353 2022-04-25 20:31:13.000000 pycomposefile-0.0.9/pycomposefile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      291 2022-04-25 20:31:13.000000 pycomposefile-0.0.9/pycomposefile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-25 20:31:13.000000 pycomposefile-0.0.9/pycomposefile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2022-04-25 20:31:13.000000 pycomposefile-0.0.9/pycomposefile.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-04-25 20:31:13.000000 pycomposefile-0.0.9/pycomposefile.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-25 20:31:13.889715 pycomposefile-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      692 2022-04-25 20:30:56.000000 pycomposefile-0.0.9/setup.py
```

### Comparing `pycomposefile-0.0.8/pycomposefile/__init__.py` & `pycomposefile-0.0.9/pycomposefile/compose_file.py`

 * *Files identical despite different names*

### Comparing `pycomposefile-0.0.8/pycomposefile/compose_element.py` & `pycomposefile-0.0.9/pycomposefile/compose_element.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,14 @@
 import re
 import os
 
 
-class ComposeElement:
-    element_keys = {}
-
-    def __init__(self, config, compose_path=""):
-        self.compose_path = compose_path
-        for key in self.element_keys.keys():
-            config_element = config.pop(key, None)
-            key_config = self.element_keys[key]
-            self.set_supported_property_from_config(key, key_config, config_element, compose_path)
-        for key in config.keys():
-            # raise Exception(f"Failed to map {key} in {compose_path}")
-            pass
-
-    def set_supported_property_from_config(self, key, key_config, value, compose_path):
-        transform = key_config[0]
-        if transform is not None:
-            if isinstance(value, dict):
-                value = transform(value, key, compose_path)
-            elif isinstance(value, list):
-                value = transform(value, key, compose_path)
-            elif value is not None:
-                value = self.transform_supported_data(value, transform)
-        else:
-            # TODO: Logging message if value was not None
-            value = None
-        self.__setattr__(key, value)
-
-    def transform_supported_data(self, value, transform):
-        if type(transform) is tuple:
-            transform, valid_values = transform
+class DataTypeTransformer():
+    def transform_supported_data(self, transform, value, valid_values=None):
+        if valid_values is not None:
             value = self.transform_and_validate_supported_data(value, transform, valid_values)
         else:
             value = transform(self.replace_environment_variables(value))
         return value
 
     def transform_and_validate_supported_data(self, value, data_transformer, valid_values):
         # TODO: if the data is an integer or decimal, should there be a "between" check?
@@ -95,37 +68,78 @@
         matches = capture.search(value)
         while matches:
             env_var = os.environ.get(matches.group("variablename"))
             value = re.sub(f"\\{matches[0]}", env_var, value)
             matches = capture.search(value)
         return value
 
+
+class ComposeElement(DataTypeTransformer):
+    element_keys = {}
+
+    def __init__(self, config, compose_path=""):
+        self.compose_path = compose_path
+        for key in self.element_keys.keys():
+            config_element = config.pop(key, None)
+            key_config = self.element_keys[key]
+            self.set_supported_property_from_config(key, key_config, config_element, compose_path)
+        for key in config.keys():
+            # raise Exception(f"Failed to map {key} in {compose_path}")
+            pass
+
+    def set_supported_property_from_config(self, key, key_config, value, compose_path):
+        valid_values = None
+        if type(key_config[0]) is tuple:
+            transform, valid_values = key_config[0]
+        else:
+            transform = key_config[0]
+
+        if transform is not None:
+            if isinstance(value, dict):
+                value = transform(value, key, compose_path)
+            elif isinstance(value, list):
+                value = transform(value, key, compose_path)
+            elif value is not None:
+                value = self.transform_supported_data(transform, value, valid_values)
+        else:
+            # TODO: Logging message if value was not None
+            value = None
+        self.__setattr__(key, value)
+
     @classmethod
     def from_parsed_yaml(cls, config, name, compose_path):
         if config is None:
             return None
         compose_path = f"{compose_path}/{name}"
         return cls(config, compose_path)
 
 
-class ComposeStringOrListElement(list):
-    data_type = None
+class ComposeStringOrListElement(DataTypeTransformer, list):
+    transform = None
+    valid_values = None
 
     def __init__(self, config, key=None, compose_path=None,):
         if compose_path is not None:
             self.compose_path = f"{compose_path}/{key}"
 
         if isinstance(config, list):
             for v in config:
                 if isinstance(v, str):
                     v = v.strip("[]").rstrip().lstrip().strip("'")
-                    self.append_data_type(v)
+                    self.append_transform(v)
                 else:
-                    self.append_data_type(v, key, compose_path)
+                    self.append_transform(v, key, compose_path)
+        else:
+            self.append_transform(config, key, compose_path)
+
+    def append(self, __object) -> None:
+        if isinstance(__object, list):
+            for element in __object:
+                super().append(element)
         else:
-            self.append_data_type(config, key, compose_path)
+            super().append(__object)
 
-    def append_data_type(self, config_value, key=None, compose_path=None):
+    def append_transform(self, config_value, key=None, compose_path=None):
         if isinstance(config_value, str) or isinstance(config_value, int):
-            self.append(self.data_type(config_value))
+            self.append(self.transform_supported_data(self.transform, config_value, self.valid_values))
         else:
-            self.append(self.data_type(config_value, key, compose_path))
+            self.append(self.transform(config_value, key, compose_path))
```

### Comparing `pycomposefile-0.0.8/setup.py` & `pycomposefile-0.0.9/setup.py`

 * *Files identical despite different names*

