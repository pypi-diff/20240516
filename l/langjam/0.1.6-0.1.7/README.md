# Comparing `tmp/langjam-0.1.6.tar.gz` & `tmp/langjam-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langjam-0.1.6.tar", max compression
+gzip compressed data, was "langjam-0.1.7.tar", max compression
```

## Comparing `langjam-0.1.6.tar` & `langjam-0.1.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11356 2024-01-21 09:11:55.610347 langjam-0.1.6/LICENSE
--rw-r--r--   0        0        0      208 2024-02-13 03:22:07.507294 langjam-0.1.6/README.md
--rw-r--r--   0        0        0      450 2024-05-06 06:19:11.927110 langjam-0.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-21 08:21:06.617635 langjam-0.1.6/src/langjam/__init__.py
--rw-r--r--   0        0        0        0 2024-02-12 04:13:22.069279 langjam-0.1.6/src/langjam/openai/__init__.py
--rw-r--r--   0        0        0        0 2024-02-12 06:59:55.786254 langjam-0.1.6/src/langjam/openai/openai_function/__init__.py
--rw-r--r--   0        0        0     4554 2024-02-15 08:05:02.108802 langjam-0.1.6/src/langjam/openai/openai_function/openai_function.py
--rw-r--r--   0        0        0      653 2024-02-14 17:02:38.025634 langjam-0.1.6/src/langjam/openai/openai_function/openai_function_model.py
--rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 langjam-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-01-21 09:11:55.610347 langjam-0.1.7/LICENSE
+-rw-r--r--   0        0        0      208 2024-02-13 03:22:07.507294 langjam-0.1.7/README.md
+-rw-r--r--   0        0        0      450 2024-05-16 09:53:43.066477 langjam-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-21 08:21:06.617635 langjam-0.1.7/src/langjam/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-12 04:13:22.069279 langjam-0.1.7/src/langjam/openai/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-12 06:59:55.786254 langjam-0.1.7/src/langjam/openai/openai_function/__init__.py
+-rw-r--r--   0        0        0     4623 2024-05-16 09:51:23.940330 langjam-0.1.7/src/langjam/openai/openai_function/openai_function.py
+-rw-r--r--   0        0        0      653 2024-02-14 17:02:38.025634 langjam-0.1.7/src/langjam/openai/openai_function/openai_function_model.py
+-rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 langjam-0.1.7/PKG-INFO
```

### Comparing `langjam-0.1.6/LICENSE` & `langjam-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `langjam-0.1.6/src/langjam/openai/openai_function/openai_function.py` & `langjam-0.1.7/src/langjam/openai/openai_function/openai_function.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,15 +57,17 @@
             params.append(key)
         return params
 
     @staticmethod
     async def _get_properties(model_json_schema: Dict[str, Any]) -> Dict[str, Dict[str, Any]]:
         properties: Dict[str, Dict[str, object]] = {}
         properties_initial_state = model_json_schema["properties"]
-        references = model_json_schema["$defs"]
+        references = {}
+        if "$defs" in model_json_schema:
+            references = model_json_schema["$defs"]
         for property_name in properties_initial_state:
             property_value = properties_initial_state[property_name]
             de_referenced_property: Dict[str, object] = await OpenaiFunction._get_de_referenced_property(
                 references,
                 property_value,
                 property_name
             )
```

### Comparing `langjam-0.1.6/src/langjam/openai/openai_function/openai_function_model.py` & `langjam-0.1.7/src/langjam/openai/openai_function/openai_function_model.py`

 * *Files identical despite different names*

### Comparing `langjam-0.1.6/PKG-INFO` & `langjam-0.1.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langjam
-Version: 0.1.6
+Version: 0.1.7
 Summary: Utils for large language model
 Author: Anurag Jha
 Author-email: toanuragjha@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

