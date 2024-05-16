# Comparing `tmp/gson-0.0.2.tar.gz` & `tmp/gson-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gson-0.0.2.tar", last modified: Fri Nov 18 05:31:05 2022, max compression
+gzip compressed data, was "gson-0.0.3.tar", last modified: Fri Nov 18 06:02:30 2022, max compression
```

## Comparing `gson-0.0.2.tar` & `gson-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 cruise    (1000) cruise    (1000)        0 2022-11-18 06:59:21.159090 gson-0.0.2/
--rwxrwxrwx   0 cruise    (1000) cruise    (1000)     1066 2022-11-18 06:11:16.000000 gson-0.0.2/LICENSE
--rwxrwxrwx   0 cruise    (1000) cruise    (1000)      445 2022-11-18 06:59:21.156570 gson-0.0.2/PKG-INFO
--rwxrwxrwx   0 cruise    (1000) cruise    (1000)       89 2022-11-18 06:11:16.000000 gson-0.0.2/README.md
--rwxrwxrwx   0 cruise    (1000) cruise    (1000)      574 2022-11-18 06:59:13.000000 gson-0.0.2/pyproject.toml
--rwxrwxrwx   0 cruise    (1000) cruise    (1000)       38 2022-11-18 06:59:21.160093 gson-0.0.2/setup.cfg
-drwxrwxrwx   0 cruise    (1000) cruise    (1000)        0 2022-11-18 06:59:20.926146 gson-0.0.2/src/
-drwxrwxrwx   0 cruise    (1000) cruise    (1000)        0 2022-11-18 06:59:20.996149 gson-0.0.2/src/decorators/
--rwxrwxrwx   0 cruise    (1000) cruise    (1000)      392 2022-11-18 06:11:16.000000 gson-0.0.2/src/decorators/safe_run.py
-drwxrwxrwx   0 cruise    (1000) cruise    (1000)        0 2022-11-18 06:59:21.042617 gson-0.0.2/src/gson/
--rwxrwxrwx   0 cruise    (1000) cruise    (1000)       23 2022-11-18 06:11:16.000000 gson-0.0.2/src/gson/__init__.py
--rwxrwxrwx   0 cruise    (1000) cruise    (1000)     7781 2022-11-18 06:33:16.000000 gson-0.0.2/src/gson/gmarshal.py
-drwxrwxrwx   0 cruise    (1000) cruise    (1000)        0 2022-11-18 06:59:21.129264 gson-0.0.2/src/gson.egg-info/
--rwxrwxrwx   0 cruise    (1000) cruise    (1000)      445 2022-11-18 06:59:20.000000 gson-0.0.2/src/gson.egg-info/PKG-INFO
--rwxrwxrwx   0 cruise    (1000) cruise    (1000)      229 2022-11-18 06:59:20.000000 gson-0.0.2/src/gson.egg-info/SOURCES.txt
--rwxrwxrwx   0 cruise    (1000) cruise    (1000)        1 2022-11-18 06:59:20.000000 gson-0.0.2/src/gson.egg-info/dependency_links.txt
--rwxrwxrwx   0 cruise    (1000) cruise    (1000)       16 2022-11-18 06:59:20.000000 gson-0.0.2/src/gson.egg-info/top_level.txt
+drwxrwxrwx   0 cruise    (1000) cruise    (1000)        0 2022-11-18 07:30:45.739569 gson-0.0.3/
+-rwxrwxrwx   0 cruise    (1000) cruise    (1000)     1066 2022-11-18 06:11:16.000000 gson-0.0.3/LICENSE
+-rwxrwxrwx   0 cruise    (1000) cruise    (1000)      445 2022-11-18 07:30:45.737492 gson-0.0.3/PKG-INFO
+-rwxrwxrwx   0 cruise    (1000) cruise    (1000)       89 2022-11-18 06:11:16.000000 gson-0.0.3/README.md
+-rwxrwxrwx   0 cruise    (1000) cruise    (1000)      574 2022-11-18 07:30:07.000000 gson-0.0.3/pyproject.toml
+-rwxrwxrwx   0 cruise    (1000) cruise    (1000)       38 2022-11-18 07:30:45.740806 gson-0.0.3/setup.cfg
+drwxrwxrwx   0 cruise    (1000) cruise    (1000)        0 2022-11-18 07:30:45.565194 gson-0.0.3/src/
+drwxrwxrwx   0 cruise    (1000) cruise    (1000)        0 2022-11-18 07:30:45.612913 gson-0.0.3/src/decorators/
+-rwxrwxrwx   0 cruise    (1000) cruise    (1000)      392 2022-11-18 06:11:16.000000 gson-0.0.3/src/decorators/safe_run.py
+drwxrwxrwx   0 cruise    (1000) cruise    (1000)        0 2022-11-18 07:30:45.650482 gson-0.0.3/src/gson/
+-rwxrwxrwx   0 cruise    (1000) cruise    (1000)       23 2022-11-18 06:11:16.000000 gson-0.0.3/src/gson/__init__.py
+-rwxrwxrwx   0 cruise    (1000) cruise    (1000)     8054 2022-11-18 07:21:13.000000 gson-0.0.3/src/gson/gmarshal.py
+drwxrwxrwx   0 cruise    (1000) cruise    (1000)        0 2022-11-18 07:30:45.720856 gson-0.0.3/src/gson.egg-info/
+-rwxrwxrwx   0 cruise    (1000) cruise    (1000)      445 2022-11-18 07:30:45.000000 gson-0.0.3/src/gson.egg-info/PKG-INFO
+-rwxrwxrwx   0 cruise    (1000) cruise    (1000)      229 2022-11-18 07:30:45.000000 gson-0.0.3/src/gson.egg-info/SOURCES.txt
+-rwxrwxrwx   0 cruise    (1000) cruise    (1000)        1 2022-11-18 07:30:45.000000 gson-0.0.3/src/gson.egg-info/dependency_links.txt
+-rwxrwxrwx   0 cruise    (1000) cruise    (1000)       16 2022-11-18 07:30:45.000000 gson-0.0.3/src/gson.egg-info/top_level.txt
```

### Comparing `gson-0.0.2/LICENSE` & `gson-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gson-0.0.2/pyproject.toml` & `gson-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gson"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Cruise Li", email="lhrotk@gmail.com" },
 ]
 description = "Json Encode/Decoder in Golang Style"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `gson-0.0.2/src/gson/gmarshal.py` & `gson-0.0.3/src/gson/gmarshal.py`

 * *Files 2% similar despite different names*

```diff
@@ -229,14 +229,21 @@
         if some_cls == type(some_json):
             return some_json
         elif some_cls == int and isinstance(some_json, str):
             try:
                 return int(some_json)
             finally:
                 pass
+        elif some_cls == bool:
+            if isinstance(some_json, str):
+                if some_json.lower() == "true":
+                    return True
+                elif some_json.lower() == "false":
+                    return False
+            return bool(some_json)
         else:
             logger.warning(f"Type miss match, field stack: {keys}")
     return None
 
 
 T = TypeVar("T")
```

