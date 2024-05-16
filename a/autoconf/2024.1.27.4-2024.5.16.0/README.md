# Comparing `tmp/autoconf-2024.1.27.4.tar.gz` & `tmp/autoconf-2024.5.16.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoconf-2024.1.27.4.tar", last modified: Sat Jan 27 19:56:36 2024, max compression
+gzip compressed data, was "autoconf-2024.5.16.0.tar", last modified: Thu May 16 09:56:26 2024, max compression
```

## Comparing `autoconf-2024.1.27.4.tar` & `autoconf-2024.5.16.0.tar`

### file list

```diff
@@ -1,28 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:36.528590 autoconf-2024.1.27.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-01-27 19:56:29.000000 autoconf-2024.1.27.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-01-27 19:56:29.000000 autoconf-2024.1.27.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-01-27 19:56:36.528590 autoconf-2024.1.27.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-01-27 19:56:29.000000 autoconf-2024.1.27.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:36.524590 autoconf-2024.1.27.4/autoconf/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-01-27 19:56:29.000000 autoconf-2024.1.27.4/autoconf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-01-27 19:56:29.000000 autoconf-2024.1.27.4/autoconf/class_path.py
--rw-r--r--   0 runner    (1001) docker     (127)    10747 2024-01-27 19:56:29.000000 autoconf-2024.1.27.4/autoconf/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-01-27 19:56:29.000000 autoconf-2024.1.27.4/autoconf/dictable.py
--rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-01-27 19:56:29.000000 autoconf-2024.1.27.4/autoconf/directory_config.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-01-27 19:56:29.000000 autoconf-2024.1.27.4/autoconf/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:36.528590 autoconf-2024.1.27.4/autoconf/json_prior/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:29.000000 autoconf-2024.1.27.4/autoconf/json_prior/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6536 2024-01-27 19:56:29.000000 autoconf-2024.1.27.4/autoconf/json_prior/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-01-27 19:56:29.000000 autoconf-2024.1.27.4/autoconf/json_prior/generate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:36.528590 autoconf-2024.1.27.4/autoconf/mock/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:29.000000 autoconf-2024.1.27.4/autoconf/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-01-27 19:56:29.000000 autoconf-2024.1.27.4/autoconf/mock/mock_real.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-01-27 19:56:29.000000 autoconf-2024.1.27.4/autoconf/output.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:36.528590 autoconf-2024.1.27.4/autoconf/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:29.000000 autoconf-2024.1.27.4/autoconf/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-01-27 19:56:29.000000 autoconf-2024.1.27.4/autoconf/tools/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:36.528590 autoconf-2024.1.27.4/autoconf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-01-27 19:56:36.000000 autoconf-2024.1.27.4/autoconf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-01-27 19:56:29.000000 autoconf-2024.1.27.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-01-27 19:56:36.528590 autoconf-2024.1.27.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-01-27 19:56:29.000000 autoconf-2024.1.27.4/setup.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:56:26.598328 autoconf-2024.5.16.0/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:56:26.532961 autoconf-2024.5.16.0/.github/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:56:26.552943 autoconf-2024.5.16.0/.github/workflows/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1241 2023-10-16 15:46:48.000000 autoconf-2024.5.16.0/.github/workflows/main.yml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18883 2022-12-19 11:17:33.000000 autoconf-2024.5.16.0/CODE_OF_CONDUCT.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1091 2020-11-16 18:50:14.000000 autoconf-2024.5.16.0/LICENSE
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      498 2022-03-30 15:09:13.000000 autoconf-2024.5.16.0/MANIFEST.in
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      775 2024-05-16 09:56:26.598328 autoconf-2024.5.16.0/PKG-INFO
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       14 2020-11-16 18:50:14.000000 autoconf-2024.5.16.0/README.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:56:26.568015 autoconf-2024.5.16.0/autoconf/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      346 2024-05-16 09:55:27.000000 autoconf-2024.5.16.0/autoconf/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1425 2023-01-10 08:25:59.000000 autoconf-2024.5.16.0/autoconf/class_path.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10977 2024-04-22 13:02:16.000000 autoconf-2024.5.16.0/autoconf/conf.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8476 2024-04-22 13:02:16.000000 autoconf-2024.5.16.0/autoconf/dictable.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6511 2024-03-12 16:16:47.000000 autoconf-2024.5.16.0/autoconf/directory_config.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       93 2021-02-08 19:43:27.000000 autoconf-2024.5.16.0/autoconf/exc.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:56:26.575739 autoconf-2024.5.16.0/autoconf/json_prior/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2020-11-10 18:01:19.000000 autoconf-2024.5.16.0/autoconf/json_prior/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6536 2022-11-29 14:08:25.000000 autoconf-2024.5.16.0/autoconf/json_prior/config.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2121 2023-01-10 08:25:59.000000 autoconf-2024.5.16.0/autoconf/json_prior/generate.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:56:26.580865 autoconf-2024.5.16.0/autoconf/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-03-01 14:51:44.000000 autoconf-2024.5.16.0/autoconf/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1918 2023-01-10 08:25:59.000000 autoconf-2024.5.16.0/autoconf/mock/mock_real.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1577 2023-11-17 15:33:42.000000 autoconf-2024.5.16.0/autoconf/output.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:56:26.585199 autoconf-2024.5.16.0/autoconf/tools/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-09-01 16:48:20.000000 autoconf-2024.5.16.0/autoconf/tools/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      657 2024-01-22 19:50:10.000000 autoconf-2024.5.16.0/autoconf/tools/decorators.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:56:26.597242 autoconf-2024.5.16.0/autoconf.egg-info/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      576 2024-05-16 09:56:26.000000 autoconf-2024.5.16.0/autoconf.egg-info/SOURCES.txt
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       38 2022-02-07 19:21:33.000000 autoconf-2024.5.16.0/eden.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       58 2023-10-16 15:46:48.000000 autoconf-2024.5.16.0/requirements.txt
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:56:26.595242 autoconf-2024.5.16.0/scripts/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      758 2022-11-29 18:29:27.000000 autoconf-2024.5.16.0/scripts/convert_config.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1108 2022-12-02 15:56:28.000000 autoconf-2024.5.16.0/scripts/convert_prior_configs.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      518 2023-01-10 08:25:59.000000 autoconf-2024.5.16.0/scripts/edenise.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      334 2020-11-16 18:50:14.000000 autoconf-2024.5.16.0/scripts/generate_priors.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       63 2024-05-16 09:56:26.599362 autoconf-2024.5.16.0/setup.cfg
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1487 2024-05-16 09:56:09.000000 autoconf-2024.5.16.0/setup.py
```

### Comparing `autoconf-2024.1.27.4/LICENSE` & `autoconf-2024.5.16.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autoconf-2024.1.27.4/PKG-INFO` & `autoconf-2024.5.16.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoconf
-Version: 2024.1.27.4
+Version: 2024.5.16.0
 Summary: PyAuto Configration
 Home-page: https://github.com/rhayes777/PyAutoConf
 Author: James Nightingale and Richard Hayes
 Author-email: richard@rghsoftware.co.uk
 License: MIT License
 Keywords: cli
 Classifier: Intended Audience :: Science/Research
@@ -14,13 +14,9 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: typing-inspect>=0.4.0
-Requires-Dist: pathlib
-Requires-Dist: PyYAML>=6.0.1
-Requires-Dist: numpy<=1.26.0
 
 # PyAutoConf
```

### Comparing `autoconf-2024.1.27.4/autoconf/class_path.py` & `autoconf-2024.5.16.0/autoconf/class_path.py`

 * *Files identical despite different names*

### Comparing `autoconf-2024.1.27.4/autoconf/conf.py` & `autoconf-2024.5.16.0/autoconf/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -330,14 +330,18 @@
             return result
 
         return wrapper
 
     return decorator
 
 
+class NoValue:
+    pass
+
+
 def with_config(*path: str, value):
     """
     Create a decorator that swaps a value in configuration
     defined by path for the scope of a test.
 
     Parameters
     ----------
@@ -354,19 +358,26 @@
     def decorator(func):
         @wraps(func)
         def wrapper(*args, **kwargs):
             config = instance
             for string in path[:-1]:
                 config = config[string]
 
-            original_value = config[path[-1]]
+            try:
+                original_value = config[path[-1]]
+            except KeyError:
+                original_value = NoValue
+
             config[path[-1]] = value
 
             result = func(*args, **kwargs)
 
-            config[path[-1]] = original_value
+            if original_value is NoValue:
+                del config[path[-1]]
+            else:
+                config[path[-1]] = original_value
 
             return result
 
         return wrapper
 
     return decorator
```

### Comparing `autoconf-2024.1.27.4/autoconf/dictable.py` & `autoconf-2024.5.16.0/autoconf/dictable.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import inspect
 import json
 import logging
 
 import numpy as np
 from pathlib import Path
-from typing import Union, Callable
+from typing import Union, Callable, Set, Tuple
 
 from autoconf.class_path import get_class_path, get_class
 
 logger = logging.getLogger(__name__)
 
 
 np_type_map = {
@@ -31,68 +31,150 @@
 def nd_array_from_dict(nd_array_dict: dict, **_) -> np.ndarray:
     """
     Converts a dictionary representation back to a numpy array.
     """
     return np.array(nd_array_dict["array"], dtype=getattr(np, nd_array_dict["dtype"]))
 
 
-def to_dict(obj):
+def is_array(obj) -> bool:
+    """
+    True if the object is a numpy array or an ArrayImpl (i.e. from JAX)
+    """
+    if isinstance(obj, np.ndarray):
+        return True
+    try:
+        return obj.__class__.__name__ == "ArrayImpl"
+    except AttributeError:
+        return False
+
+
+def to_dict(obj, filter_args: Tuple[str, ...] = ()) -> dict:
     if isinstance(obj, (int, float, str, bool, type(None))):
         return obj
 
     if hasattr(obj, "dict"):
         try:
             return obj.dict()
         except TypeError as e:
             logger.debug(e)
 
-    if isinstance(obj, np.ndarray):
+    if is_array(obj):
         try:
             return nd_array_as_dict(obj)
         except Exception as e:
             logger.info(e)
 
+    if isinstance(obj, Path):
+        return {
+            "type": "path",
+            "path": str(obj),
+        }
+
     if inspect.isclass(obj):
         return {
             "type": "type",
             "class_path": get_class_path(obj),
         }
 
     if isinstance(obj, list):
         return {"type": "list", "values": list(map(to_dict, obj))}
     if isinstance(obj, dict):
         return {
             "type": "dict",
-            "arguments": {key: to_dict(value) for key, value in obj.items()},
+            "arguments": {
+                key: to_dict(value)
+                for key, value in obj.items()
+                if key not in filter_args
+            },
         }
     if obj.__class__.__name__ == "method":
         return to_dict(obj())
     if obj.__class__.__module__ == "builtins":
         return obj
 
     if inspect.isclass(type(obj)):
-        return instance_as_dict(obj)
+        return instance_as_dict(obj, filter_args=filter_args)
 
     return obj
 
 
-def instance_as_dict(obj):
-    arguments = set(inspect.getfullargspec(obj.__init__).args[1:])
+def get_arguments(obj) -> Set[str]:
+    """
+    Get the arguments of a class. This is done by inspecting the constructor.
+
+    If the constructor has a **kwargs parameter, the arguments of the base classes are also included.
+
+    Parameters
+    ----------
+    obj
+        The class to get the arguments of.
+
+    Returns
+    -------
+    A set of the arguments of the class.
+    """
+    args_spec = inspect.getfullargspec(obj.__init__)
+    args = set(args_spec.args[1:])
+    if args_spec.varkw:
+        for base in obj.__bases__:
+            if base is object:
+                continue
+            args |= get_arguments(base)
+    return args
+
+
+def instance_as_dict(obj, filter_args: Tuple[str, ...] = ()):
+    """
+    Convert an instance of a class to a dictionary representation.
+
+    Serialises any children of the object which are given as constructor arguments
+    or included in the __identifier_fields__ attribute.
+
+    Sets any fields in the __nullify_fields__ attribute to None.
+
+    Parameters
+    ----------
+    obj
+        The instance of the class to be converted to a dictionary representation.
+    filter_args
+        A tuple of arguments to exclude from the dictionary representation.
+
+    Returns
+    -------
+    A dictionary representation of the instance.
+    """
+    arguments = get_arguments(type(obj))
     try:
         arguments |= set(obj.__identifier_fields__)
     except (AttributeError, TypeError):
         pass
+
     argument_dict = {
         arg: getattr(obj, arg)
         for arg in arguments
+        if arg not in filter_args
         if hasattr(obj, arg)
         and not inspect.ismethod(
             getattr(obj, arg),
         )
     }
+    try:
+        for field in obj.__nullify_fields__:
+            argument_dict[field] = None
+    except (AttributeError, TypeError):
+        pass
+
+    try:
+        for field in obj.__exclude_fields__:
+            try:
+                argument_dict.pop(field)
+            except KeyError:
+                logger.debug(f"Field {field} not found in object")
+    except (AttributeError, TypeError):
+        pass
 
     return {
         "type": "instance",
         "class_path": get_class_path(obj.__class__),
         "arguments": {key: to_dict(value) for key, value in argument_dict.items()},
     }
 
@@ -161,14 +243,17 @@
     except KeyError:
         logger.debug("No type field in dictionary")
         return dictionary
     except TypeError as e:
         logger.debug(e)
         return None
 
+    if type_ == "path":
+        return Path(dictionary["path"])
+
     if type_ in __parsers:
         return __parsers[type_](dictionary, **kwargs)
 
     if type_ == "list":
         return list(map(from_dict, dictionary["values"]))
     if type_ == "dict":
         return {key: from_dict(value, **kwargs) for key, value in dictionary.items()}
```

### Comparing `autoconf-2024.1.27.4/autoconf/directory_config.py` & `autoconf-2024.5.16.0/autoconf/directory_config.py`

 * *Files identical despite different names*

### Comparing `autoconf-2024.1.27.4/autoconf/json_prior/config.py` & `autoconf-2024.5.16.0/autoconf/json_prior/config.py`

 * *Files identical despite different names*

### Comparing `autoconf-2024.1.27.4/autoconf/json_prior/generate.py` & `autoconf-2024.5.16.0/autoconf/json_prior/generate.py`

 * *Files identical despite different names*

### Comparing `autoconf-2024.1.27.4/autoconf/mock/mock_real.py` & `autoconf-2024.5.16.0/autoconf/mock/mock_real.py`

 * *Files identical despite different names*

### Comparing `autoconf-2024.1.27.4/autoconf/output.py` & `autoconf-2024.5.16.0/autoconf/output.py`

 * *Files identical despite different names*

### Comparing `autoconf-2024.1.27.4/autoconf/tools/decorators.py` & `autoconf-2024.5.16.0/autoconf/tools/decorators.py`

 * *Files identical despite different names*

### Comparing `autoconf-2024.1.27.4/setup.py` & `autoconf-2024.5.16.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     long_description = file.read()
 
 with open(join(this_dir, "requirements.txt")) as f:
     requirements = f.read().split("\n")
 
 setup(
     name="autoconf",
-    version=environ.get("VERSION", "1.0.dev0"),
+    version=environ.get("VERSION", "2024.5.16.0"),
     description="PyAuto Configration",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/rhayes777/PyAutoConf",
     author="James Nightingale and Richard Hayes",
     author_email="richard@rghsoftware.co.uk",
     include_package_data=True,
```

