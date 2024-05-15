# Comparing `tmp/update_toml-0.1.0.tar.gz` & `tmp/update_toml-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "update_toml-0.1.0.tar", max compression
+gzip compressed data, was "update_toml-0.2.0.tar", max compression
```

## Comparing `update_toml-0.1.0.tar` & `update_toml-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      322 2024-05-15 22:53:35.174960 update_toml-0.1.0/README.md
--rw-r--r--   0        0        0      610 2024-05-15 22:53:43.677886 update_toml-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1009 2024-05-15 22:52:43.134329 update_toml-0.1.0/update_toml/cli_input_handler.py
--rw-r--r--   0        0        0       50 2024-05-15 22:39:14.752166 update_toml-0.1.0/update_toml/exceptions/file_not_loaded_exception.py
--rw-r--r--   0        0        0      160 2024-05-15 22:39:14.752365 update_toml-0.1.0/update_toml/interfaces/input_handler.py
--rw-r--r--   0        0        0      825 2024-05-15 22:39:14.752514 update_toml-0.1.0/update_toml/main.py
--rw-r--r--   0        0        0      112 2024-05-15 22:39:14.752715 update_toml-0.1.0/update_toml/models/user_input.py
--rw-r--r--   0        0        0     2342 2024-05-15 22:49:21.710456 update_toml-0.1.0/update_toml/toml_file.py
--rw-r--r--   0        0        0      973 1970-01-01 00:00:00.000000 update_toml-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      624 2024-05-15 23:37:19.556266 update_toml-0.2.0/README.md
+-rw-r--r--   0        0        0      610 2024-05-15 23:36:17.635046 update_toml-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2670 2024-05-15 23:36:05.230929 update_toml-0.2.0/update_toml/cli_input_handler.py
+-rw-r--r--   0        0        0       50 2024-05-15 22:39:14.752166 update_toml-0.2.0/update_toml/exceptions/file_not_loaded_exception.py
+-rw-r--r--   0        0        0      160 2024-05-15 22:39:14.752365 update_toml-0.2.0/update_toml/interfaces/input_handler.py
+-rw-r--r--   0        0        0     1098 2024-05-15 23:33:24.929342 update_toml-0.2.0/update_toml/main.py
+-rw-r--r--   0        0        0      156 2024-05-15 23:25:11.696767 update_toml-0.2.0/update_toml/models/user_input.py
+-rw-r--r--   0        0        0     3026 2024-05-15 23:31:43.826383 update_toml-0.2.0/update_toml/toml_file.py
+-rw-r--r--   0        0        0     1275 1970-01-01 00:00:00.000000 update_toml-0.2.0/PKG-INFO
```

### Comparing `update_toml-0.1.0/pyproject.toml` & `update_toml-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "update_toml"
-version = "0.1.0"
+version = "0.2.0"
 description = "Update a toml value from a CLI"
 authors = ["Jake Cyr <cyrjake@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 keywords = ["toml", "requirements", "update"]
 
 [tool.poetry.dependencies]
```

### Comparing `update_toml-0.1.0/update_toml/toml_file.py` & `update_toml-0.2.0/update_toml/toml_file.py`

 * *Files 16% similar despite different names*

```diff
@@ -34,14 +34,35 @@
                 "Path should have at least two parts (ex. project.version)"
             )
 
         parent_object: dict = self._get_parent_object(path_parts, self._contents)
         property_to_update: str = path_parts[0]
         parent_object[property_to_update] = new_value
 
+    def path_exists(self, path: str) -> bool:
+        if self._contents is None:
+            raise FileNotLoadedException("load has not yet been called")
+
+        try:
+            path_parts: list[str] = path.split(".")
+            self._get_value(path_parts, self._contents)
+            return True
+        except KeyError:
+            return False
+
+    def get_value_safe(self, path: str) -> str:
+        if self._contents is None:
+            raise FileNotLoadedException("load has not yet been called")
+
+        try:
+            path_parts: list[str] = path.split(".")
+            return self._get_value(path_parts, self._contents)
+        except KeyError:
+            return ""
+
     def get_value(self, path: str) -> str:
         if self._contents is None:
             raise FileNotLoadedException("load has not yet been called")
 
         path_parts: list[str] = path.split(".")
         return self._get_value(path_parts, self._contents)
```

