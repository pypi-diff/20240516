# Comparing `tmp/bilbyai_source_label_map-0.2.1.tar.gz` & `tmp/bilbyai_source_label_map-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bilbyai_source_label_map-0.2.1.tar", max compression
+gzip compressed data, was "bilbyai_source_label_map-0.2.2.tar", max compression
```

## Comparing `bilbyai_source_label_map-0.2.1.tar` & `bilbyai_source_label_map-0.2.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3067 2024-05-16 05:13:09.392161 bilbyai_source_label_map-0.2.1/README.md
--rw-r--r--   0        0        0        0 2024-05-16 05:13:09.392161 bilbyai_source_label_map-0.2.1/bilbyai/__init__.py
--rw-r--r--   0        0        0      132 2024-05-16 05:13:09.392161 bilbyai_source_label_map-0.2.1/bilbyai/source_label_map/__init__.py
--rw-r--r--   0        0        0    18400 2024-05-16 05:13:09.392161 bilbyai_source_label_map-0.2.1/bilbyai/source_label_map/source_label_map.py
--rw-r--r--   0        0        0      505 2024-05-16 05:13:09.392161 bilbyai_source_label_map-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3561 1970-01-01 00:00:00.000000 bilbyai_source_label_map-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     3180 2024-05-16 05:17:06.981864 bilbyai_source_label_map-0.2.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-16 05:17:06.981864 bilbyai_source_label_map-0.2.2/bilbyai/__init__.py
+-rw-r--r--   0        0        0      132 2024-05-16 05:17:06.981864 bilbyai_source_label_map-0.2.2/bilbyai/source_label_map/__init__.py
+-rw-r--r--   0        0        0    18400 2024-05-16 05:17:06.981864 bilbyai_source_label_map-0.2.2/bilbyai/source_label_map/source_label_map.py
+-rw-r--r--   0        0        0      507 2024-05-16 05:17:06.981864 bilbyai_source_label_map-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3675 1970-01-01 00:00:00.000000 bilbyai_source_label_map-0.2.2/PKG-INFO
```

### Comparing `bilbyai_source_label_map-0.2.1/README.md` & `bilbyai_source_label_map-0.2.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 # source_label_map
 
 Converts source code into human-friendly labels
 
 # Quickstart
 
-## Using `get_source_labels` directly
+## Installation
+
+Install the package with pip:
+
+```bash
+pip install -U bilbyai-source-label-map
+```
+
+## Usage
+
+### Using `get_source_labels` directly
 
 ```python
 from bilbyai.source_label_map import get_source_labels
 
 get_source_labels("ben") # outputs 'Beijing Evening News'
 
 get_source_labels(["gmwnews", "ben"]) # outputs ['Enlightenment Daily', 'Beijing Evening News']
@@ -19,15 +29,15 @@
 
 get_source_labels("cannot-be-found", when_not_found="set_unknown") # outputs 'unknown'
 
 get_source_labels("ben", when_not_found="throw_error") # raises ValueError
 ```
 
 
-## Using `get_source_labels` with DataFrames 
+### Using `get_source_labels` with DataFrames 
 
 ```python
 import pandas as pd
 from bilbyai.source_label_map import get_source_labels
 
 df = pd.DataFrame(
     {
```

### Comparing `bilbyai_source_label_map-0.2.1/bilbyai/source_label_map/source_label_map.py` & `bilbyai_source_label_map-0.2.2/bilbyai/source_label_map/source_label_map.py`

 * *Files identical despite different names*

### Comparing `bilbyai_source_label_map-0.2.1/PKG-INFO` & `bilbyai_source_label_map-0.2.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: bilbyai-source-label-map
-Version: 0.2.1
-Summary: Converts source code into human-friendly labels
+Version: 0.2.2
+Summary: Converts news sources into human-friendly labels
 Author: David Lee
 Author-email: leetdavidu@gmail.com
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -14,15 +14,25 @@
 
 # source_label_map
 
 Converts source code into human-friendly labels
 
 # Quickstart
 
-## Using `get_source_labels` directly
+## Installation
+
+Install the package with pip:
+
+```bash
+pip install -U bilbyai-source-label-map
+```
+
+## Usage
+
+### Using `get_source_labels` directly
 
 ```python
 from bilbyai.source_label_map import get_source_labels
 
 get_source_labels("ben") # outputs 'Beijing Evening News'
 
 get_source_labels(["gmwnews", "ben"]) # outputs ['Enlightenment Daily', 'Beijing Evening News']
@@ -33,15 +43,15 @@
 
 get_source_labels("cannot-be-found", when_not_found="set_unknown") # outputs 'unknown'
 
 get_source_labels("ben", when_not_found="throw_error") # raises ValueError
 ```
 
 
-## Using `get_source_labels` with DataFrames 
+### Using `get_source_labels` with DataFrames 
 
 ```python
 import pandas as pd
 from bilbyai.source_label_map import get_source_labels
 
 df = pd.DataFrame(
     {
```

