# Comparing `tmp/bilbyai_source_label_map-0.1.0.tar.gz` & `tmp/bilbyai_source_label_map-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bilbyai_source_label_map-0.1.0.tar", max compression
+gzip compressed data, was "bilbyai_source_label_map-0.2.0.tar", max compression
```

## Comparing `bilbyai_source_label_map-0.1.0.tar` & `bilbyai_source_label_map-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      933 2024-05-16 03:58:47.150868 bilbyai_source_label_map-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-16 03:58:47.150868 bilbyai_source_label_map-0.1.0/bilbyai/__init__.py
--rw-r--r--   0        0        0      132 2024-05-16 03:58:47.150868 bilbyai_source_label_map-0.1.0/bilbyai/source_label_map/__init__.py
--rw-r--r--   0        0        0    18175 2024-05-16 03:58:47.150868 bilbyai_source_label_map-0.1.0/bilbyai/source_label_map/source_label_map.py
--rw-r--r--   0        0        0      505 2024-05-16 03:58:47.150868 bilbyai_source_label_map-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1427 1970-01-01 00:00:00.000000 bilbyai_source_label_map-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2035 2024-05-16 05:00:29.186449 bilbyai_source_label_map-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-16 05:00:29.186449 bilbyai_source_label_map-0.2.0/bilbyai/__init__.py
+-rw-r--r--   0        0        0      132 2024-05-16 05:00:29.186449 bilbyai_source_label_map-0.2.0/bilbyai/source_label_map/__init__.py
+-rw-r--r--   0        0        0    18400 2024-05-16 05:00:29.186449 bilbyai_source_label_map-0.2.0/bilbyai/source_label_map/source_label_map.py
+-rw-r--r--   0        0        0      505 2024-05-16 05:00:29.186449 bilbyai_source_label_map-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2529 1970-01-01 00:00:00.000000 bilbyai_source_label_map-0.2.0/PKG-INFO
```

### Comparing `bilbyai_source_label_map-0.1.0/bilbyai/source_label_map/source_label_map.py` & `bilbyai_source_label_map-0.2.0/bilbyai/source_label_map/source_label_map.py`

 * *Files 3% similar despite different names*

```diff
@@ -265,63 +265,73 @@
     "zqrb": "Securities Daily",
     "cbmd": "China Building Materials News",
     "zhongguoshuiwu": "China Tax Newspaper",
 }
 
 
 def get_source_labels(
-    inputs: str | Iterable[str],
+    sources: str | Iterable[str],
     *,
-    when_not_found: Literal[
-        "preserve_source_name", "set_to_none", "set_to_unknown", "throw_error"
-    ] = "preserve_source_name",
+    when_not_found: Literal["preserve", "set_none", "set_unknown", "raise_error"] = "preserve",
     source_label_dict: dict = source_label_dict,
 ):
-    """Get source labels for a list of inputs.
+    """Get source labels for a source or list of source.
 
     Args:
-        `inputs`: The list of inputs to get source labels for.
+        `source`: The list of inputs to get source labels for.
         `when_not_found`: The action to take when a source label is not found.
-            - `"preserve_source_name"`: Preserve the source name as the source label.
-            - `"set_to_none"`: Set the source label to None.
-            - `"set_to_unknown"`: Set the source label to "unknown".
-            - `"throw_error"`: Raise an error if a source label is not found.
+            - `"preserve"`: Preserve the source name as the source label.
+            - `"set_none"`: Set the source label to None.
+            - `"set_unknown"`: Set the source label to "unknown".
+            - `"raise_error"`: Raise an error if a source label is not found.
         `source_label_dict`: A dictionary mapping source names to source labels.
+        Set this value to override the default source label dictionary.
 
     Returns:
-        A list of source labels for the inputs.
+        A string or list of strings of source labels for the sources.
 
     Raises:
         ValueError: If the when_not_found value is not recognized.
-        ValueError: If the inputs are not a string or iterable of strings.
-        ValueError: If when_not_found is set to "throw_error" and a source label is not found.
+        ValueError: If the source(s) are not a string or a string iterable.
+        ValueError: If when_not_found is set to "raise_error" and a source label is not found.
     """
 
     if when_not_found not in [
-        "preserve_source_name",
-        "set_to_none",
-        "set_to_unknown",
-        "throw_error",
+        "preserve",
+        "set_none",
+        "set_unknown",
+        "raise_error",
     ]:
         raise ValueError(f"Unknown label_when_not_found value: {when_not_found}")
 
-    if isinstance(inputs, str):
-        inputs = [inputs]
+    if not isinstance(sources, Iterable) and not isinstance(sources, str):
+        raise TypeError(
+            f"source(s) must be a string or string iterable but instead got: {type(sources).__name__}"
+        )
 
-    if not isinstance(inputs, Iterable):
-        raise ValueError("inputs must be a string or iterable of strings")
+    is_single_input = isinstance(sources, str)
+
+    if is_single_input:
+        sources = [sources]
 
     source_labels = []
-    for input in inputs:
-        if input in source_label_dict:
-            source_labels.append(source_label_dict[input])
+    for source in sources:
+        if source in source_label_dict:
+            source_labels.append(source_label_dict[source])
+
         else:
-            if when_not_found == "preserve_source_name":
-                source_labels.append(input)
-            elif when_not_found == "set_to_none":
+            if when_not_found == "preserve":
+                source_labels.append(source)
+
+            elif when_not_found == "set_none":
                 source_labels.append(None)
-            elif when_not_found == "set_to_unknown":
+
+            elif when_not_found == "set_unknown":
                 source_labels.append("unknown")
-            else:
-                raise ValueError(f"Unknown label_when_not_found value: {when_not_found}")
+
+            elif when_not_found == "raise_error":
+                raise ValueError(f"key '{source}' not found in dict")
+
+    if is_single_input:
+        return source_labels[0]
 
     return source_labels
```

