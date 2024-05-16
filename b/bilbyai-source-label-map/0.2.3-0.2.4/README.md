# Comparing `tmp/bilbyai_source_label_map-0.2.3.tar.gz` & `tmp/bilbyai_source_label_map-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bilbyai_source_label_map-0.2.3.tar", max compression
+gzip compressed data, was "bilbyai_source_label_map-0.2.4.tar", max compression
```

## Comparing `bilbyai_source_label_map-0.2.3.tar` & `bilbyai_source_label_map-0.2.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3144 2024-05-16 05:25:20.336614 bilbyai_source_label_map-0.2.3/README.md
--rw-r--r--   0        0        0        0 2024-05-16 05:25:20.336614 bilbyai_source_label_map-0.2.3/bilbyai/__init__.py
--rw-r--r--   0        0        0      132 2024-05-16 05:25:20.336614 bilbyai_source_label_map-0.2.3/bilbyai/source_label_map/__init__.py
--rw-r--r--   0        0        0    18400 2024-05-16 05:25:20.336614 bilbyai_source_label_map-0.2.3/bilbyai/source_label_map/source_label_map.py
--rw-r--r--   0        0        0      507 2024-05-16 05:25:20.336614 bilbyai_source_label_map-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     3639 1970-01-01 00:00:00.000000 bilbyai_source_label_map-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     3452 2024-05-16 05:42:13.587460 bilbyai_source_label_map-0.2.4/README.md
+-rw-r--r--   0        0        0        0 2024-05-16 05:42:13.587460 bilbyai_source_label_map-0.2.4/bilbyai/__init__.py
+-rw-r--r--   0        0        0      132 2024-05-16 05:42:13.587460 bilbyai_source_label_map-0.2.4/bilbyai/source_label_map/__init__.py
+-rw-r--r--   0        0        0    18400 2024-05-16 05:42:13.587460 bilbyai_source_label_map-0.2.4/bilbyai/source_label_map/source_label_map.py
+-rw-r--r--   0        0        0      507 2024-05-16 05:42:13.587460 bilbyai_source_label_map-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     3947 1970-01-01 00:00:00.000000 bilbyai_source_label_map-0.2.4/PKG-INFO
```

### Comparing `bilbyai_source_label_map-0.2.3/README.md` & `bilbyai_source_label_map-0.2.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# source_label_map
+# Source Label Map
 
-Converts source code into human-friendly labels
+Converts news sources into human-friendly labels
 
 # Quickstart
 
 ## Installation
 
 Install the package with pip:
 
@@ -72,23 +72,31 @@
 
 
 # Function Specs
 Get source labels for a list of inputs.
 
 ### Args:
 
-`inputs` (`str | Iterable[str]`): The string or list of strings to get source labels for.
+`source` (`str | Iterable[str]`): The string or list of strings to get source labels for.
   
 `when_not_found`: The action to take when a source label is not found. Set to "preserve_source_name" by default.
-- `"preserve_source_name"`: Preserve the source name as the source label. 
-- `"set_to_none"`: Set the source label to None. 
-- `"set_to_unknown"`: Set the source label to "unknown". 
-- `"throw_error"`: Raise an error if a source label is not found. 
+- `"preserve"`: Preserve the source name as the source label. 
+- `"set_none"`: Set the source label to None. 
+- `"set_unknown"`: Set the source label to "unknown". 
+- `"raise_error"`: Raise an error if a source label is not found. 
 
-`source_label_dict`: A dictionary mapping source names to source labels.
+`source_label_dict`: A dictionary mapping source names to source labels. Set this value to override the default source label dictionary. It should be a dictionary mapping source names to source labels, like this:
+```python
+source_label_dict = {
+    "gmwnews": "Enlightenment Daily",
+    "sina_news": "Sina News",
+    "xueqiu": "Xueqiu (Snowball Finance)",
+    "peoplenews": "People's Daily",
+}
+```
 
 ### Returns:
   A list of source labels for the inputs.
 
 ### Raises:
   `ValueError`: If the when_not_found value is not recognized.
   `ValueError`: If the inputs are not a string or iterable of strings.
```

### Comparing `bilbyai_source_label_map-0.2.3/bilbyai/source_label_map/source_label_map.py` & `bilbyai_source_label_map-0.2.4/bilbyai/source_label_map/source_label_map.py`

 * *Files identical despite different names*

### Comparing `bilbyai_source_label_map-0.2.3/PKG-INFO` & `bilbyai_source_label_map-0.2.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: bilbyai-source-label-map
-Version: 0.2.3
+Version: 0.2.4
 Summary: Converts news sources into human-friendly labels
 Author: David Lee
 Author-email: leetdavidu@gmail.com
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 
-# source_label_map
+# Source Label Map
 
-Converts source code into human-friendly labels
+Converts news sources into human-friendly labels
 
 # Quickstart
 
 ## Installation
 
 Install the package with pip:
 
@@ -86,23 +86,31 @@
 
 
 # Function Specs
 Get source labels for a list of inputs.
 
 ### Args:
 
-`inputs` (`str | Iterable[str]`): The string or list of strings to get source labels for.
+`source` (`str | Iterable[str]`): The string or list of strings to get source labels for.
   
 `when_not_found`: The action to take when a source label is not found. Set to "preserve_source_name" by default.
-- `"preserve_source_name"`: Preserve the source name as the source label. 
-- `"set_to_none"`: Set the source label to None. 
-- `"set_to_unknown"`: Set the source label to "unknown". 
-- `"throw_error"`: Raise an error if a source label is not found. 
+- `"preserve"`: Preserve the source name as the source label. 
+- `"set_none"`: Set the source label to None. 
+- `"set_unknown"`: Set the source label to "unknown". 
+- `"raise_error"`: Raise an error if a source label is not found. 
 
-`source_label_dict`: A dictionary mapping source names to source labels.
+`source_label_dict`: A dictionary mapping source names to source labels. Set this value to override the default source label dictionary. It should be a dictionary mapping source names to source labels, like this:
+```python
+source_label_dict = {
+    "gmwnews": "Enlightenment Daily",
+    "sina_news": "Sina News",
+    "xueqiu": "Xueqiu (Snowball Finance)",
+    "peoplenews": "People's Daily",
+}
+```
 
 ### Returns:
   A list of source labels for the inputs.
 
 ### Raises:
   `ValueError`: If the when_not_found value is not recognized.
   `ValueError`: If the inputs are not a string or iterable of strings.
```

