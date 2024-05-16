# Comparing `tmp/rfc9457-0.0.1.tar.gz` & `tmp/rfc9457-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfc9457-0.0.1.tar", max compression
+gzip compressed data, was "rfc9457-0.0.2.tar", max compression
```

## Comparing `rfc9457-0.0.1.tar` & `rfc9457-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11307 2024-05-16 06:44:12.192758 rfc9457-0.0.1/LICENSE
--rw-r--r--   0        0        0     1789 2024-05-16 06:44:12.192758 rfc9457-0.0.1/README.md
--rw-r--r--   0        0        0     2021 2024-05-16 06:44:12.192758 rfc9457-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2429 2024-05-16 06:44:12.192758 rfc9457-0.0.1/src/rfc9457/__init__.py
--rw-r--r--   0        0        0     2451 1970-01-01 00:00:00.000000 rfc9457-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11307 2024-05-16 06:47:10.052792 rfc9457-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1789 2024-05-16 06:47:10.052792 rfc9457-0.0.2/README.md
+-rw-r--r--   0        0        0     2021 2024-05-16 06:47:10.052792 rfc9457-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2581 2024-05-16 06:47:10.052792 rfc9457-0.0.2/src/rfc9457/__init__.py
+-rw-r--r--   0        0        0     2451 1970-01-01 00:00:00.000000 rfc9457-0.0.2/PKG-INFO
```

### Comparing `rfc9457-0.0.1/LICENSE` & `rfc9457-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rfc9457-0.0.1/README.md` & `rfc9457-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `rfc9457-0.0.1/pyproject.toml` & `rfc9457-0.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rfc9457"
-version = "0.0.1"
+version = "0.0.2"
 description = "Implementation of RFC9457 problems."
 authors = ["Daniel Edgecombe <daniel@nrwl.co>"]
 license = "Apache-2.0"
 repository="https://github.com/NRWLDev/rfc9457/"
 homepage="https://github.com/NRWLDev/rfc9457/"
 readme = "README.md"
 
@@ -19,15 +19,15 @@
 pytest-random-order = "^1.0"
 
 # Style
 ruff = "^0.3"
 pre-commit = "^3.0.2"
 
 [tool.bumpversion]
-current_version = "0.0.1"
+current_version = "0.0.2"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

### Comparing `rfc9457-0.0.1/src/rfc9457/__init__.py` & `rfc9457-0.0.2/src/rfc9457/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,20 @@
 
 import re
 import typing as t
 
 CONVERT_RE = re.compile(r"(?<!^)(?=[A-Z])")
 
 
+def error_class_to_type(exc: Exception) -> str:
+    """Convert an exception class name to a `problem-type` string."""
+    type_ = "".join(exc.__class__.__name__.rsplit("Error", 1))
+    return CONVERT_RE.sub("-", type_).lower()
+
+
 class Problem(Exception):  # noqa: N818
     """
     A base exception designed to support all API error handling.
     All exceptions should inherit from this or a subclass of it (depending on the usage),
     this will allow all apps and libraries to maintain a common exception chain.
     """
 
@@ -31,16 +37,15 @@
         self.title = title
         self.details = details
         self.status = status
         self.extras = kwargs
 
     @property
     def type(self: t.Self) -> str:
-        type_ = "".join(self.__class__.__name__.rsplit("Error", 1))
-        type_ = CONVERT_RE.sub("-", type_).lower()
+        type_ = error_class_to_type(self)
         return self._type if self._type else type_
 
     def marshal(self: t.Self, *, strip_debug: bool = False) -> dict[str, t.Any]:
         """Generate a JSON compatible representation.
 
         Args:
         ----
```

### Comparing `rfc9457-0.0.1/PKG-INFO` & `rfc9457-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfc9457
-Version: 0.0.1
+Version: 0.0.2
 Summary: Implementation of RFC9457 problems.
 Home-page: https://github.com/NRWLDev/rfc9457/
 License: Apache-2.0
 Author: Daniel Edgecombe
 Author-email: daniel@nrwl.co
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

