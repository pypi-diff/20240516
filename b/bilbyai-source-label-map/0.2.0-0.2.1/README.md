# Comparing `tmp/bilbyai_source_label_map-0.2.0.tar.gz` & `tmp/bilbyai_source_label_map-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bilbyai_source_label_map-0.2.0.tar", max compression
+gzip compressed data, was "bilbyai_source_label_map-0.2.1.tar", max compression
```

## Comparing `bilbyai_source_label_map-0.2.0.tar` & `bilbyai_source_label_map-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2035 2024-05-16 05:00:29.186449 bilbyai_source_label_map-0.2.0/README.md
--rw-r--r--   0        0        0        0 2024-05-16 05:00:29.186449 bilbyai_source_label_map-0.2.0/bilbyai/__init__.py
--rw-r--r--   0        0        0      132 2024-05-16 05:00:29.186449 bilbyai_source_label_map-0.2.0/bilbyai/source_label_map/__init__.py
--rw-r--r--   0        0        0    18400 2024-05-16 05:00:29.186449 bilbyai_source_label_map-0.2.0/bilbyai/source_label_map/source_label_map.py
--rw-r--r--   0        0        0      505 2024-05-16 05:00:29.186449 bilbyai_source_label_map-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2529 1970-01-01 00:00:00.000000 bilbyai_source_label_map-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3067 2024-05-16 05:13:09.392161 bilbyai_source_label_map-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-16 05:13:09.392161 bilbyai_source_label_map-0.2.1/bilbyai/__init__.py
+-rw-r--r--   0        0        0      132 2024-05-16 05:13:09.392161 bilbyai_source_label_map-0.2.1/bilbyai/source_label_map/__init__.py
+-rw-r--r--   0        0        0    18400 2024-05-16 05:13:09.392161 bilbyai_source_label_map-0.2.1/bilbyai/source_label_map/source_label_map.py
+-rw-r--r--   0        0        0      505 2024-05-16 05:13:09.392161 bilbyai_source_label_map-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3561 1970-01-01 00:00:00.000000 bilbyai_source_label_map-0.2.1/PKG-INFO
```

### Comparing `bilbyai_source_label_map-0.2.0/README.md` & `bilbyai_source_label_map-0.2.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,87 @@
 # source_label_map
 
 Converts source code into human-friendly labels
 
 # Quickstart
 
+## Using `get_source_labels` directly
+
 ```python
 from bilbyai.source_label_map import get_source_labels
 
-# Get source labels for a list of inputs.
-label = get_source_labels("ben") # outputs ['Beijing Evening News']
+get_source_labels("ben") # outputs 'Beijing Evening News'
+
+get_source_labels(["gmwnews", "ben"]) # outputs ['Enlightenment Daily', 'Beijing Evening News']
+
+get_source_labels("cannot-be-found") # outputs 'cannot-be-found'
+
+get_source_labels("cannot-be-found", when_not_found="set_none") # outputs None
+
+get_source_labels("cannot-be-found", when_not_found="set_unknown") # outputs 'unknown'
+
+get_source_labels("ben", when_not_found="throw_error") # raises ValueError
+```
+
+
+## Using `get_source_labels` with DataFrames 
 
+```python
+import pandas as pd
+from bilbyai.source_label_map import get_source_labels
+
+df = pd.DataFrame(
+    {
+        "source": [
+            "gmwnews",
+            "ben",
+            "cannot-be-found",
+            "zqrb",
+        ]
+    }
+)
+
+# Option A: using list comprehension
+df["source_label"] = get_source_labels(df["source"])
+
+# Option B: using apply
+df["source_label"] = df["source"].apply(get_source_labels)
+
+df["source_label"]
+# Outputs: 
+# 0     Enlightenment Daily
+# 1    Beijing Evening News
+# 2         cannot-be-found
+# 3        Securities Daily
+# Name: source_label, dtype: object
 ```
 
+
+# Function Specs
 Get source labels for a list of inputs.
 
-Args:
-    `inputs` (`str | Iterable[str]`): The string or list of strings to get source labels for.
-    
-    `when_not_found`: The action to take when a source label is not found. Set to "preserve_source_name" by default.
-      - `"preserve_source_name"`: Preserve the source name as the source label. 
-      - `"set_to_none"`: Set the source label to None. 
-      - `"set_to_unknown"`: Set the source label to "unknown". 
-      - `"throw_error"`: Raise an error if a source label is not found. 
-    
-    source_label_dict: A dictionary mapping source names to source labels.
-
-Returns:
-    A list of source labels for the inputs.
-
-Raises:
-    ValueError: If the when_not_found value is not recognized.
-    ValueError: If the inputs are not a string or iterable of strings.
-    ValueError: If when_not_found is set to "throw_error" and a source label is not found.
+### Args:
+
+`inputs` (`str | Iterable[str]`): The string or list of strings to get source labels for.
+  
+`when_not_found`: The action to take when a source label is not found. Set to "preserve_source_name" by default.
+- `"preserve_source_name"`: Preserve the source name as the source label. 
+- `"set_to_none"`: Set the source label to None. 
+- `"set_to_unknown"`: Set the source label to "unknown". 
+- `"throw_error"`: Raise an error if a source label is not found. 
+
+`source_label_dict`: A dictionary mapping source names to source labels.
+
+### Returns:
+  A list of source labels for the inputs.
+
+### Raises:
+  `ValueError`: If the when_not_found value is not recognized.
+  `ValueError`: If the inputs are not a string or iterable of strings.
+  `ValueError`: If when_not_found is set to "throw_error" and a source label is not found.
 
 The project owner is [@leetdavid](https://github.com/leetdavid).
 
 ## Development
 
 If not already in a virtual environement, create and use one.
 Read about it in the Python documentation: [venv — Creation of virtual environments](https://docs.python.org/3/library/venv.html).
```

### Comparing `bilbyai_source_label_map-0.2.0/bilbyai/source_label_map/source_label_map.py` & `bilbyai_source_label_map-0.2.1/bilbyai/source_label_map/source_label_map.py`

 * *Files identical despite different names*

### Comparing `bilbyai_source_label_map-0.2.0/PKG-INFO` & `bilbyai_source_label_map-0.2.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bilbyai-source-label-map
-Version: 0.2.0
+Version: 0.2.1
 Summary: Converts source code into human-friendly labels
 Author: David Lee
 Author-email: leetdavidu@gmail.com
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -14,42 +14,88 @@
 
 # source_label_map
 
 Converts source code into human-friendly labels
 
 # Quickstart
 
+## Using `get_source_labels` directly
+
 ```python
 from bilbyai.source_label_map import get_source_labels
 
-# Get source labels for a list of inputs.
-label = get_source_labels("ben") # outputs ['Beijing Evening News']
+get_source_labels("ben") # outputs 'Beijing Evening News'
+
+get_source_labels(["gmwnews", "ben"]) # outputs ['Enlightenment Daily', 'Beijing Evening News']
+
+get_source_labels("cannot-be-found") # outputs 'cannot-be-found'
+
+get_source_labels("cannot-be-found", when_not_found="set_none") # outputs None
+
+get_source_labels("cannot-be-found", when_not_found="set_unknown") # outputs 'unknown'
+
+get_source_labels("ben", when_not_found="throw_error") # raises ValueError
+```
+
+
+## Using `get_source_labels` with DataFrames 
 
+```python
+import pandas as pd
+from bilbyai.source_label_map import get_source_labels
+
+df = pd.DataFrame(
+    {
+        "source": [
+            "gmwnews",
+            "ben",
+            "cannot-be-found",
+            "zqrb",
+        ]
+    }
+)
+
+# Option A: using list comprehension
+df["source_label"] = get_source_labels(df["source"])
+
+# Option B: using apply
+df["source_label"] = df["source"].apply(get_source_labels)
+
+df["source_label"]
+# Outputs: 
+# 0     Enlightenment Daily
+# 1    Beijing Evening News
+# 2         cannot-be-found
+# 3        Securities Daily
+# Name: source_label, dtype: object
 ```
 
+
+# Function Specs
 Get source labels for a list of inputs.
 
-Args:
-    `inputs` (`str | Iterable[str]`): The string or list of strings to get source labels for.
-    
-    `when_not_found`: The action to take when a source label is not found. Set to "preserve_source_name" by default.
-      - `"preserve_source_name"`: Preserve the source name as the source label. 
-      - `"set_to_none"`: Set the source label to None. 
-      - `"set_to_unknown"`: Set the source label to "unknown". 
-      - `"throw_error"`: Raise an error if a source label is not found. 
-    
-    source_label_dict: A dictionary mapping source names to source labels.
-
-Returns:
-    A list of source labels for the inputs.
-
-Raises:
-    ValueError: If the when_not_found value is not recognized.
-    ValueError: If the inputs are not a string or iterable of strings.
-    ValueError: If when_not_found is set to "throw_error" and a source label is not found.
+### Args:
+
+`inputs` (`str | Iterable[str]`): The string or list of strings to get source labels for.
+  
+`when_not_found`: The action to take when a source label is not found. Set to "preserve_source_name" by default.
+- `"preserve_source_name"`: Preserve the source name as the source label. 
+- `"set_to_none"`: Set the source label to None. 
+- `"set_to_unknown"`: Set the source label to "unknown". 
+- `"throw_error"`: Raise an error if a source label is not found. 
+
+`source_label_dict`: A dictionary mapping source names to source labels.
+
+### Returns:
+  A list of source labels for the inputs.
+
+### Raises:
+  `ValueError`: If the when_not_found value is not recognized.
+  `ValueError`: If the inputs are not a string or iterable of strings.
+  `ValueError`: If when_not_found is set to "throw_error" and a source label is not found.
 
 The project owner is [@leetdavid](https://github.com/leetdavid).
 
 ## Development
 
 If not already in a virtual environement, create and use one.
 Read about it in the Python documentation: [venv — Creation of virtual environments](https://docs.python.org/3/library/venv.html).
```

