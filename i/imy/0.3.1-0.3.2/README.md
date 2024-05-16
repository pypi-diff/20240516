# Comparing `tmp/imy-0.3.1.tar.gz` & `tmp/imy-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imy-0.3.1.tar", max compression
+gzip compressed data, was "imy-0.3.2.tar", max compression
```

## Comparing `imy-0.3.1.tar` & `imy-0.3.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1059 2024-03-07 06:41:37.092412 imy-0.3.1/LICENSE
--rw-r--r--   0        0        0      202 2024-02-09 18:31:32.595945 imy-0.3.1/README.md
--rw-r--r--   0        0        0        0 2024-04-22 13:27:52.000000 imy-0.3.1/imy/__init__.py
--rw-r--r--   0        0        0     6727 2024-04-26 06:20:02.579623 imy-0.3.1/imy/assets.py
--rw-r--r--   0        0        0     6395 2024-04-29 15:43:18.799268 imy-0.3.1/imy/async_utils.py
--rw-r--r--   0        0        0     9840 2024-04-22 13:49:54.000000 imy-0.3.1/imy/config.py
--rw-r--r--   0        0        0     1112 2024-04-29 16:01:49.458562 imy-0.3.1/imy/docstrings/__init__.py
--rw-r--r--   0        0        0     6498 2024-04-28 15:53:31.243915 imy-0.3.1/imy/docstrings/data_models.py
--rw-r--r--   0        0        0    18387 2024-05-10 11:07:00.691935 imy-0.3.1/imy/docstrings/parsers.py
--rw-r--r--   0        0        0     8578 2024-04-25 19:05:06.904544 imy-0.3.1/imy/inject.py
--rw-r--r--   0        0        0    14594 2024-04-29 15:43:49.552681 imy-0.3.1/imy/logs.py
--rw-r--r--   0        0        0     3185 2024-04-22 13:27:52.000000 imy-0.3.1/imy/package_metadata.py
--rw-r--r--   0        0        0      753 2024-05-10 11:08:02.772084 imy-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      970 1970-01-01 00:00:00.000000 imy-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1059 2024-03-07 06:41:37.092412 imy-0.3.2/LICENSE
+-rw-r--r--   0        0        0      202 2024-02-09 18:31:32.595945 imy-0.3.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-22 13:27:52.000000 imy-0.3.2/imy/__init__.py
+-rw-r--r--   0        0        0     6727 2024-04-26 06:20:02.579623 imy-0.3.2/imy/assets.py
+-rw-r--r--   0        0        0     6395 2024-04-29 15:43:18.799268 imy-0.3.2/imy/async_utils.py
+-rw-r--r--   0        0        0     9840 2024-04-22 13:49:54.000000 imy-0.3.2/imy/config.py
+-rw-r--r--   0        0        0     1112 2024-04-29 16:01:49.458562 imy-0.3.2/imy/docstrings/__init__.py
+-rw-r--r--   0        0        0     6538 2024-05-16 08:25:56.236283 imy-0.3.2/imy/docstrings/data_models.py
+-rw-r--r--   0        0        0    18612 2024-05-16 08:25:56.236283 imy-0.3.2/imy/docstrings/parsers.py
+-rw-r--r--   0        0        0     8578 2024-04-25 19:05:06.904544 imy-0.3.2/imy/inject.py
+-rw-r--r--   0        0        0    14594 2024-04-29 15:43:49.552681 imy-0.3.2/imy/logs.py
+-rw-r--r--   0        0        0     3185 2024-04-22 13:27:52.000000 imy-0.3.2/imy/package_metadata.py
+-rw-r--r--   0        0        0      753 2024-05-16 08:25:59.966294 imy-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      970 1970-01-01 00:00:00.000000 imy-0.3.2/PKG-INFO
```

### Comparing `imy-0.3.1/LICENSE` & `imy-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `imy-0.3.1/imy/assets.py` & `imy-0.3.2/imy/assets.py`

 * *Files identical despite different names*

### Comparing `imy-0.3.1/imy/async_utils.py` & `imy-0.3.2/imy/async_utils.py`

 * *Files identical despite different names*

### Comparing `imy-0.3.1/imy/config.py` & `imy-0.3.2/imy/config.py`

 * *Files identical despite different names*

### Comparing `imy-0.3.1/imy/docstrings/__init__.py` & `imy-0.3.2/imy/docstrings/__init__.py`

 * *Files identical despite different names*

### Comparing `imy-0.3.1/imy/docstrings/data_models.py` & `imy-0.3.2/imy/docstrings/data_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,14 +205,16 @@
 
 @dataclass
 class FunctionDocs:
     """
     A docstring specifically for functions and methods.
     """
 
+    object: Callable
+
     name: str
     parameters: list[FunctionParameter]
     return_type: introspection.types.TypeAnnotation | Unset
     synchronous: bool
 
     summary: str | None
     details: str | None
@@ -242,14 +244,16 @@
 
 @dataclass
 class ClassDocs:
     """
     A docstring specifically for classes.
     """
 
+    object: type
+
     name: str
     attributes: list[ClassField]
     functions: list[FunctionDocs]
 
     summary: str | None
     details: str | None
```

### Comparing `imy-0.3.1/imy/docstrings/parsers.py` & `imy-0.3.2/imy/docstrings/parsers.py`

 * *Files 0% similar despite different names*

```diff
@@ -364,14 +364,15 @@
         # Parse the metadata
         metadata = data_models.FunctionMetadata.from_dictionary(
             parsed.key_sections["metadata"]
         )
 
     # Build the result
     return data_models.FunctionDocs(
+        object=func,
         name=func.__name__,
         parameters=list(parameters.values()),
         return_type=parse_annotation(signature.return_annotation),
         synchronous=not inspect.iscoroutinefunction(func),
         summary=parsed.summary,
         details=parsed.details,
         raises=raises,
@@ -526,17 +527,20 @@
     )
 
     # Add any information learned about fields from the docstring
     for field_name, field_details in docs.key_sections["attributes"].items():
         try:
             result_field = fields_by_name[field_name]
         except KeyError:
-            warnings.warn(
-                f"The docstring for class `{cls.__name__}` mentions a field `{field_name}` that does not exist in the class."
-            )
+            # Warn about the missing field, unless there's a property with that
+            # name
+            if not isinstance(getattr(cls, field_name, None), property):
+                warnings.warn(
+                    f"The docstring for class `{cls.__name__}` mentions a field `{field_name}` that does not exist in the class."
+                )
             continue
 
         result_field.description = field_details
 
     # If `__init__` is missing documentation for any parameters, try to copy the
     # values from matching fields.
     for func_docs in functions_by_name.values():
@@ -554,14 +558,15 @@
 
             param.description = field.description
 
         break
 
     # Build the result
     return data_models.ClassDocs(
+        object=cls,
         name=cls.__name__,
         attributes=list(fields_by_name.values()),
         functions=list(functions_by_name.values()),
         summary=docs.summary,
         details=docs.details,
         metadata=data_models.ClassMetadata.from_dictionary(
             docs.key_sections["metadata"]
```

### Comparing `imy-0.3.1/imy/inject.py` & `imy-0.3.2/imy/inject.py`

 * *Files identical despite different names*

### Comparing `imy-0.3.1/imy/logs.py` & `imy-0.3.2/imy/logs.py`

 * *Files identical despite different names*

### Comparing `imy-0.3.1/imy/package_metadata.py` & `imy-0.3.2/imy/package_metadata.py`

 * *Files identical despite different names*

### Comparing `imy-0.3.1/pyproject.toml` & `imy-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "imy"
-version = "0.3.1"
+version = "0.3.2"
 description = "Random utilities I can't go without"
 authors = ["Jakob Pinterits <jakob.pinterits@gmail.com>"]
 license = "MIT"
 repository = "https://gitlab.com/Vivern/i-miss-you"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `imy-0.3.1/PKG-INFO` & `imy-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imy
-Version: 0.3.1
+Version: 0.3.2
 Summary: Random utilities I can't go without
 Home-page: https://gitlab.com/Vivern/i-miss-you
 License: MIT
 Author: Jakob Pinterits
 Author-email: jakob.pinterits@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

