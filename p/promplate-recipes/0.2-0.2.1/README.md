# Comparing `tmp/promplate_recipes-0.2.tar.gz` & `tmp/promplate_recipes-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promplate_recipes-0.2.tar", last modified: Thu May 16 12:08:55 2024, max compression
+gzip compressed data, was "promplate_recipes-0.2.1.tar", last modified: Thu May 16 12:22:52 2024, max compression
```

## Comparing `promplate_recipes-0.2.tar` & `promplate_recipes-0.2.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      200 2024-04-10 06:40:35.413855 promplate_recipes-0.2/promplate_recipes/__init__.py
--rw-r--r--   0        0        0     2017 2024-05-16 12:08:32.913071 promplate_recipes-0.2/promplate_recipes/context.py
--rw-r--r--   0        0        0       46 2024-05-16 11:12:22.101605 promplate_recipes-0.2/promplate_recipes/version.py
--rw-r--r--   0        0        0      689 2024-05-16 12:08:55.488102 promplate_recipes-0.2/pyproject.toml
--rw-r--r--   0        0        0      206 1970-01-01 00:00:00.000000 promplate_recipes-0.2/PKG-INFO
+-rw-r--r--   0        0        0      200 2024-04-10 06:40:35.413855 promplate_recipes-0.2.1/promplate_recipes/__init__.py
+-rw-r--r--   0        0        0     2191 2024-05-16 12:21:26.190215 promplate_recipes-0.2.1/promplate_recipes/context.py
+-rw-r--r--   0        0        0       48 2024-05-16 12:21:52.594227 promplate_recipes-0.2.1/promplate_recipes/version.py
+-rw-r--r--   0        0        0      691 2024-05-16 12:22:52.390233 promplate_recipes-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      208 1970-01-01 00:00:00.000000 promplate_recipes-0.2.1/PKG-INFO
```

### Comparing `promplate_recipes-0.2/promplate_recipes/context.py` & `promplate_recipes-0.2.1/promplate_recipes/context.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,20 @@
 
 
 @partial(partial, default_box=True)
 class SilentBox(Box):
     def __str__(self):
         return super().__str__() if len(self) else ""
 
+    if __debug__:
+
+        def __call__(self, *args, **kwargs):
+            print(f"{self.__class__} shouldn't be called {args = } {kwargs = }")
+            return ""
+
 
 class BuiltinsLayer(dict):
     def __getitem__(self, key):
         return get_builtins()[key]
 
     def __contains__(self, key):
         return key in get_builtins()
```

### Comparing `promplate_recipes-0.2/pyproject.toml` & `promplate_recipes-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     { name = "Muspi Merol", email = "me@promplate.dev" },
 ]
 dependencies = [
     "promplate~=0.3.4",
     "python-box~=7.1.1",
 ]
 requires-python = ">=3.10"
-version = "0.2"
+version = "0.2.1"
 
 [project.license]
 text = "MIT"
 
 [tool.pdm]
 distribution = true
```

